# Lab: SOC Metrics and Objectives

**Role:** Junior Security Analyst / Tier 1 SOC Analyst

## 🎯 Objective
To evaluate Security Operations Center (SOC) efficiency and alignment with business goals by measuring core performance indicators across alert triage quality (False Positive/Escalation rates) and time-based incident SLA benchmarks (MTTD, MTTA, and MTTR).

## 🚀 Execution Steps
1. **Triage Quality & Volume Metrics Tracking:** 
   * Examined core triage performance metrics to measure alert handling efficiency and detection engine accuracy.
   * Analyzed key quality indicators, including **Alerts Count** (workload volume), **False Positive Rate** (noise level vs. tuning efficiency), and **Alert Escalation Rate** (ratio of alerts escalated from L1 to L2).
2. **Time-Based Performance & SLA Evaluation:** 
   * Evaluated time-based metrics tied to organizational Service Level Agreements (SLAs) to benchmark the speed of security operations.
   * Tracked the end-to-end timeline of simulated incidents across three vital stages: **Mean Time to Detect (MTTD)**, **Mean Time to Acknowledge (MTTA)**, and **Mean Time to Respond/Remediate (MTTR)**.
3. **Operational Optimization & Cross-Role Alignment:** 
   * Assessed how metrics influence daily SOC workflows, identifying bottlenecks in triage that cause SLA breaches.
   * Established continuous feedback loops between L1 Analysts, L2 Responders, and SOC Engineers to optimize detection rules, lower False Positive rates, and accelerate MTTA/MTTR.

## 📊 Results & Evidence
* Successfully evaluated simulated SOC performance data, mapped alert triage metrics to operational bottlenecks, and analyzed time-based SLA benchmarks to optimize incident response workflows.

> 📸 <br><img width="789" height="637" alt="image" src="https://github.com/user-attachments/assets/a471d628-4b34-4717-b39a-6fa4f9cb4ea3" />

> 📸 Create Workbook to Handle<br><img width="823" height="694" alt="image" src="https://github.com/user-attachments/assets/37940f1f-57b9-40e3-9d9b-5cb2b3afba15" />

> 📸 Improve SIEM Triage Alert<br><img width="816" height="738" alt="image" src="https://github.com/user-attachments/assets/5d75b210-0438-44c6-be01-380c71ac0fa4" />

> 📸 Remediation Noise<br><img width="789" height="637" alt="image" src="https://github.com/user-attachments/assets/cdcf656d-7496-4dfe-add1-d1a97c4f424c" />


## 🧠 Key Takeaways
* **Speed vs. Quality Balance:** Learned that a high-performing SOC must balance speed (Time-based Metrics) with accuracy (Triage Metrics). Reducing **MTTA/MTTR** is useless if the **False Positive Rate** remains so high that critical alerts are overlooked.
* **The Core SLA Benchmarks (MTTD, MTTA, MTTR):**
  * **MTTD (Detect):** Measures how quickly a threat is recognized by security tools after compromise occurs.
  * **MTTA (Acknowledge):** Measures how fast a Tier 1 analyst picks up an alert after it fires.
  * **MTTR (Respond):** Measures the overall time required to contain, remediate, and resolve the incident.
* **Metrics Drive Engineering Improvements:** Understood that high False Positive or Escalation rates are direct indicators for SOC Engineers to refine SIEM detection rules and update L1 workbooks, ensuring continuous operational improvement across the team.
