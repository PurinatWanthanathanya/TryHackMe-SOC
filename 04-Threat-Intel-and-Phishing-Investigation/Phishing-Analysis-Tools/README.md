# Lab: Phishing Analysis Tools

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To operationalize a suite of technical phishing analysis tools to automate the extraction of Indicators of Compromise (IOCs), evaluate IP and URL reputations, decode obfuscated artifacts, and safely detonate malicious attachments within a sandbox environment.

## 🚀 Execution Steps
1. **Automated Header & Reputation Analysis:** 
   * Leveraged **PhishTool** to parse complex email headers rapidly and extract underlying routing data, sender IP addresses, and embedded URLs.
   * Conducted OSINT reputation checks against extracted indicators using platforms like **VirusTotal** to determine historical malicious activity and domain credibility.
2. **Artifact Decoding & Hash Calculation:** 
   * Utilized the data manipulation "Swiss Army Knife," **CyberChef**, to decode obfuscated payloads, specifically targeting Base64-encoded email attachments.
   * Applied command-line utilities (e.g., executing `sha256sum` in Linux) to generate cryptographic hashes of extracted files for accurate identification and threat intelligence correlation.
3. **Sandbox Detonation & Behavioral Observation:** 
   * Investigated specific social engineering campaigns (e.g., Netflix-impersonation phishing emails) by extracting suspicious PDF and Excel attachments.
   * Safely detonated the extracted attachments inside the **ANY.RUN** interactive malware sandbox to observe real-time behavioral indicators, network callbacks, and spawned processes without jeopardizing the host environment.

## 📊 Results & Evidence
* Successfully investigated a Netflix-impersonation phishing campaign by computing file hashes, defanging malicious URLs, decoding Base64 payloads via CyberChef, and observing macro execution inside the ANY.RUN sandbox.

> 📸 <br><img width="940" height="867" alt="image" src="https://github.com/user-attachments/assets/8402905c-bca5-45a3-94b8-efdd0cb510f4" />

> 📸 <br><img width="1903" height="920" alt="image" src="https://github.com/user-attachments/assets/33c16ee2-22eb-4939-98c6-57380c64fc3a" />

> 📸 <br><img width="1404" height="796" alt="image" src="https://github.com/user-attachments/assets/3b98b45a-baf6-4cd0-8e8d-ffe4b460a8b2" />

> 📸 <br><img width="1909" height="918" alt="image" src="https://github.com/user-attachments/assets/0bbab7e7-18d7-4305-ae58-ac827ae50f3d" />

> 📸 <br><img width="1919" height="873" alt="image" src="https://github.com/user-attachments/assets/f5f70618-3a6f-48dc-a058-bba1a27df732" />

> 📸 <br><img width="1591" height="814" alt="image" src="https://github.com/user-attachments/assets/15137d3e-3d02-4616-9a2e-668afd51e334" />

## 🧠 Key Takeaways
* **Tool Synergy Scales Analysis:** Learned that manual inspection is too slow for modern SOC environments. Combining tools (e.g., parsing with PhishTool $\rightarrow$ decoding with CyberChef $\rightarrow$ checking with VirusTotal) drastically accelerates triage workflows.
* **The Necessity of Sandboxes:** Recognized that static analysis (just looking at code) is often insufficient for modern malware. Detonating attachments in **ANY.RUN** safely reveals the dynamic behavior of the threat, such as unauthorized network connections or registry modifications.
* **Hashing as the Source of Truth:** Understood the importance of generating cryptographic hashes (`sha256sum`). Hashes act as a unique fingerprint for attachments, allowing analysts to definitively verify if a specific file has been previously flagged by the global cybersecurity community.
