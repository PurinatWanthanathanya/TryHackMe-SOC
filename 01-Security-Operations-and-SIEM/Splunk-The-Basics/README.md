# Lab: Splunk: The Basics

**Role:** Junior Security Analyst

## 🎯 Objective
To utilize Splunk as a centralized SIEM platform for aggregating, analyzing, and correlating network and host logs, and to develop proficiency in Search Processing Language (SPL) for real-time threat detection.

## 🚀 Execution Steps
1. **Data Ingestion & Management:** 
   * Configured data inputs into the Splunk environment using various ingestion methods, including manual **Uploads** for static files, setting up the **Monitor** option for continuous file/port tracking, and understanding the use of **Forwarders** for remote endpoint collection.
2. **Log Parsing & Formatting:** 
   * Navigated the Search Head interface to inspect raw ingested data.
   * Applied the `spath` command within SPL to properly parse and extract structured data fields from complex JSON log formats, making them highly readable and searchable for analysis.
3. **Querying & Threat Analysis (SPL):** 
   * Constructed targeted SPL queries using logical operators (AND/OR/NOT) to filter specific fields, isolate malicious indicators, and exclude irrelevant network noise.
   * Utilized aggregation commands like `stats count` to group data, identify anomalies (e.g., spikes in specific error codes or failed logins), and track suspicious user activities across the infrastructure.

## 📊 Results & Evidence
* Successfully ingested, parsed, and analyzed raw security logs, transforming them into actionable insights and structured data ready for incident response and dashboard creation.

> 📸 Ingest Data<br><img width="774" height="631" alt="image" src="https://github.com/user-attachments/assets/20830bb9-3372-49cb-9f56-c5d6fa288079" />

> 📸 Splunk Search Head<br><img width="774" height="633" alt="image" src="https://github.com/user-attachments/assets/ea0089e1-dd71-4097-a01d-649605f3edbe" />

## 🧠 Key Takeaways
* **Splunk Architecture:** Gained a solid understanding of Splunk's three core components: the **Forwarder** (collects and forwards data from endpoints), the **Indexer** (parses, organizes, and stores the data), and the **Search Head** (provides the GUI for analysts to execute queries using SPL).
* **Data Ingestion Flexibility:** Learned that Splunk can ingest data through multiple avenues (Upload, Monitor, Forward), making it highly adaptable for both offline forensic analysis and real-time enterprise monitoring.
* **The Power of SPL:** Realized that Search Processing Language (SPL) is an essential tool for a SOC Analyst. Mastering commands like `spath` for parsing JSON structures and `stats` for data aggregation is crucial for efficiently hunting threats within massive datasets.
