# Lab: Wireshark: Traffic Analysis

**Role:** Junior Security Analyst / Network Threat Hunter Trainee

## 🎯 Objective
To perform deep-packet inspection across various network protocols, detect covert channels and network scanning techniques, decrypt secure communications for exploit analysis (Log4j), and identify active Man-in-the-Middle (MitM) attacks within captured network traffic.

## 🚀 Execution Steps
1. **Cleartext Protocol & Encrypted Traffic Analysis:** 
   * Inspected unencrypted traffic protocols (HTTP, FTP) to hunt for exposed credentials and plain-text payloads.
   * Utilized TLS decryption keys to inspect encrypted HTTPS traffic, isolating critical exploitation attempts such as the **Log4j** vulnerability.
2. **Host Identification & Tunneling Detection:** 
   * Leveraged DHCP, NetBIOS, and Kerberos traffic to identify and map active hostnames and network entities.
   * Applied specialized display filters to detect covert data exfiltration and Command-and-Control (C2) channels via **ICMP and DNS Tunneling**.
3. **Reconnaissance & MitM Threat Detection:** 
   * Analyzed network scanning signatures to distinguish between **TCP Connect** and **SYN Stealth** scans executed by reconnaissance tools like Nmap.
   * Conducted ARP packet analysis to identify network manipulation attempts, successfully detecting **ARP Poisoning / Man-in-the-Middle (MitM)** attacks.
4. **Remediation & Rule Generation:** 
   * Translated identified malicious traffic patterns into actionable firewall and network defense rules to prevent further unauthorized access.

## 📊 Results & Evidence
* Successfully decrypted HTTPS sessions to identify exploit attempts, isolated covert ICMP/DNS tunnels, detected Nmap reconnaissance scans, and identified spoofed ARP packets.

> 📸 TCP Connect<br><img width="994" height="728" alt="image" src="https://github.com/user-attachments/assets/d31c8829-3f8c-4a43-91d9-50c381e47a2f" />

> 📸 UDP close port<br><img width="999" height="739" alt="image" src="https://github.com/user-attachments/assets/6ad04b4d-b20f-47aa-a5d0-a06faadfb607" />

> 📸 Which UDP port in the 55-70 port range is open<br><img width="995" height="731" alt="image" src="https://github.com/user-attachments/assets/f41d2a3c-6308-4a09-a27c-669ed8d83062" />

> 📸 number of ARP requests crafted by the attacker<br><img width="985" height="741" alt="image" src="https://github.com/user-attachments/assets/942b53cf-2893-44ac-95df-9331b5c5412c" />

> 📸 HTTP packets received by the attacker<br><img width="976" height="722" alt="image" src="https://github.com/user-attachments/assets/da3426f6-a61b-4d6b-aa28-00be91eb9b4e" />

> 📸 MAC address of the host "Galaxy A30"<br><img width="981" height="721" alt="image" src="https://github.com/user-attachments/assets/0d83df36-d76c-4a8e-a1e0-57fcce35cd12" />

> 📸 NetBIOS registration requests does the "LIVALJM" workstation<br><img width="983" height="745" alt="image" src="https://github.com/user-attachments/assets/5603114d-d25a-4161-a99e-617d68e55ab1" />

> 📸 Which host requested the IP address "172.16.13.85"<br><img width="993" height="729" alt="image" src="https://github.com/user-attachments/assets/eb74b8e8-c04b-4365-96ef-297b8dfaa32c" />


## 🧠 Key Takeaways
* **Cleartext is a Vulnerability:** Learned that unencrypted protocols like FTP and HTTP expose sensitive credentials directly to anyone listening on the wire, making transition to encrypted alternatives mandatory.
* **Decryption Grants Visibility:** Recognized that modern threats hide inside encrypted HTTPS traffic; leveraging session keys allows analysts to inspect payloads for severe threats like Log4j safely.
* **Tunneling & Spoofing Signatures:** Understood how to spot malicious behavior—unusually large ICMP payloads or high-volume DNS queries indicate covert tunneling, while rapid unsourced ARP replies signal ARP Poisoning attacks.
