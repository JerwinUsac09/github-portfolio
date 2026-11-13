# TCP SYN Flood Attack Analysis

## Overview

A simulated cybersecurity incident analysis activity completed as part of the Google Cybersecurity Certificate training.

The scenario involves a travel agency whose web server becomes unresponsive after receiving an unusually high volume of TCP SYN requests.

## Objective

Identify and analyze a suspected TCP SYN flood attack, understand its effect on server availability, and recommend appropriate security measures.

## Attack Identification

The large volume of incoming TCP SYN requests and resulting connection timeouts are consistent with a suspected TCP SYN flood, a type of Denial-of-Service (DoS) attack.

## Technical Analysis

### TCP Three-Way Handshake

A normal TCP connection is established through three steps:

1. **SYN:** The client requests a connection with the server.
2. **SYN-ACK:** The server acknowledges the request and responds with its own synchronization information.
3. **ACK:** The client acknowledges the server's response, completing the handshake.

### How a SYN Flood Works

In a SYN flood attack, an attacker sends numerous TCP SYN requests. Some connection attempts do not complete the final ACK step.

The server may retain resources for these pending, half-open connections. If enough accumulate, the server's connection backlog or other resources can become exhausted, preventing legitimate users from establishing connections.

## Recommended Security Measures

- **SYN cookies:** Help protect server resources when handling large numbers of pending TCP connections.
- **Rate limiting:** Restrict excessive connection requests.
- **Anti-spoofing filters:** Help prevent forged or invalid source IP addresses from entering the network.
- **Network monitoring:** Monitor unusual SYN traffic and server resource utilization.
- **DDoS protection:** Consider upstream protection to help absorb or mitigate large-scale attacks.

Blocking one suspicious IP address alone may not be sufficient because attackers can change or spoof source IP addresses.

## Skills Demonstrated

- Understanding TCP connection establishment
- Recognizing potential SYN flood indicators
- Analyzing Denial-of-Service attacks
- Understanding half-open TCP connections
- Identifying security controls and mitigation strategies

## Supporting Documentation

See the `reports` folder for the original incident report completed during training.

## Disclaimer

This is a simulated cybersecurity training exercise, not an actual professional incident investigation or hands-on packet capture.
