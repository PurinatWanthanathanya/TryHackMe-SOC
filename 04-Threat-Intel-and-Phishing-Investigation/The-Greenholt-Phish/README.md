# Lab: The Greenholt Phish

**Role:** Junior Security Analyst

## 🎯 Objective
To investigate a simulated phishing campaign by analyzing email headers, verifying domain authentication protocols, and safely extracting and examining malicious attachments using threat intelligence tools.

## 🚀 Execution Steps
1. **Header Analysis & Origin Tracking:** 
   * Conducted a thorough analysis of the email headers to trace the true source of the phishing attempt.
   * Identified the originating IP address and performed OSINT research to determine the entity or ISP that owns the IP.
2. **Domain Authentication Verification:** 
   * Investigated the sender's domain legitimacy by performing SPF (Sender Policy Framework) and DMARC (Domain-based Message Authentication, Reporting, and Conformance) lookups to confirm email spoofing techniques.
3. **Attachment Triage & Extraction:** 
   * Safely handled and investigated a suspicious email attachment identified as a CAB (Cabinet) file.
   * Extracted the contents of the compressed archive in a controlled manner for further forensic examination.
4. **Malware Analysis via Threat Intel:** 
   * Calculated the SHA-256 cryptographic hash of the extracted payload.
   * Utilized VirusTotal to cross-reference the hash against global threat intelligence databases, verifying its malicious nature and identifying the specific malware signature.

## 📊 Results & Evidence
* Successfully dismantled the phishing attack by exposing the spoofed domain infrastructure, extracting the hidden payload from a CAB archive, and verifying the malware strain using SHA-256 hashing and VirusTotal.

> 📸 SPF<br><img width="1274" height="732" alt="image" src="https://github.com/user-attachments/assets/c1dab0ae-1b9a-42d9-9bd9-6496da602207" />

> 📸 VirusTotal<br><img width="1525" height="735" alt="image" src="https://github.com/user-attachments/assets/948db551-5a39-49d3-b18a-68b67c4b500d" />


## 🧠 Key Takeaways
* **Validating Email Infrastructure:** Reinforced the importance of checking SPF and DMARC records. Attackers frequently spoof trusted domains, and understanding these authentication protocols is critical for proving that an email did not originate from the claimed sender.
* **Handling Compressed Payloads:** Learned that attackers often hide malware inside compressed or archive formats like CAB files to bypass standard email gateway scans. Safely extracting and hashing these files is a fundamental SOC skill.
* **The Value of Cryptographic Hashes:** Realized that calculating a file's SHA-256 hash is one of the most definitive ways to identify malware. Searching a hash on platforms like VirusTotal provides immediate, actionable threat intelligence without needing to execute the file.
