# Lab: Cyber Kill Chain

**Role:** Junior Security Analyst / SOC Analyst Trainee

## 🎯 Objective
To apply the Lockheed Martin Cyber Kill Chain framework to analyze end-to-end adversary intrusion lifecycles, map security telemetry across all seven attack phases, and deploy targeted defensive controls to break the intrusion chain before adversaries achieve their objectives.

## 🚀 Execution Steps
1. **Adversary Lifecycle Mapping:** 
   * Deconstructed sophisticated cyber attacks into the seven sequential stages of the Cyber Kill Chain: **Reconnaissance**, **Weaponization**, **Delivery**, **Exploitation**, **Installation**, **Command and Control (C2)**, and **Actions on Objectives**.
   * Analyzed external attacker behaviors during Pre-Att&ck stages (Reconnaissance and Weaponization) to identify threat actor preparations and payload packaging.
2. **Delivery & Exploitation Investigation:** 
   * Examined common attack vectors utilized during the **Delivery** phase (e.g., targeted phishing emails, watering hole websites, USB baiting).
   * Investigated the **Exploitation** and **Installation** phases to identify how adversaries leverage software vulnerabilities or human error to execute code and establish persistence on target systems.
3. **C2 Analysis & Breaking the Chain:** 
   * Investigated **Command and Control (C2)** channels utilized by adversaries to issue remote instructions and manipulate infected endpoints.
   * Formulated defensive strategies and mitigation points across each stage of the lifecycle, demonstrating that successfully disrupting any single link in the kill chain halts the attack before **Actions on Objectives** (such as data exfiltration or encryption) occur.

## 📊 Results & Evidence
* Successfully mapped simulated attack scenarios against the seven stages of the Cyber Kill Chain and identified strategic defensive controls required to disrupt adversary progress across network and host layers.

> 📸 <br><img width="790" height="741" alt="image" src="https://github.com/user-attachments/assets/d9b28a0c-3bfa-4a51-8125-0bc71698fe7a" />

## 🧠 Key Takeaways
* **The Power of "Breaking the Chain":** Learned that defenders do not need to prevent an attack at stage one; disrupting the intrusion at *any* stage (such as blocking C2 traffic at the firewall or catching persistence mechanisms via EDR) completely neutralizes the adversary's attack.
* **Structuring Threat Intelligence:** Recognized that the Cyber Kill Chain provides a shared operational language for SOC teams to categorize incidents, assess how far an intruder has progressed, and align appropriate response actions.
* **Proactive vs. Reactive Defense:** Understood that mapping historical incidents to the Kill Chain reveals organizational blind spots, allowing engineering teams to fortify early-stage defenses (e.g., email filtering for Delivery, patching for Exploitation) rather than reacting only during the Actions on Objectives stage.
