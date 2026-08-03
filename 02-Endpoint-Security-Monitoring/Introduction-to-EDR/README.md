# Lab: Introduction to EDR

**Role:** Junior Security Analyst / SOC Analyst

## 🎯 Objective
To understand the architecture and operational capabilities of Endpoint Detection and Response (EDR) solutions, differentiate behavioral threat detection from traditional signature-based antivirus, and execute real-time incident response actions such as process analysis and host isolation.

## 🚀 Execution Steps
1. **EDR Architecture & Telemetry Analysis:** 
   * Examined the core components of an EDR deployment, monitoring how lightweight endpoint agents continuously stream behavioral telemetry to a centralized management console.
   * Differentiated between traditional signature-based Antivirus (AV) and advanced EDR capabilities, focusing on behavioral analysis, machine learning, and the detection of fileless malware.
2. **Investigation via Process Tree Visualization:** 
   * Investigated suspicious alerts within the EDR dashboard by examining **Process Tree Visualizations** to establish parent-child process relationships.
   * Traversed command-line arguments and execution lineages to uncover stealthy persistence mechanisms and identify malicious scripts spawned by legitimate system processes.
3. **Endpoint Response & Containment Execution:** 
   * Executed immediate EDR response actions to contain simulated intrusions without wiping the endpoint.
   * Performed targeted **Process Termination** to halt active malicious threads and initiated **Host Isolation** (network quarantine) to block lateral movement while preserving remote access for forensic investigation.

## 📊 Results & Evidence
* Successfully analyzed endpoint telemetry via Process Tree diagrams, identified behavioral threat indicators bypassing traditional AV, and executed containment procedures via process termination and host isolation.

> 📸 <br><img width="814" height="745" alt="image" src="https://github.com/user-attachments/assets/943ad257-2950-40f0-a0a7-727bd35198c0" />

> 📸 <br><img width="807" height="726" alt="image" src="https://github.com/user-attachments/assets/da37d1b2-92e5-4339-b6ae-2c73b949200f" />

> 📸 <br><img width="794" height="750" alt="image" src="https://github.com/user-attachments/assets/45512121-0982-4343-9bdc-d5df7f2357ef" />

> 📸 <br><img width="812" height="755" alt="image" src="https://github.com/user-attachments/assets/ce87e70d-6734-4feb-a86f-a5722270e6e2" />

> 📸 <br><img width="817" height="744" alt="image" src="https://github.com/user-attachments/assets/86a82a27-01cc-4d8d-a055-eb61d83059f7" />

## 🧠 Key Takeaways
* **Beyond Signature-Based Detection:** Learned that modern adversaries easily bypass static AV signatures. EDR is critical because it monitors *behavior* (e.g., PowerShell launching an unknown executable or modifying registry keys), allowing SOC analysts to catch zero-day and fileless attacks.
* **The Power of Process Trees:** Recognized that visualizing parent-child process relationships is vital for root-cause analysis. It enables analysts to quickly trace an alert back to its initial entry vector (e.g., a malicious Word document spawning a command shell).
* **Rapid & Precise Containment (Host Isolation):** Understood that containing a threat no longer requires physically pulling a network cable. EDR's **Host Isolation** feature cuts off the infected machine from the enterprise network while maintaining a secure administrative channel for the SOC team to conduct remote forensics.
