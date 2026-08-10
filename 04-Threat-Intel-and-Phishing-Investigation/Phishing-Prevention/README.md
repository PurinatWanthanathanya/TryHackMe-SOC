# Lab: Phishing Prevention

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To evaluate and implement enterprise-grade email security mechanisms, focusing on domain authentication protocols (SPF, DKIM, DMARC), cryptographic standards (S/MIME), and automated defensive layers (Secure Email Gateways) to actively prevent email spoofing and social engineering attacks.

## 🚀 Execution Steps
1. **Email Authentication & Policy Enforcement:** 
   * Analyzed the triad of domain-level email authentication protocols to prevent sender spoofing:
     * **SPF (Sender Policy Framework):** Verified authorized IP addresses permitted to send emails on behalf of a domain.
     * **DKIM (DomainKeys Identified Mail):** Evaluated cryptographic signatures injected into email headers to ensure message integrity during transit.
     * **DMARC (Domain-based Message Authentication, Reporting, and Conformance):** Examined policy enforcement mechanisms that dictate how receiving mail servers should handle emails failing SPF or DKIM alignment.
2. **Cryptographic Identity & Confidentiality (S/MIME):** 
   * Investigated the deployment of **S/MIME** (Secure/Multipurpose Internet Mail Extensions) to provide robust end-to-end encryption and digital signatures, ensuring the absolute identity of the sender and the confidentiality of the payload.
3. **Enterprise Defensive Infrastructure & Human Firewall:** 
   * Evaluated the role of **Secure Email Gateways (SEGs)** in automating threat prevention through spam filtering, link rewriting, and detonating suspicious attachments within a sandbox environment.
   * Highlighted the importance of user-focused controls, such as appending `[External]` warning banners to inbound communications and deploying periodic Phishing Simulation training to strengthen organizational awareness.

## 📊 Results & Evidence
* Successfully analyzed SPF, DKIM, and DMARC DNS records for alignment, evaluated the integration of S/MIME for digital signatures, and mapped technical gateway controls to prevent malicious email delivery.

> 📸 <br><img width="527" height="264" alt="image" src="https://github.com/user-attachments/assets/5c14bfa7-668c-4f78-be44-a3b4d6cc7a69" />

> 📸 <br><img width="524" height="60" alt="image" src="https://github.com/user-attachments/assets/f9119694-899c-46d3-b835-2ab6e37cb2db" />
> 📸 <br><img width="527" height="254" alt="image" src="https://github.com/user-attachments/assets/7730073c-cb5c-4ebf-85fa-aa210e378324" />

> 📸 <br><img width="527" height="290" alt="image" src="https://github.com/user-attachments/assets/7545122e-1b93-41ad-9b0a-84b2e8c30932" />

> 📸 <br><img width="567" height="235" alt="image" src="https://github.com/user-attachments/assets/bdc5b01a-dfa4-4bc0-974f-6f204359c26b" />

> 📸 <br><img width="526" height="310" alt="image" src="https://github.com/user-attachments/assets/9b724971-32f5-48f9-bd6c-e14b3509b843" />

> 📸 <br><img width="820" height="759" alt="image" src="https://github.com/user-attachments/assets/663f8989-f1dc-42d2-8293-71574398aa6e" />

> 📸 <br><img width="835" height="750" alt="image" src="https://github.com/user-attachments/assets/6b1e5cdb-2f8f-4b94-bfc4-c1630527145e" />

> 📸 <br><img width="811" height="747" alt="image" src="https://github.com/user-attachments/assets/2029096d-26e5-4f39-9abf-e2b172f9b8a2" />

> 📸 <br><img width="833" height="744" alt="image" src="https://github.com/user-attachments/assets/98ca4a3f-2dc9-4225-a25c-f693a0491859" />

## 🧠 Key Takeaways
* **The Holy Trinity of Email Security:** Learned that stopping email spoofing requires a layered approach. **SPF** checks the source, **DKIM** guarantees the message wasn't tampered with, and **DMARC** tells the receiver whether to quarantine or reject the email if those checks fail.
* **S/MIME Provides Ultimate Trust:** Recognized that while DMARC protects the domain, **S/MIME** protects the individual user. It uses public key infrastructure (PKI) to definitively prove *who* wrote the email and ensures no one intercepted it.
* **Defense in Depth:** Understood that technical controls (Sandboxing, Link Rewriting) must be paired with human controls. Even the best Secure Email Gateway cannot stop a 100% targeted zero-day attack, which is why external sender indicators and continuous staff training remain critical final lines of defense.
