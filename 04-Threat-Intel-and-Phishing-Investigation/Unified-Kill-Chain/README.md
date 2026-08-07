# Lab: Unified Kill Chain

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To apply the Unified Kill Chain (UKC) framework to analyze sophisticated modern cyber attacks, evaluate adversary Tactics, Techniques, and Procedures (TTPs) across 18 tactical phases grouped into three overarching stages (In, Through, and Out), and formulate defense-in-depth strategies.

## 🚀 Execution Steps
1. **Adversary Intrusion Phase Mapping (In - Initial Access):** 
   * Examined the initial entry stage (**"In"**), mapping how adversaries conduct external reconnaissance, weaponize payloads, and exploit perimeter or human vulnerabilities to establish initial footholds within an enterprise.
   * Investigated early-stage tactical phases including Social Engineering, Exploitation, and Persistence mechanisms used to survive system reboots.
2. **Network Propagation & Pivoting Analysis (Through - Network Propagation):** 
   * Tracked post-exploitation activities within the internal network (**"Through"**), analyzing how threat actors escalate privileges, evade detection, and execute credential dumping.
   * Mapped internal reconnaissance, lateral movement, and pivoting techniques as adversaries traverse from initial endpoints to critical internal servers and domain controllers.
3. **Actions on Objectives Investigation (Out - Action on Objectives):** 
   * Investigated the final phase of the attack lifecycle (**"Out"**), where threat actors leverage Command and Control (C2) infrastructure to achieve their ultimate operational goals.
   * Analyzed impact techniques such as data exfiltration, system encryption (ransomware deployment), and infrastructure denial-of-service, establishing multi-layered defensive controls across all 18 tactical phases to disrupt attack chains.

## 📊 Results & Evidence
* Successfully mapped end-to-end simulated Advanced Persistent Threat (APT) attack scenarios across the 18 tactical phases of the Unified Kill Chain, aligning SOC detection capabilities to the In, Through, and Out phases.

> 📸 Unified Kill Chain<br><img width="1230" height="794" alt="image" src="https://github.com/user-attachments/assets/052e1285-8b8b-4ae2-acda-12e2df209ef6" />

> 📸 Phase In<br><img width="1201" height="844" alt="image" src="https://github.com/user-attachments/assets/0a2b48eb-30a9-40b4-b700-34a0ee439a5f" />

> 📸 Phase Through<br><img width="1115" height="823" alt="image" src="https://github.com/user-attachments/assets/9e3327a4-394b-42f1-83be-3e0ab61c395e" />

> 📸 Phase Out<br><img width="1197" height="771" alt="image" src="https://github.com/user-attachments/assets/3e41c744-3d38-4d28-b2bd-06b1886170ea" />

## 🧠 Key Takeaways
* **Evolution of the Kill Chain:** Learned that traditional linear kill chains often fall short against modern Advanced Persistent Threats (APTs). The **Unified Kill Chain** bridges this gap by merging the conceptual lifecycle of Lockheed Martin with the tactical depth of **MITRE ATT&CK**.
* **The "In, Through, Out" Paradigm:**
  * **In (Initial Access):** Gaining a foothold via phishing, vulnerability exploitation, or compromised credentials.
  * **Through (Network Propagation):** Expanding reach via privilege escalation, credential harvesting, and lateral movement.
  * **Out (Action on Objectives):** Achieving the primary mission—whether data theft, extortion, or sabotage.
* **Granular Defensive Posture:** Understood that dividing an attack into 18 tactical phases allows SOC analysts to pinpoint exact defensive blind spots within the network, ensuring robust detection controls are present during internal propagation ("Through"), not just at the perimeter ("In").
