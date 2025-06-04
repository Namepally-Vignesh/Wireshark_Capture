# Capture and Analyze Network Traffic Using Wireshark
## Objective
The objective of this task was to capture live network packets and analyze the traffic to identify basic protocols and types of communication using Wireshark.
## Contents
- **Packet Capture File:** `capture.pcap` - This file contains the captured network packets during the session.
- **Screenshots:** 
  - `wireshark_interface.png` - Screenshot of the Wireshark interface during packet capture.
  - `filtering_packets (http, icmp, dns, tcp, tls)` - Screenshots showing the application of filters in Wireshark.
- **Summary Report:** `report.txt` - A brief report summarizing the protocols identified and observations made during the analysis.

## Steps Followed
1. Already Installed Wireshark in Kali Linux.
2. Captured packets on `eth0` for 60 seconds while:
   - Browsing `example.com` 
   - Pinging `8.8.8.8`
   - as i have chosen the testphp.vulnweb.com
3. Stopped the capture and filtered protocols:
   - DNS
   - HTTP
   - ICMP
   - TLS
4. Analyzed packet details: source/destination IPs, request types, headers.

## Conclusion
The packet capture provided insights into the types of protocols commonly used in web traffic. HTTP and DNS were the most active protocols, reflecting typical user behavior while browsing the internet. The presence of TCP packets confirmed the reliability of the connections established during the capture.
