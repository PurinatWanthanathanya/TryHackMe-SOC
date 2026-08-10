# Lab: Network Traffic Basics

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To analyze network traffic patterns and metadata for threat detection, understand TCP/IP stack vulnerabilities, and investigate protocol-specific anomalies to uncover hidden malicious activities such as data exfiltration and intrusion detection system (IDS) evasion.

## 🚀 Execution Steps
1. **Metadata Analysis (NetFlow & IPFIX):** 
   * Utilized network metadata protocols (NetFlow and IPFIX) to monitor high-volume endpoint traffic and establish baseline network behaviors.
   * Detected anomalous traffic patterns indicative of Command-and-Control (C2) communication and unauthorized data exfiltration without relying on resource-heavy full packet captures (PCAP).
2. **TCP/IP Stack Vulnerability Investigation:** 
   * Analyzed sophisticated network-level attacks exploiting the TCP/IP stack, including **TCP Session Hijacking** via sequence number manipulation.
   * Investigated **IP Fragmentation attacks** designed specifically to bypass and evade enterprise Intrusion Detection Systems (IDS).
3. **Application Layer Protocol Analysis:** 
   * Conducted deep-dive investigations into application-layer protocols, identifying malicious data encapsulated within standard traffic, such as **DNS Tunneling** (via subdomain structures).
   * Analyzed unencrypted HTTP traffic payloads and investigated authentication protocol workflows (e.g., SMB relying on Kerberos) to extract hidden artifacts and flags.

## 📊 Results & Evidence
* Successfully identified data exfiltration anomalies using NetFlow data, detected IDS-evading fragmented packets, and extracted hidden payloads from simulated HTTP and DNS traffic.

> 📸 <br><img width="1370" height="457" alt="image" src="https://github.com/user-attachments/assets/77601b5f-5568-4ae0-aeb4-91fb08581c03" />

> 📸 <br><img width="1210" height="212" alt="image" src="https://github.com/user-attachments/assets/2cdd1297-219b-4e0c-895c-3361087df99c" />

> 📸 <br><img width="1030" height="350" alt="image" src="https://github.com/user-attachments/assets/9f4d0ccc-d4cc-4bb4-8f87-414a1ac7d368" />

> 📸 <br><img width="1060" height="510" alt="image" src="https://github.com/user-attachments/assets/459b46f5-1108-4b96-8f31-e8f750285216" />

## 🧠 Key Takeaways
* **Metadata is Powerful:** Learned that full packet capture is not always necessary (or feasible) for threat detection. Metadata like **NetFlow** and **IPFIX** provides sufficient context to identify who is talking to whom, when, and how much data is being transferred—key indicators for spotting exfiltration.
* **Attackers Exploit the Rules:** Recognized how adversaries manipulate the rules of standard protocols to their advantage. Modifying TCP sequence numbers allows for session hijacking, while intentionally fragmenting IP packets can blind signature-based IDSs.
* **Protocol Blind Spots:** Understood that everyday protocols like DNS and HTTP are frequently abused. DNS is rarely blocked outbound, making it a prime candidate for covert C2 channels (DNS Tunneling) using complex subdomain structures.
