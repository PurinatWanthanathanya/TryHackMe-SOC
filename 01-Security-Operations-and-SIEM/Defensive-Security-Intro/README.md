# Lab: Defensive Security Intro

**Role:** Junior Security Analyst

## 🎯 Objective
To understand the core responsibilities of a Security Operations Centre (SOC), practice structured incident triage, execute containment strategies on compromised accounts, and leverage threat intelligence to document security incidents effectively.

## 🚀 Execution Steps
1. **Security Monitoring & Alert Assessment:** 
   * Monitored simulated SOC dashboards to identify incoming security alerts and suspicious activities across the enterprise environment.
   * Followed the defensive principle of thoroughly assessing and understanding the scope of an incident before rushing into remediation.
2. **Incident Investigation & Account Containment:** 
   * Investigated an alert involving unauthorized access and anomalous behavior linked to a specific user account.
   * Executed immediate containment measures by locking the compromised user account (`dave.saunders`) to halt the ongoing attack and prevent lateral movement.
3. **Threat Intelligence Correlation:** 
   * Consulted internal threat intelligence reports to identify adversary Tactics, Techniques, and Procedures (TTPs).
   * Correlated the observed attack indicators with known threat actor profiles, specifically tracking the activities of the `ShadowFigures` group.
4. **Incident Reporting & Documentation:** 
   * Compiled a formal post-incident report detailing the timeline of events, root cause analysis, and remediation actions taken.
   * Documented findings to support future team training and improve defensive detection rules.

## 📊 Results & Evidence
* Successfully triaged a simulated breach, contained the threat by locking down the compromised `dave.saunders` account, and correlated the attack with `ShadowFigures` threat intelligence to produce a comprehensive incident report.

> 📸 Attack alerted<br><img width="831" height="752" alt="image" src="https://github.com/user-attachments/assets/9b8eaebc-9528-46a2-b083-4c619c93e5c8" />

> 📸 Threat Intelligence<br><img width="821" height="784" alt="image" src="https://github.com/user-attachments/assets/f11cdc53-1bd6-466b-ab24-3229c2d6a299" />

## 🧠 Key Takeaways
* **Assess Before Acting:** Learned that the primary goal of a defensive analyst is to methodically investigate and understand the full scope of an incident rather than hastily eliminating artifacts, which could destroy critical forensic evidence.
* **The Importance of Rapid Containment:** Recognized that once a compromised account is positively identified (e.g., `dave.saunders`), immediate containment through account locking is vital to stop the attacker's progression.
* **Leveraging Threat Intelligence:** Realized that threat intel is not just theoretical; cross-referencing indicators with known adversary groups (like `ShadowFigures`) helps analysts anticipate attacker behavior and close security gaps more effectively.
* **Documentation is Essential:** Understood that a SOC analyst's job isn't finished until the incident report is written. Clear documentation ensures accountability and strengthens future defensive postures.
