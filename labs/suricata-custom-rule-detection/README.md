# Suricata Custom Rule Detection and Log Analysis

## Overview
A hands-on network security monitoring lab completed as part of the Google Cybersecurity Certificate. This activity involved configuring a custom Suricata detection rule, analyzing network traffic from a packet capture file, and examining generated security alerts.

## Objective
Use Suricata to detect HTTP GET requests in captured network traffic, generate alerts using a custom rule, and examine the resulting logs to understand how an intrusion detection system records network events.

## Tools and Technologies
- **Suricata** – Open-source network threat detection engine.
- **PCAP** – Sample packet capture file used for traffic analysis.
- **EVE JSON** – Structured event logging format.
- **fast.log** – Human-readable alert log.
- **jq** – Command-line tool for filtering and examining JSON data.
- Linux terminal

## Tasks Performed

### 1. Examine the Custom Detection Rule
Reviewed and modified a custom Suricata rule to detect HTTP GET requests.

```text
alert http $HOME_NET any -> $EXTERNAL_NET any (msg:"GET on wire"; flow:established,to_server; content:"GET"; http_method; sid:12345; rev:3;)
```

The rule generates an alert when matching HTTP GET requests travel from the defined home network toward an external network.

### 2. Run Suricata Against a PCAP File
Executed Suricata against the supplied packet capture using the custom rule file.

```bash
sudo suricata -r sample.pcap -S custom.rules -k none
```

Suricata successfully processed 200 packets and generated log files.

### 3. Examine fast.log
Reviewed the generated `fast.log` file and identified two alerts matching the custom rule.

Both alerts involved:
- Signature ID: `12345`
- Signature message: `GET on wire`
- Protocol: TCP
- Destination port: 80
- Priority: 3

### 4. Examine EVE JSON
Inspected `eve.json` to examine the structured alert information.

The event details included:
- Source and destination IP addresses
- Source and destination ports
- HTTP request method
- Requested hostname and URL
- Alert signature and severity
- HTTP response status and redirect information

One observed event contained an HTTP GET request to `opensource.google.com` and an HTTP 301 redirect response.

### 5. Filter JSON Events Using jq
Used `jq` to examine EVE JSON records and extract relevant event information.

This demonstrated how analysts can filter structured security logs and focus on specific alert fields during an investigation.

## Key Findings
- The custom Suricata rule successfully matched HTTP GET requests in the supplied packet capture.
- Two matching alerts appeared in `fast.log`.
- EVE JSON provided additional information about the detected HTTP events.
- The generated alerts had an `allowed` action, meaning the traffic was detected but not blocked.

## Security Concepts Demonstrated
- Intrusion Detection Systems (IDS)
- Custom network detection rules
- HTTP traffic inspection
- Packet capture analysis
- Security alert investigation
- Structured event logging
- JSON filtering and analysis
- Difference between detection and prevention

## Skills Demonstrated
- Configuring custom Suricata signatures
- Running Suricata against PCAP files
- Interpreting IDS alerts
- Examining `fast.log` and EVE JSON
- Using `jq` to inspect structured logs
- Identifying relevant network traffic information

## Evidence
Selected terminal screenshots demonstrating rule configuration, Suricata execution, and alert analysis will be included in the `screenshots` folder.

## Disclaimer
This activity was completed in a simulated training environment using a supplied packet capture file. The alerts demonstrate rule matching and network monitoring, not the detection of a confirmed malicious attack.
