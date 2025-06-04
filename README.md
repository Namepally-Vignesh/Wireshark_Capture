# Capture and Analyze Network Traffic Using Wireshark
## Objective
The objective of this task was to capture live network packets and analyze the traffic to identify basic protocols and types of communication using Wireshark.
## Contents
- **Packet Capture File:** `capture.pcap` - This file contains the captured network packets during the session.
- **Screenshots:** 
  - `wireshark_interface.png` - Screenshot of the Wireshark interface during packet capture.
  - `filtering_packets (http, icmp, dns, tcp, tls)` - Screenshots showing the application of filters in Wireshark.

## Steps Followed
1. Already Installed Wireshark in Kali Linux.
2. Captured packets on `eth0` for 60 seconds while:
   - Browsing `example.com` 
   - Pinging `8.8.8.8`
   - as i have chosen the testphp.vulnweb.com
3. Stopped the capture and filtered protocols:
   - HTTP
   - DNS
   - TCP
   - ICMP
4. Analyzed packet details: source/destination IPs, request types, headers.

## Summary
In this task, I installed/upgraded Wireshark on a Linux virtual machine, captured live network traffic while browsing the website and analyzed the captured packets.
The key protocols identified include:

1. **HTTP (Hypertext Transfer Protocol)**
   - **Purpose:** Used for transferring web pages and facilitating communication between web browsers and servers.
   - **Observations:** Captured multiple HTTP requests and responses, including GET and POST methods.

2. **DNS (Domain Name System)**
   - **Purpose:** Translates human-readable domain names into IP addresses.
   - **Observations:** Captured several DNS queries and responses, indicating name resolution activities.

3. **TCP (Transmission Control Protocol)**
   - **Purpose:** A connection-oriented protocol that ensures reliable data transmission.
   - **Observations:** Noted numerous TCP packets, including SYN, ACK, and FIN flags, indicating the establishment and termination of connections.

4. **ICMP (Internet Control Message Protocol)**
   - **Purpose:** Used for sending error messages and operational information.
   - **Observations:** Captured echo request and reply packets from the ping command.

## Conclusion
The packet capture provided insights into the types of protocols commonly used in web traffic. HTTP and DNS were the most active protocols, reflecting typical user behavior while browsing the internet. The presence of TCP packets confirmed the reliability of the connections established during the capture.
