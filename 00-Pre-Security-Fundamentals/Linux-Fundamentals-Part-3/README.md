# Lab: Linux Fundamentals Part 3

**Role:** Pre-Security Student / Linux System Administrator Trainee

## 🎯 Objective
To master advanced Linux administration tasks, including system logging inspection, package management, process control, file transfer utilities, and task automation using Cron jobs in an enterprise environment.

## 🚀 Execution Steps
1. **System Logging & Package Management:** 
   * Inspected critical system event logs located within the `/var/log` directory to analyze system behavior and service statuses.
   * Managed software installations, repository updates, and GPG key verifications utilizing the `apt` package manager.
2. **Process Management & Resource Tracking:** 
   * Monitored active system processes and resource utilization using dynamic tools like `top` and static snapshots via `ps`.
   * Controlled process lifecycles by issuing process termination signals (e.g., `SIGTERM` and `SIGKILL`) to handle unresponsive services.
   * Managed process execution states, toggling tasks between the foreground and background.
3. **File Transfer & Task Automation:** 
   * Utilized text editing with `nano` and executed remote file transfers and downloads using `wget` and `scp`.
   * Deployed a lightweight local HTTP web server using Python's built-in `http.server` module for rapid file delivery.
   * Configured scheduled automated tasks and periodic jobs utilizing the `crontab` utility.

## 📊 Results & Evidence
* Successfully managed system processes, configured automated background tasks via Cron, inspected `/var/log` artifacts, and executed remote file transfers using standard Linux CLI utilities.

> 📸 <br><img width="961" height="751" alt="image" src="https://github.com/user-attachments/assets/f7f7df21-f823-4ea5-b1ac-2d53fd60c49b" />

> 📸 <br><img width="965" height="594" alt="image" src="https://github.com/user-attachments/assets/255a9226-3bee-46ec-b059-64ede0841b24" />

## 🧠 Key Takeaways
* **Logs are the Ultimate Source of Truth:** Learned that `/var/log` is the primary repository for forensic analysis and system troubleshooting, providing crucial visibility into system events and failures.
* **Mastering Process Control:** Recognized that knowing how to monitor (`top`/`ps`) and terminate (`kill`/`SIGKILL`) runaway or malicious processes is a mandatory skill for system defense and incident response.
* **Automation Drives Efficiency:** Understood how `crontab` enables administrators and analysts to automate routine maintenance, backup scripts, and log rotations seamlessly in the background.
