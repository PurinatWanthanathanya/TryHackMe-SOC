# Lab: Windows Logging for SOC

**Role:** Junior Security Analyst

## 🎯 Objective
To understand the fundamentals of Windows Event Logs, differentiate critical Event IDs related to authentication and user management, and utilize tools like Event Viewer and Sysmon to monitor endpoint activities and detect malicious behaviors.

## 🚀 Execution Steps
1. **Log Collection & Initial Triage:** 
   * Navigated to the Windows Event Viewer and accessed binary log files (`.EVTX`) located at `C:\Windows\System32\winevt\Logs`.
   * Filtered the Security logs to investigate reported anomalous activities on the host endpoint.
2. **Authentication & User Management Investigation:** 
   * Analyzed Logon Events by filtering for Event ID 4625 (Failed Logon) to identify potential RDP brute-force attacks, followed by Event ID 4624 (Successful Logon, Type 10) to confirm unauthorized access.
   * Investigated user account modifications using the 47xx series (e.g., 4720 for account creation, 4732 for adding a user to the Administrators group) to track privilege escalation and persistence.
3. **Process & Command Execution Tracking:** 
   * Cross-referenced standard logs with Sysmon telemetry (Event ID 1 for Process Creation, Event ID 3 for Network Connections) to track the attacker's footprint and correlate activities using `ProcessId`.
   * Monitored Event ID 1 (Process Creation) and Event ID 3 (Network Connection) for initial malicious execution and external communications.
   * Investigated Event ID 11 (File Creation) and Event ID 13 (Registry Set) to identify newly dropped payloads and unauthorized registry modifications.
   * Analyzed Event ID 22 (DNS Query) to detect attempts to resolve malicious domains or URLs.
   * Inspected the hidden PowerShell History File (`ConsoleHost_history.txt`) to uncover specific malicious commands and scripts executed by the attacker that might have bypassed standard logging.

## 📊 Results & Evidence
* Successfully mapped a complete attack chain on a Windows endpoint, from the initial brute-force entry and privilege escalation to the execution of malicious scripts via PowerShell.

> 📸 EventViewer<br><img width="670" height="495" alt="image" src="https://github.com/user-attachments/assets/c3efeadb-d3ba-447e-8148-ca64d3fc4854" />

> 📸 Sysmon<br><img width="674" height="491" alt="image" src="https://github.com/user-attachments/assets/249130e8-f31d-42c4-b030-cd4b37ce3213" />

> 📸 PowerShell History File<br><img width="671" height="545" alt="image" src="https://github.com/user-attachments/assets/592077e5-60ec-49a4-b548-4d80403934db" />

## 🧠 Key Takeaways
* **Authentication & Logon IDs:** Recognized the critical importance of monitoring Event IDs 4624 and 4625, and learned how to use unique Logon IDs to correlate all activities within a specific compromised session.
* **Tracking Malicious Account Activity:** Realized that attackers frequently manipulate accounts to maintain access. Monitoring the 47xx event series (e.g., 4720, 4722, 4732) is essential for spotting unauthorized privilege escalation.
* **Sysmon vs. Standard Logging:** Discovered that Sysmon provides significantly deeper forensic telemetry (such as parent-child process relationships, file hashes, and DNS queries) compared to default Windows logging.
* **Uncovering Hidden Commands:** Learned that standard Sysmon logging might miss specific sub-commands in PowerShell, making the `ConsoleHost_history.txt` file a vital artifact for revealing the exact commands used in "fileless" attacks.
