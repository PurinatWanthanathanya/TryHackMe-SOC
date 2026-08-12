# Lab: OSI Model

**Role:** Pre-Security Student / Network Fundamentals Trainee

## 🎯 Objective
To understand the Open Systems Interconnection (OSI) Model as the universal framework for network communication, analyze the specific functions of its seven layers, and comprehend the data encapsulation process across diverse networking environments.

## 🚀 Execution Steps
1. **Framework & Interoperability Analysis:** 
   * Examined the OSI Model as a standardized seven-layer architectural framework designed to ensure seamless interoperability and communication between diverse hardware devices and vendor ecosystems.
2. **Layer-by-Layer Functional Deconstruction:** 
   * **Layer 7 (Application):** Analyzed the user-facing layer interfacing directly with applications via the Graphical User Interface (GUI).
   * **Layer 6 (Presentation):** Investigated data formatting, syntax translation, and cryptographic encryption processes.
   * **Layer 5 (Session):** Monitored the establishment, management, and termination of communication sessions between endpoints.
   * **Layer 4 (Transport):** Evaluated end-to-end data delivery mechanisms, focusing on reliable (TCP) versus best-effort (UDP) transmission protocols.
   * **Layer 3 (Network):** Analyzed logical addressing (IP addresses) and routing methodologies utilized to navigate data across multiple networks.
   * **Layer 2 (Data Link):** Investigated physical hardware addressing utilizing MAC addresses for local node-to-node frame delivery.
   * **Layer 1 (Physical):** Examined the transmission and reception of raw binary data bits over physical mediums (e.g., copper cabling, fiber optics).
3. **Data Encapsulation Tracking:** 
   * Traced the flow of data originating from the Application layer down to the Physical layer.
   * Analyzed the **Encapsulation** process, observing how specific protocol headers and control information are systematically appended to the data payload at each successive layer before physical transmission.

## 📊 Results & Evidence
* Successfully mapped the seven layers of the OSI model, differentiated between logical (IP) and physical (MAC) addressing, and tracked the encapsulation lifecycle of network traffic.

> 📸 <br><img width="1077" height="800" alt="image" src="https://github.com/user-attachments/assets/03adb492-3fa7-4820-9c60-4512cd0d5a95" />

## 🧠 Key Takeaways
* **The Universal Language of Networking:** Learned that the OSI Model is the foundational concept that allows a Windows machine, an Apple smartphone, and a Cisco router to communicate flawlessly by adhering to the same structured rules.
* **Troubleshooting by the Layers:** Recognized that SOC analysts and network engineers use the OSI model as a systematic troubleshooting tool (e.g., checking Layer 1 physical cables before investigating Layer 3 routing issues).
* **Encapsulation is Key:** Understood that as data travels down the stack, it is continuously wrapped in new headers (Encapsulation) containing vital routing and delivery instructions, which are then stripped away (Decapsulation) upon reaching the destination.
