Enterprise DNS Security Lab using BIND9 on Ubuntu


Overview : 
Enterprise DNS Security Lab is a hands-on cybersecurity project that demonstrates the deployment, administration, monitoring, and security of a DNS infrastructure using BIND9 on Ubuntu Linux.
The project implements both authoritative and recursive DNS services, integrates Response Policy Zones (RPZ) for domain blocking, enables DNS query and RPZ logging, analyzes DNS traffic using Wireshark, and simulates DNS tunneling using Bash scripts. The implementation is correlated with the MITRE ATT&CK Framework to demonstrate how DNS can be abused and monitored in enterprise environments.


Features : 
Authoritative DNS Server using BIND9
Recursive DNS Resolution
Forward Lookup Zones
Reverse Lookup Zones (PTR Records)
Nginx Web Server Integration
Response Policy Zones (RPZ)
DNS Query Logging
RPZ Event Logging
Wireshark DNS Packet Analysis
Bash-based DNS Tunneling Simulation
MITRE ATT&CK Mapping (T1572 – Protocol Tunneling)



Lab Architecture : 

<img width="236" height="335" alt="image" src="https://github.com/user-attachments/assets/c299337c-ef9e-4601-9227-29de3c9dd178" />






Project Workflow : 
Configure authoritative DNS zones.
Configure recursive DNS resolution.
Create forward and reverse lookup zones.
Integrate Nginx-hosted web applications.
Implement Response Policy Zones (RPZ).
Enable DNS query logging.
Enable RPZ event logging.
Analyze DNS packets using Wireshark.
Simulate DNS tunneling using Bash scripts.
Correlate the activity with MITRE ATT&CK.


DNS Tunneling Simulation : 
The script - 
Base64-encodes a sample file
Splits it into DNS-safe chunks
Sends each chunk as a DNS query
Generates observable DNS traffic

Example - 
1.VXNlcm5hbWU.attacker.test
2.YWRtaW4.attacker.test
