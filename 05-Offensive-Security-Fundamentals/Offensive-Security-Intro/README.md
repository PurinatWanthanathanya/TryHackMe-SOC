# Lab: Offensive Security Intro

**Role:** Junior Security Analyst / Pentester Trainee

## 🎯 Objective
To understand the fundamentals of offensive security methodologies, demonstrate why "Security through Obscurity" fails, and utilize web directory scanning tools to uncover hidden assets and unauthenticated web endpoints.

## 🚀 Execution Steps
1. **Offensive vs. Defensive Scope Alignment:** 
   * Examined the differences between offensive security (proactive attack simulation to discover vulnerabilities) and defensive security (monitoring, detection, and mitigation).
   * Evaluated standard penetration testing phases, focusing on reconnaissance and enumeration against web application environments.
2. **Web Directory Enumeration:** 
   * Employed directory-bruteforcing tools (`dirb`) to actively scan the target web application for hidden paths and sensitive endpoints that were not publicly linked.
   * Uncovered obscure administrative and financial management pages that lacked proper access control and authentication mechanisms.
3. **Vulnerability Exploitation & Verification:** 
   * Accessed the exposed web endpoints to test for authorization flaws and business logic vulnerabilities.
   * Investigated the simulated banking interface, successfully identifying confidential data (Bank Account Number `8881`).
   * Executed an unauthorized fund transfer to verify the flaw, successfully triggering the `BANK HACKED` confirmation pop-up.

## 📊 Results & Evidence
* Successfully enumerated hidden web directories using `dirb` and exploited an unauthenticated endpoint to compromise sensitive financial data within the simulated banking application.

> 📸 <img width="840" height="708" alt="image" src="https://github.com/user-attachments/assets/756d9dd0-b6e4-4c88-90c0-d29207ae1b6c" />

> 📸 <img width="676" height="592" alt="image" src="https://github.com/user-attachments/assets/b1416a55-04dc-41f1-a5f3-b195ad3eaed6" />

## 🧠 Key Takeaways
* **Security through Obscurity is Dead:** Demonstrated firsthand that simply hiding a web page URL or relying on unguessable directory names does not protect an application. Automated scanners like `dirb` will easily discover unlinked paths.
* **The Necessity of Robust Authentication:** Recognized that critical endpoints and sensitive actions must always be protected by strong user authentication and access controls, rather than assuming an attacker won't find the page.
* **Thinking Like an Attacker (Offensive Mindset):** Learned that understanding offensive techniques is crucial for a Defensive/SOC Analyst. Knowing how adversaries perform enumeration allows blue teams to better monitor scanning activities and secure exposed attack surfaces.
