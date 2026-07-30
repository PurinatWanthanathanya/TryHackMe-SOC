# Lab: IP and Domain Threat Intel

**Role:** Junior Security Analyst

## 🎯 Objective
To apply the core SOC analyst workflow of "Verify, Enrich, and Decide" by utilizing Open-Source Intelligence (OSINT) and threat intelligence tools to investigate suspicious IP addresses, domains, and network infrastructure.

## 🚀 Execution Steps
1. **Domain Enrichment & WHOIS Analysis:** 
   * Conducted WHOIS and RDAP lookups to inspect domain registration details, focusing on domain age, registrar information, and registrant metadata.
   * Investigated domain structures and DNS records to identify typosquatting attempts and newly registered domains (NRDs) frequently used in phishing campaigns.
2. **IP Address & Infrastructure Profiling:** 
   * Performed IP enrichment using tools like AbuseIPDB to check historical abuse reputation, geolocation, and Autonomous System Number (ASN) ownership.
   * Examined exposed network services and inspected TLS/SSL certificates to identify suspicious infrastructure configurations, such as untrusted self-signed certificates used by command-and-control (C2) servers.
3. **Contextual Triage & Decision Making:** 
   * Evaluated IP addresses for commercial VPN or proxy usage during alert triage to distinguish between anonymized attackers and legitimate user activity.
   * Synthesized all enriched data to reach a definitive verdict ("Verify, Enrich, and Decide") on whether the investigated IOCs (Indicators of Compromise) were malicious.

## 📊 Results & Evidence
* Successfully enriched suspicious IP addresses and domain names, uncovering malicious typosquatting infrastructure and identifying self-signed TLS certificates associated with attack servers.

> 📸 <br><img width="401" height="468" alt="image" src="https://github.com/user-attachments/assets/2b9e301c-997b-46b7-b51c-24f5056da3b8" />

> 📸 <img width="2339" height="1653" alt="tls" src="https://github.com/user-attachments/assets/983ec835-ad38-4701-a761-31b9dbf93e70" />

## 🧠 Key Takeaways
* **The 'Verify, Enrich, Decide' Workflow:** Mastered the foundational methodology of a SOC Analyst. Never make a decision based on an alert alone; always verify the artifact, enrich it with external threat intelligence, and then make an informed decision.
* **Domain Age & Typosquatting:** Learned that newly registered domains (NRDs) and domains that closely mimic legitimate brand names (typosquatting) are prime indicators of malicious intent and require immediate scrutiny.
* **Exposed Services & TLS Certificates:** Realized that inspecting TLS/SSL certificate details (e.g., self-signed certificates or mismatched Common Names) is a powerful technique for uncovering hidden C2 infrastructure.
* **Nuances of VPN Detection:** Recognized that while commercial VPN usage warrants close attention during an investigation, the absence of a VPN does not automatically rule out malicious activity—context and behavioral patterns are key.
