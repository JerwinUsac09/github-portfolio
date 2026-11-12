# ICMP Denial-of-Service (DoS) Incident Analysis

## Project Overview

This project presents a simulated cybersecurity incident analysis based on a Denial-of-Service (DoS) attack against a multimedia company.

The incident involved an ICMP packet flood that disrupted network services for approximately two hours. The analysis applies the NIST Cybersecurity Framework to identify security gaps and recommend improvements across identification, protection, detection, response, and recovery.

## Scenario

A multimedia company experienced a DoS attack that caused internal network services to become unavailable for approximately two hours.

The investigation identified an unconfigured firewall as a security gap exploited by a malicious actor to flood network services with ICMP packets.

The organization subsequently implemented firewall rules, network monitoring software, and IDS/IPS capabilities to improve network security.

## NIST Cybersecurity Framework Analysis

### 1. Identify

- Identified an unconfigured firewall as a security weakness.
- Recognized the vulnerability in the network's security configuration.
- Analyzed how the exposed security gap contributed to the disruption of network services.

### 2. Protect

Recommended security improvements:

- Regularly audit and monitor firewall configurations and rules.
- Inspect and control incoming and outgoing network traffic.
- Implement source IP address verification to help detect spoofed addresses.
- Establish firewall controls for incoming ICMP traffic.
- Implement IDS/IPS and network monitoring capabilities.

### 3. Detect

Detection mechanisms identified:

- Network monitoring software to identify abnormal traffic patterns.
- Traffic filtering to restrict unauthorized or unnecessary network traffic.
- IDS/IPS capabilities to identify and handle suspicious ICMP traffic.

### 4. Respond

Incident response actions identified:

- Block or restrict malicious ICMP traffic to contain the attack.
- Temporarily disable non-critical network services when necessary.
- Investigate the incident and assess its impact.
- Mitigate the exploited security weaknesses.
- Prepare for service restoration using backups and baseline configurations.

### 5. Recover

Recovery measures identified:

- Restore critical network services.
- Utilize backup plans and baseline configurations.
- Maintain regular backups to support recovery from network disruptions.

## Key Learning Outcomes

- Understanding how firewall misconfigurations can contribute to network security incidents.
- Applying the NIST Cybersecurity Framework to a simulated security incident.
- Identifying preventive, detective, responsive, and recovery security measures.
- Understanding the importance of network monitoring, traffic filtering, and incident recovery planning.

## Disclaimer

This is a simulated cybersecurity case study completed as part of cybersecurity training. It does not represent a real-world incident handled professionally.
