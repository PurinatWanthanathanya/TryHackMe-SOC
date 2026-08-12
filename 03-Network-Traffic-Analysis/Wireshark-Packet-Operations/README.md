# Lab: Wireshark: Packet Operations

**Role:** Junior Security Analyst / Network Traffic Analyst Trainee

## 🎯 Objective
To master advanced packet inspection methodologies in Wireshark, leveraging complex display filtering, string functions, custom analyst profiles, and statistical traffic analysis to rapidly detect anomalies and streamline incident investigation workflows.

## 🚀 Execution Steps
1. **Advanced Display Filtering & String Manipulation:** 
   * Deployed advanced filtering operators (`contains`, `matches`, `in`) to isolate precise threat artifacts within large PCAP files.
   * Utilized string manipulation functions (`upper`, `lower`, `string`) to normalize and search packet payloads regardless of case sensitivity or encoding variations.
2. **Workflow Optimization & Environment Customization:** 
   * Customized Wireshark operational profiles to suit specific threat-hunting scenarios.
   * Configured custom display filter buttons and saved bookmarks for frequently used queries, significantly reducing investigation triage times.
3. **Statistical Analysis & Network Profiling:** 
   * Utilized the **Statistics** menu to analyze **Protocol Hierarchy**, **Endpoints**, and **Conversations** to identify anomalous bandwidth spikes or unrecognized communicating IP addresses.
   * Evaluated resolved addresses to detect malicious hostname resolutions.
   * Differentiated between **Capture Filters** (applied pre-capture to limit data collection scope) and **Display Filters** (applied post-capture for dynamic payload reduction and analysis).

## 📊 Results & Evidence
* Successfully isolated hidden payload threats using string-based display filters, optimized analyst workspace efficiency via custom profiles, and mapped high-volume network conversations using Wireshark statistics.

> 📸 resolved addresses<br><img width="984" height="723" alt="image" src="https://github.com/user-attachments/assets/f7430db3-20e6-4d97-9c46-a7174793bb65" />

> 📸 IPv4 conversations<br><img width="985" height="724" alt="image" src="https://github.com/user-attachments/assets/a2df3182-5635-47f1-9f37-bb7124a32295" />

> 📸 <br><img width="986" height="735" alt="image" src="https://github.com/user-attachments/assets/d885e4db-cb72-44dd-9a00-cf1e4eb044c4" />
          
> 📸 <br><img width="969" height="722" alt="image" src="https://github.com/user-attachments/assets/5741924d-f517-47bf-9367-b680271f8a28" />

> 📸 the most used IPv4 destination address<br><img width="960" height="712" alt="image" src="https://github.com/user-attachments/assets/4240d41e-9a48-404d-b9a2-496ffa733e6d" />

> 📸 request-response time of the DNS packets<br><img width="988" height="715" alt="image" src="https://github.com/user-attachments/assets/05db120e-a380-45f6-ab67-7302daf330fd" />

> 📸 <br><img width="1001" height="720" alt="image" src="https://github.com/user-attachments/assets/895922c0-73c5-40e1-853d-5f3915826940" />

> 📸 <br><img width="1008" height="730" alt="image" src="https://github.com/user-attachments/assets/2f852cdd-f2b4-44ba-8cfb-2b03fa2e950e" />

> 📸 TTL value less than 10<br><img width="992" height="727" alt="image" src="https://github.com/user-attachments/assets/03cada2e-a1d3-49da-8f76-b2b86088ff7b" />

> 📸 packets which uses "TCP port 4444"<br><img width="992" height="728" alt="image" src="https://github.com/user-attachments/assets/ec472dfa-f4f1-4a3c-be24-ab9e9fc92237" />

> 📸 "HTTP GET" requests sent to port "80"<br><img width="1002" height="738" alt="image" src="https://github.com/user-attachments/assets/dde500a2-6eeb-4164-8040-022d5afb3862" />

> 📸 DNS Queries<br><img width="999" height="749" alt="image" src="https://github.com/user-attachments/assets/b068222b-22dd-4a70-abbe-162bdfec1468" />

> 📸 Microsoft IIS servers did not originate from "port 80"<br><img width="1002" height="745" alt="image" src="https://github.com/user-attachments/assets/988fcc5d-dfd2-478e-b79d-299d8cb6bbed" />

> 📸 Microsoft IIS servers have version 7.5<br><img width="1002" height="741" alt="image" src="https://github.com/user-attachments/assets/59120b0e-45b1-443c-8f7b-5c0444c29117" />

> 📸 packets that use ports 3333, 4444 or 9999<br><img width="999" height="723" alt="image" src="https://github.com/user-attachments/assets/c6036d7c-bb09-427f-b7bf-aee4a74c265c" />

> 📸 packets with "even TTL numbers"<br><img width="1003" height="735" alt="image" src="https://github.com/user-attachments/assets/3802ba7b-c7b5-4f1b-848a-bf5716dce439" />

> 📸 Change the profile to "Checksum Control" and number "Bad TCP Checksum" packets<br><img width="1003" height="740" alt="image" src="https://github.com/user-attachments/assets/5cd402ed-5e9d-443a-a33a-d5daa3ef56fc" />

> 📸 <br><img width="998" height="739" alt="image" src="https://github.com/user-attachments/assets/9cf5d142-738e-4057-b245-eff11df52c81" />

## 🧠 Key Takeaways
* **Filter with Precision:** Learned that basic filters are often not enough during an active incident. Using advanced operators like `contains` and case-insensitive functions allows analysts to find hidden payloads embedded in HTTP or DNS traffic quickly.
* **Statistics Reveal Anomalies:** Recognized that the **Statistics Menu** is an analyst's best starting point. Instead of reading packets one by one, inspecting the Protocol Hierarchy and Endpoints immediately surfaces abnormal traffic patterns or C2 beacons.
* **Capture vs. Display Filters:** Understood the fundamental operational difference: Capture Filters reduce the raw packet intake at the interface level, while Display Filters allow analysts to dynamically parse and drill down into collected data without altering the source capture.
