# Lab: MITRE

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To operationalize the MITRE ATT&CK framework for cyber threat intelligence and SOC investigations, map adversary Tactics, Techniques, and Procedures (TTPs) across Enterprise matrices, and leverage ATT&CK Navigator to identify defensive coverage gaps and optimize detection rules.

## 🚀 Execution Steps
1. **Adversary TTP Classification & ATT&CK Navigation:** 
   * Examined the core architecture of the **MITRE ATT&CK** Enterprise framework, distinguishing between overarching adversary objectives (**Tactics**) and specific technical executions (**Techniques** and **Sub-techniques**).
   * Investigated real-world threat actor profiles (Advanced Persistent Threat groups) and software suites documented within the framework to understand historical attack methodologies.
2. **Threat Emulation & ATT&CK Navigator Mapping:** 
   * Utilized the **MITRE ATT&CK Navigator** tool to generate visual matrices of simulated adversary attack campaigns.
   * Highlighted and layered specific threat actor TTPs across the matrix to model end-to-end intrusion paths and identify critical attack vectors requiring defensive prioritization.
3. **GAP Analysis & Detection Rule Alignment:** 
   * Cross-referenced enterprise SIEM and EDR log telemetry against the ATT&CK Matrix to perform a security posture gap analysis.
   * Formulated practical detection strategies and mitigation controls aligned with specific MITRE Technique IDs (e.g., `T1059` Command and Scripting Interpreter, `T1003` OS Credential Dumping) to harden enterprise defenses against known behavioral patterns.

## 📊 Results & Evidence
* Successfully mapped simulated threat actor campaigns using MITRE ATT&CK Navigator, identified organizational detection blind spots, and aligned security monitoring controls to specific MITRE Technique IDs.

> 📸 <br><img width="1549" height="773" alt="image" src="https://github.com/user-attachments/assets/103a105f-66d4-47b9-89cd-5f49e5d533b4" />

> 📸 <br><img width="1567" height="765" alt="image" src="https://github.com/user-attachments/assets/11c8f8c6-86f0-4aaf-92b0-3b19e3bdb996" />

## 🧠 Key Takeaways
* **The Global Standard for Threat Intel:** Learned that **MITRE ATT&CK** serves as the universal language for cybersecurity professionals, enabling SOC analysts, threat hunters, and engineers to communicate about threat behaviors without ambiguity.
* **Tactics vs. Techniques:**
  * **Tactics (The "Why"):** The adversary's tactical goal (e.g., *Privilege Escalation*, *Lateral Movement*).
  * **Techniques & Sub-techniques (The "How"):** The specific methods used to achieve that goal (e.g., *LSASS Memory Dumping*, *Pass the Hash*).
* **Data-Driven SOC Engineering:** Understood that mapping organizational detection capabilities against ATT&CK Navigator provides visual proof of security gaps, allowing security teams to strategically deploy SIEM rules and EDR policies where they matter most.
