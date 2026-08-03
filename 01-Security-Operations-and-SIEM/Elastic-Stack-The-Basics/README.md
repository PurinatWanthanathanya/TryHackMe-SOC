# Lab: Elastic Stack: The Basics

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To understand the architecture and ingestion pipeline of the Elastic (ELK) Stack, master log navigation using the Kibana Discover tab, and apply Kibana Query Language (KQL) to investigate security anomalies and failed authentication events.

## 🚀 Execution Steps
1. **ELK Architecture & Data Pipeline Analysis:** 
   * Examined the core components of the Elastic Stack pipeline: **Beats** (lightweight agents collecting endpoint telemetry), **Logstash** (parsing, filtering, and normalizing logs), **Elasticsearch** (indexing and storage engine), and **Kibana** (visualization and SOC investigation interface).
2. **Log Navigation & Filtering in Kibana (Discover Tab):** 
   * Navigated enterprise security logs using the Kibana **Discover** interface, configuring time ranges and index patterns to isolate specific investigation periods.
   * Applied field-level filtering and customized index columns (e.g., `UserName`, `Source_ip`, `Event.Action`) to streamline the visualization of log telemetry.
3. **Threat Hunting via KQL (Kibana Query Language):** 
   * Constructed targeted **KQL queries** to investigate simulated security incidents across network and authentication logs.
   * Filtered VPN connection telemetry and identified anomalies, specifically isolating unauthorized activities and repetitive failed authentication attempts linked to specific user accounts (e.g., `Manal`).

## 📊 Results & Evidence
* Successfully mapped the ELK data pipeline, navigated indexed logs using Kibana, and executed KQL queries to investigate suspicious VPN telemetry and identify failed login attempts.

> 📸 <br><img width="842" height="732" alt="image" src="https://github.com/user-attachments/assets/efe111dc-01e9-49b9-9878-78acbd3c1763" />

> 📸 <br><img width="826" height="752" alt="image" src="https://github.com/user-attachments/assets/2b892626-f439-47a2-ae46-92455e0bffd0" />

> 📸 <br><img width="824" height="640" alt="image" src="https://github.com/user-attachments/assets/67a83806-01bf-4b8e-9e85-65093390c9a5" />

> 📸 <br><img width="829" height="628" alt="image" src="https://github.com/user-attachments/assets/a1aad248-b741-43be-a2b8-a474f50794c3" />

> 📸 <br><img width="833" height="661" alt="image" src="https://github.com/user-attachments/assets/93445a32-8527-4508-bcb5-9e3f9defded7" />

## 🧠 Key Takeaways
* **The ELK Data Pipeline:** Learned how logs transform into actionable security intelligence—telemetry collected by **Beats** is normalized by **Logstash**, indexed for lightning-fast searches by **Elasticsearch**, and visualized for Blue Teams in **Kibana**.
* **Mastering KQL for Speed:** Recognized that proficiency in **Kibana Query Language (KQL)** is essential for tier-one triage; filtering by exact fields (e.g., `user.name: "Manal" AND event.action: "login_failed"`) dramatically cuts down investigation time.
* **Customizing the Discover Tab:** Understood that adjusting column layouts and time windows in Kibana prevents analyst fatigue by stripping away irrelevant JSON noise and highlighting only critical forensic indicators.
