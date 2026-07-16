# Lab: SOC L1 Alert Triage

**Role:** Junior Security Analyst

## 🎯 Objective
To apply a systematic triage workflow for evaluating security alerts, determining their validity based on business context, and correctly identifying True Positives and False Positives.[cite: 1]

## 🚀 Execution Steps
1. **Alert Prioritization & Assignment:** 
   * Selected unassigned alerts by prioritizing them from highest severity to lowest (Critical -> Low), and then chronologically from oldest to newest.[cite: 1]
   * Assigned the selected cases to myself and changed the status to "In Progress" to prevent duplicated effort among team members.[cite: 1]
2. **Contextual Investigation:** 
   * Investigated the technical details of the alerts while factoring in the surrounding business context, such as user identity, IPs, and typical behavior.[cite: 1]
   * Evaluated the legitimacy of user activities, such as verifying if code downloads from GitHub were normal because the user belonged to a developer network (VPN/DEVELOPERS), or if an overseas VPN login (from Japan) was actually the CFO on a confirmed travel itinerary.[cite: 1]
3. **Decision & Closure (Verdict):** 
   * Reached a verdict on whether each alert was a real attack (True Positive) or a misclassification (False Positive).[cite: 1]
   * Closed the alerts by writing clear explanatory comments for the decision and updating the status to "Closed", while ensuring that highly severe cases were escalated to Level 2 (L2) analysts.[cite: 1]

## 📊 Results & Evidence
* Successfully processed and closed multiple alerts by analyzing user contexts, correctly distinguishing between normal business activities and actual cyber threats like RDP brute-force attacks and phishing attempts.[cite: 1]

> 📸 WorkFlow Analysis<img width="1010" height="347" alt="image" src="https://github.com/user-attachments/assets/d692d345-9167-46b2-9e75-f791f5d3fef8" />

> 📸 Alert Analysis<img width="1237" height="436" alt="image" src="https://github.com/user-attachments/assets/ea85410a-df18-474a-81e3-81f4ee6f37ee" />

> 📝 **Self-Improvement Note:** 
> I still need to refine my case closure comments to ensure they follow a proper, professional structure. Moving forward, my comments must clearly state: (1) What happened, (2) How it was analyzed, and (3) How it was handled.

> 📸 New Comment:True Positive. Detected a suspicious file with a double extension (e.g., .mp4.exe) indicating malware. The file has been blocked, and the alert is escalated to the L2 team for further investigation. <img width="1224" height="489" alt="image" src="https://github.com/user-attachments/assets/20c86332-829e-49e2-943e-12a9ea9aa0e6" />

> 📸 New Comment:False Positive. The tracked IP address did not look suspicious, and the activity was related to the Zoom platform. Closed the ticket.<img width="1209" height="555" alt="image" src="https://github.com/user-attachments/assets/e50f55da-7ef1-4ad0-abe0-e01e53cf72aa" />

> 📸 New Comment:False Positive. User on trusted VPN/DEVELOPER network was downloading from GitHub. Alert closed.<img width="1232" height="338" alt="image" src="https://github.com/user-attachments/assets/56a73a61-35d5-4988-9413-1fae68e510d1" />

> 📸 Analyzed by the lab<img width="1205" height="339" alt="image" src="https://github.com/user-attachments/assets/27cb0cf1-3379-4b22-abfa-46bc188222ea" />
> 📸 Analyzed by the lab<img width="1206" height="404" alt="image" src="https://github.com/user-attachments/assets/f6d9ffe7-d3b1-4917-ba5a-5a2eaac68c41" />

## 🧠 Key Takeaways
* **Business Context vs. Technical Rules:** Learned that automated rules trigger based on technical conditions, but human analysts are needed to understand the business context.[cite: 1] For example, a massive 5.8 GB data transfer flagged as "Data Exfiltration" was actually just a legitimate video meeting when the destination was identified as `*.zoom.us` (False Positive).[cite: 1]
* **Recognizing True Positives:** Developed an eye for spotting genuine threat patterns.[cite: 1] This included identifying phishing techniques that use double-extensions (e.g., `cats2025.mp4.exe`) and recognizing brute-force attacks on RDP ports featuring an excessively high number of failed logins (e.g., 1,620 attempts).[cite: 1]
* **Structured Triage Workflow:** Mastered a disciplined operational flow: Assign, Investigate, Decide, and Close/Escalate, which is crucial for efficient and organized SOC environments.[cite: 1]
