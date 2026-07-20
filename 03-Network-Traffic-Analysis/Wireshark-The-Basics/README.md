# Lab: Wireshark: The Basics

**Role:** Junior Security Analyst

## 🎯 Objective
To understand the fundamentals of network traffic analysis using Wireshark, inspect packets across the OSI model layers, and utilize advanced filtering and flow analysis techniques to investigate PCAP (Packet Capture) files for anomalies.

## 🚀 Execution Steps
1. **PCAP Ingestion & Initial Assessment:** 
   * Imported raw PCAP files into Wireshark for deep packet inspection.
   * Utilized the **Expert Info** feature to quickly identify network anomalies, malformed packets, and protocol errors before diving into manual analysis.
2. **Packet Filtering & Dissection:** 
   * Applied specific display filters to isolate relevant traffic (e.g., filtering by IP, port, or specific protocols) and reduce network noise.
   * Dissected individual packets, examining the headers and payloads through the lens of the OSI model layers (from the Data Link layer up to the Application layer).
3. **Traffic Flow Analysis & Artifact Extraction:** 
   * Used the **Follow Stream** feature (TCP/UDP/HTTP) to logically reconstruct fragmented packets and view the complete, readable conversation between a client and a server.
   * Executed the **Export Objects** function to extract transferred files directly from the network capture for further malware or forensic analysis.
4. **Documentation & Evidence Management:** 
   * Marked important packets and added contextual comments directly within the capture file to document investigative findings.
   * Exported specific filtered streams to save as concrete evidence for incident reporting.

## 📊 Results & Evidence
* Successfully navigated and analyzed raw network traffic, filtered out irrelevant data, reconstructed communication streams, and extracted hidden artifacts from the provided PCAP files.

> 📸 Display Filter 'http'<br><img width="658" height="523" alt="image" src="https://github.com/user-attachments/assets/23a162bb-9747-44f5-a661-ae83a2dc96ba" />

> 📸 Follow HTTP Stream<br><img width="680" height="533" alt="image" src="https://github.com/user-attachments/assets/7674051b-781f-49ac-8f77-9b5a47e30366" />

## 🧠 Key Takeaways
* **Packet Analyzer vs. IDS:** Learned that Wireshark is a powerful open-source packet analyzer used for traffic sniffing and forensic PCAP analysis, but it is not an Intrusion Detection System (IDS); it requires an analyst's manual interpretation to identify threats.
* **The Power of 'Follow Stream':** Realized that analyzing individual packets can be confusing, but reconstructing the entire flow provides a clear, human-readable view of the communication and potential data exfiltration.
* **Efficient Triage with Expert Info:** Discovered that utilizing Wireshark's Expert Info is a crucial first step in any investigation, as it automatically highlights warnings and errors that might indicate an attack or network misconfiguration.
* **Mastering Filters:** Concluded that effective network analysis heavily relies on mastering display filters to quickly pinpoint suspicious activities within massive network captures.
