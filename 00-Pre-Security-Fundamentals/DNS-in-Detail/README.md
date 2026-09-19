# Lab: DNS in Detail

**Role:** Pre-Security Student / Network Infrastructure Trainee

## 🎯 Objective
To deconstruct the architecture of the Domain Name System (DNS), analyze the hierarchical domain tree (TLDs, subdomains), examine critical DNS record types, and trace the step-by-step recursive query resolution workflow.

## 🚀 Execution Steps
1. **Domain Name Hierarchy & Structural Constraints:** 
   * Analyzed the distributed DNS hierarchical namespace translating human-friendly domain names into machine-routable IP addresses.
   * Examined structural elements, including **Top-Level Domains (TLDs)** categorized into generic TLDs (gTLDs) and country-code TLDs (ccTLDs), along with subdomains and the overall 253-character domain length restriction.
2. **DNS Record Types & Functional Analysis:** 
   * Investigated primary resource record types utilized for network routing and identity verification:
     * **A & AAAA Records:** Mapping domain names to IPv4 and IPv6 addresses respectively.
     * **CNAME Records:** Creating canonical alias mappings linking one domain name to another.
     * **MX Records:** Routing email traffic to destination mail exchange servers.
     * **TXT Records:** Storing arbitrary text, utilized for verification protocols (SPF, DKIM, domain ownership).
3. **Recursive Resolution Workflow & Caching:** 
   * Traced the sequential stages of the DNS lookup lifecycle:
     1. Local cache inspection (browser and OS DNS cache).
     2. Query forwarding to the **Recursive DNS Resolver**.
     3. Referral through the **Root Name Servers** (`.`).
     4. Redirection through **TLD Name Servers** (e.g., `.com`, `.net`).
     5. Querying the **Authoritative Name Server** to extract the target record.
   * Evaluated the role of **Time To Live (TTL)** values governing record caching lifetimes and consistency across endpoints.

## 📊 Results & Evidence
* Successfully mapped DNS domain tree hierarchies, differentiated record structures across A, CNAME, MX, and TXT types, and traced recursive lookup query chains to authoritative endpoints.

> 📸 <img width="1140" height="800" alt="image" src="https://github.com/user-attachments/assets/c92c7d82-b462-4443-87b8-abffa19426c5" />

> 📸 <img width="933" height="577" alt="image" src="https://github.com/user-attachments/assets/4810a5a1-eec8-4862-9f93-4dd77cacb23d" />

## 🧠 Key Takeaways
* **The Phonebook of the Internet:** Learned that DNS abstraction is foundational to web communications; understanding the hierarchical resolution chain is essential for troubleshooting connectivity and analyzing network traffic.
* **DNS as an Attack Vector:** Recognized that because DNS was not originally built with security in mind, monitoring DNS queries (e.g., high volumes of TXT records or abnormal subdomain queries) is critical for identifying DNS tunneling and data exfiltration.
* **TTL Controls Propagation:** Understood that Time To Live (TTL) values define how long resolvers cache DNS responses, directly impacting how quickly security teams can sinkhole malicious domains or update server infrastructure.
