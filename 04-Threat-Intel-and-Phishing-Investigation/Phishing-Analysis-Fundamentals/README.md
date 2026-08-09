# Lab: Phishing Analysis Fundamentals

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To understand core email infrastructure and protocols, identify sophisticated social engineering vectors (such as Spear Phishing and Whaling), and conduct technical investigations of email headers, source code, and attachments while maintaining safe analysis environments.

## 🚀 Execution Steps
1. **Email Architecture & Protocol Analysis:** 
   * Examined the fundamental infrastructure of email delivery, analyzing the roles of core messaging protocols including **SMTP**, **POP3**, and **IMAP**.
   * Investigated the relationship between Domain Name System (DNS) records and email authentication mechanisms to understand how domains establish trust.
2. **Technical Header & Source Code Inspection:** 
   * Extracted and analyzed raw email headers to trace the true origin of suspicious messages, circumventing superficial Display Name deception.
   * Investigated email source code to identify malicious indicators, sender spoofing tactics, and psychological manipulation techniques (e.g., false urgency, authority impersonation).
3. **Payload Extraction & Safe Handling (Defanging):** 
   * Reconstructed and analyzed suspicious email attachments by decoding hidden **Base64** data streams within the raw email source.
   * Applied safe handling practices by **Defanging** potentially malicious URLs and IP addresses (e.g., converting `http` to `hxxp` and `.` to `[.]`) to neutralize threats before documenting them in security reports.

## 📊 Results & Evidence
* Successfully parsed email headers to expose sender spoofing, decoded Base64 malicious attachments, and applied defanging techniques to safely document actionable Indicators of Compromise (IOCs).

> 📸 <br><img width="950" height="863" alt="image" src="https://github.com/user-attachments/assets/4f62ed7d-2577-4bef-8361-751f384d60f7" />

> 📸 defang<br><img width="1919" height="898" alt="image" src="https://github.com/user-attachments/assets/93736461-3f83-4159-b44b-a098a98a9323" />

## 🧠 Key Takeaways
* **Never Trust the Display Name:** Learned that attackers routinely spoof display names to execute Spear Phishing and Whaling attacks. True attribution requires deep inspection of the email's underlying source code and routing headers.
* **Mastering the Protocols:** Understood that a solid grasp of SMTP, POP3, IMAP, and DNS is not just for IT administration; it is a critical prerequisite for tracing the digital footprint of a phishing campaign.
* **Safe Analysis Practices:** Recognized the importance of securely handling malicious artifacts. Defanging URLs and decoding attachments in isolated environments prevents accidental execution and protects the enterprise network during an ongoing investigation.
