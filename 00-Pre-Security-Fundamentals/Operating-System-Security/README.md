# Lab: Operating System Security

**Role:** Pre-Security Student / IT Fundamentals Trainee

## 🎯 Objective
To understand core operating system security principles based on the CIA Triad, identify common system vulnerabilities (such as improper file permissions and weak authentication), and perform basic system investigations across Linux and Windows environments.

## 🚀 Execution Steps
1. **Core Security Principles (CIA Triad):** 
   * Analyzed the foundational concepts of information security: **Confidentiality** (preventing unauthorized access), **Integrity** (preventing unauthorized modification), and **Availability** (ensuring data is accessible when needed).
   * Evaluated how common operating system misconfigurations, such as weak user passwords and improper file permissions, directly compromise the CIA triad.
2. **Malware Threat Analysis:** 
   * Investigated the behavioral characteristics of malicious software, specifically focusing on **Trojans** and **Ransomware**, and analyzed their operational impact on system integrity and data availability.
3. **Cross-Platform Investigation & Privilege Management:** 
   * **Linux Environment:** Utilized native command-line utilities (e.g., `ssh` for secure remote access, `whoami` to verify identity, and `history` to review past command execution) to investigate system activities. Examined the necessity of privilege escalation to transition from a standard user to the `root` account.
   * **Windows Environment:** Conducted practical incident response tasks, including basic forensic analysis, identifying active malware payloads, and verifying data compliance policies.

## 📊 Results & Evidence
* Successfully applied the CIA triad to evaluate system vulnerabilities, identified malicious software behaviors, and navigated both Linux and Windows operating systems to investigate user activities and privilege levels.

> 📸 <br><img width="1140" height="800" alt="image" src="https://github.com/user-attachments/assets/8d827709-645f-466f-9525-6a4121527bd3" />

> 📸 <br><img width="543" height="372" alt="image" src="https://github.com/user-attachments/assets/bf6365b0-cb99-473a-827a-005b93649848" />

## 🧠 Key Takeaways
* **The CIA Triad is the North Star:** Learned that every defensive measure implemented on an operating system ultimately traces back to protecting the Confidentiality, Integrity, or Availability of the system's data.
* **Permissions are Paramount:** Recognized that improper file permissions and weak passwords are the primary enablers for unauthorized privilege escalation, allowing attackers to gain `root` or `Administrator` access.
* **Visibility through Logs and History:** Understood the importance of built-in OS utilities. Tools like the `history` command in Linux are invaluable during initial incident response to reconstruct an attacker's timeline and identify malicious actions.
