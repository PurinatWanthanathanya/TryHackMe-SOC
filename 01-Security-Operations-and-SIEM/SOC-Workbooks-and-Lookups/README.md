# Lab: SOC Workbooks and Lookups

**Role:** Junior Security Analyst / Tier 1 SOC Analyst

## 🎯 Objective
To enhance alert triage and incident investigations by leveraging SIEM Workbooks as Standard Operating Procedures (SOPs), utilizing Lookup tables for data enrichment, and cross-referencing asset and identity inventories to accurately map attack paths.

## 🚀 Execution Steps
1. **Data Enrichment via Lookup Tables:** 
   * Integrated external context into security investigations by correlating raw alert logs with internal inventory systems and identity lookups (e.g., HR/employee databases like BambooHR).
   * Utilized Lookup tables to identify the ownership, department, and physical locations associated with suspicious IP addresses, hosts, and user accounts.
2. **Operationalizing SOC Workbooks (SOPs):** 
   * Implemented interactive SIEM Workbooks to standardize the investigative workflow for Level 1 (L1) SOC Analysts.
   * Followed step-by-step workbook playbooks to ensure consistent, repeatable, and methodical triage of security alerts without omitting critical forensic checks.
3. **Asset Mapping & Attack Path Analysis:** 
   * Cross-referenced enriched alert artifacts against enterprise asset inventories and architecture/network diagrams.
   * Mapped adversary movement across the infrastructure to visualize potential attack paths and determine the blast radius of a simulated compromise.

## 📊 Results & Evidence
* Successfully enriched raw SIEM alerts using Identity/Asset Lookup tables and followed standardized SOC Workbooks to systematically triage incidents and map network attack paths.

> 📸 Network Diagrams<br><img width="3560" height="1480" alt="image" src="https://github.com/user-attachments/assets/f8511669-7017-4e95-a507-dff5b753bc66" />
  
> 📸 SOC Workbooks<br><img width="1342" height="690" alt="image" src="https://github.com/user-attachments/assets/a4358b04-381c-4e70-9cba-a7dcc294f80d" />

> 📸 Email analysis<br><img width="786" height="741" alt="image" src="https://github.com/user-attachments/assets/5036df4b-9e24-4e8c-93b6-41ef5feb3ac7" />

> 📸 Powershell analysis<br><img width="786" height="737" alt="image" src="https://github.com/user-attachments/assets/dd7d2d28-8a5f-4a77-90fc-09533e570a0e" />

> 📸 Network analysis<br><img width="801" height="719" alt="image" src="https://github.com/user-attachments/assets/3a8d4166-5bf8-4da4-8272-dbeaae0fb8bc" />


## 🧠 Key Takeaways
* **The Value of Data Enrichment:** Learned that raw alerts alone often lack meaning—enriching logs with Lookup tables (e.g., mapping an IP to a specific user via HR systems) is essential for turning ambiguous telemetry into actionable intelligence.
* **Workbooks as Consistency Drivers:** Recognized that SOC Workbooks act as living Standard Operating Procedures (SOPs). They guide analysts through systematic investigation steps, reducing human error and ensuring uniform quality across Tier 1 triage.
* **Contextualizing Attack Paths:** Understood that combining identity lookups, asset inventories, and network diagrams allows security analysts to see the "bigger picture," enabling faster identification of critical assets and lateral movement during an incident.
