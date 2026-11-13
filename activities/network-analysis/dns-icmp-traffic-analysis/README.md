# DNS and ICMP Traffic Analysis

## Overview

This activity demonstrates basic network traffic analysis using tcpdump as part of the Google Cybersecurity Certificate training.

The exercise involved investigating a connectivity issue affecting users who could not access a company website.

## Objective

Analyze captured network traffic to identify the affected network service, interpret DNS and ICMP messages, and determine possible causes of the connectivity issue.

## Tools and Protocols

**Tool:**
- tcpdump

**Protocols:**
- DNS
- UDP
- ICMP

## Investigation and Findings

The packet capture showed DNS queries being sent using UDP to destination port 53.

The DNS requests received ICMP Destination Unreachable messages indicating that UDP port 53 was unreachable.

This prevented successful DNS resolution, affecting users' ability to access the website through its domain name.

## Technical Analysis

The findings indicate a DNS connectivity problem.

The packet capture establishes that the DNS query could not reach an available service at the destination port. However, the exact underlying cause cannot be confirmed from this evidence alone.

Further investigation should include:

- Checking whether the DNS service is running and listening on port 53.
- Reviewing firewall rules and network filtering configurations.
- Verifying connectivity between the client and DNS server.
- Examining DNS server logs for additional errors.

## Skills Demonstrated

- Network traffic analysis using tcpdump
- Identifying DNS queries and ICMP error messages
- Understanding UDP port 53
- Interpreting packet capture findings
- Basic network troubleshooting and incident analysis

## Supporting Documentation

See the `reports` folder for the original incident report completed during the training activity.

## Disclaimer

This is a simulated cybersecurity training exercise. It does not represent an actual professional incident investigation.
