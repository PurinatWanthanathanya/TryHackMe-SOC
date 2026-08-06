# Lab: Pyramid of Pain

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To apply the Pyramid of Pain conceptual model within Threat Intelligence and SOC workflows, evaluate the effectiveness of Indicators of Compromise (IOCs) across six hierarchical tiers, and elevate threat detection from simple artifact blocking to disrupting adversary Tactics, Techniques, and Procedures (TTPs).

## 🚀 Execution Steps
1. **IOC Classification across Hierarchical Tiers:** 
   * Categorized Indicators of Compromise into the six levels of the Pyramid of Pain: **Hash Values** (Trivial), **IP Addresses** (Easy), **Domain Names** (Simple), **Network/Host Artifacts** (Annoying), **Tools** (Challenging), and **TTPs** (Tough).
   * Evaluated why traditional signature-based defenses relying solely on low-level indicators (Hashes, IPs, Domains) provide temporary protection due to the low effort required for adversaries to alter them.
2. **Artifact Analysis & Tool Detection:** 
   * Investigated mid-level **Network and Host Artifacts** (e.g., specific user-agent strings, registry keys, dropped files) to understand how detecting these indicators causes operational irritation to attackers.
   * Analyzed adversary **Tools** (e.g., custom C2 frameworks, malware utilities) to implement rules that neutralize entire toolsets rather than individual payloads.
3. **Behavioral TTP Hunting & Adversary Disruption:** 
   * Mapped security alerts and telemetry to high-level **Tactics, Techniques, and Procedures (TTPs)** leveraging the MITRE ATT&CK framework.
   * Constructed behavioral detection rules targeting adversary methodology, successfully inflicting maximum "pain" by forcing attackers to abandon their core attack strategies.

## 📊 Results & Evidence
* Successfully classified IOCs across the Pyramid of Pain tiers, evaluated the operational impact of blocking threat artifacts, and designed behavioral detection approaches targeting adversary TTPs.

> 📸 <br><img width="994" height="321" alt="image" src="https://github.com/user-attachments/assets/90f80f3e-ba3f-49ce-b675-43318caa7be6" />

> 📸 <br><img width="831" height="654" alt="image" src="https://github.com/user-attachments/assets/9e5f2e02-add5-4700-a915-5e8ed7d289c9" />


## 🧠 Key Takeaways
* **The Hierarchy of Adversary Pain:** Learned that not all IOCs are created equal. Blocking **Hash Values**, **IPs**, or **Domains** only inconveniences attackers for minutes, whereas detecting **Tools** and **TTPs** undermines their fundamental capabilities and training.
* **Moving Beyond Whack-a-Mole:** Recognized that focusing SOC resources solely on low-level indicators leads to alert fatigue. Sustainable defense requires moving up the pyramid to detect *how* an attacker behaves rather than *what* specific tools or IPs they use today.
* **TTPs as the Ultimate Target:** Understood that hunting for **Tactics, Techniques, and Procedures (TTPs)**—such as specific PowerShell downgrade attacks or credential dumping patterns—provides resilient, long-term security posture improvements across the enterprise.
