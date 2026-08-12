# Lab: Windows CLI Basics

**Role:** Pre-Security Student / IT Fundamentals Trainee

## 🎯 Objective
To master essential Windows Command Line Interface (CLI) operations, including system navigation, configuration enumeration, and network inspection, while recognizing the strategic advantages of utilizing the CLI over a Graphical User Interface (GUI) for cybersecurity tasks.

## 🚀 Execution Steps
1. **Directory Navigation & File Inspection:** 
   * Navigated the Windows file system efficiently without relying on Windows Explorer by utilizing fundamental commands such as `cd` (change directory).
   * Executed `dir` to list directory contents and leveraged the `dir /s` switch to recursively search through subdirectories, locating specific target files deeply embedded within the file system.
2. **System Profiling & Enumeration:** 
   * Conducted initial privilege and identity verification using the `whoami` command.
   * Retrieved critical host information by executing `hostname` and utilized `systeminfo` to extract a comprehensive overview of the operating system configuration, hardware details, and applied hotfixes.
3. **Network Configuration Analysis:** 
   * Inspected network adapter configurations and connectivity details by executing the `ipconfig` command, retrieving essential metrics such as the assigned IPv4 address, subnet mask, and default gateway.

## 📊 Results & Evidence
* Successfully navigated the Windows directory structure via the terminal, extracted critical system and hardware configurations, and verified network adapter details using native CLI tools.

> 📸 <br><img width="822" height="751" alt="image" src="https://github.com/user-attachments/assets/c21b4540-65b6-4eb5-a67d-e8d66544bc1c" />

> 📸 <br><img width="822" height="737" alt="image" src="https://github.com/user-attachments/assets/fb2c29a2-fd6f-4a77-91f7-94fec4a921af" />

## 🧠 Key Takeaways
* **The CLI Advantage:** Learned that command-line tools provide superior speed, precision, and automation capabilities compared to traditional graphical interfaces, especially when managing or querying large amounts of data.
* **Deep System Visibility:** Recognized that mastering CLI fundamentals enables much deeper visibility into the underlying operating system—a critical requirement for effective system administration and security monitoring.
* **Core Triage Skills:** Understood that commands like `systeminfo` and `ipconfig` are not just for troubleshooting; they are the exact commands a SOC Analyst or an Incident Responder uses during the initial triage of a potentially compromised Windows endpoint.
