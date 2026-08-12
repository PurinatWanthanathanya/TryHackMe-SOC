# Lab: Packets & Frames

**Role:** Pre-Security Student / Network Security Trainee

## 🎯 Objective
To deconstruct the structural differences between network packets and frames, evaluate the behavioral characteristics of TCP and UDP transport protocols, and identify critical standard service ports utilized in enterprise network communications.

## 🚀 Execution Steps
1. **Data Encapsulation Analysis (Packets vs. Frames):** 
   * Differentiated between data units across the OSI model. Analyzed **Packets** at the Network Layer (Layer 3), identifying crucial components such as logical IP headers and data payloads.
   * Investigated how packets are encapsulated into **Frames** at the Data Link Layer (Layer 2), appending hardware-specific MAC addresses for local node-to-node delivery.
2. **Transport Protocol Evaluation (TCP vs. UDP):** 
   * Evaluated the fundamental mechanics of the **Transmission Control Protocol (TCP)**, focusing on its connection-oriented nature and the reliability guaranteed by the **Three-Way Handshake** synchronization process.
   * Contrasted TCP with the **User Datagram Protocol (UDP)**, analyzing its stateless, connectionless architecture prioritized for high-speed transmission with minimal overhead.
3. **Service Port Identification:** 
   * Mapped well-known network services to their designated port numbers, establishing a foundational understanding of connection endpoints.
   * Specifically identified critical enterprise ports, including **FTP (Port 21)** for file transfers, **SSH (Port 22)** for secure remote administration, and **HTTPS (Port 443)** for encrypted web traffic.

## 📊 Results & Evidence
* Successfully distinguished between Layer 2 and Layer 3 data structures, evaluated protocol reliability versus transmission speed, and mapped critical service ports utilized for network enumeration.

> 📸 TCP<br><img width="981" height="949" alt="image" src="https://github.com/user-attachments/assets/b5011fbf-c886-4c71-8f12-26612f4c1159" />
> 📸 <br><img width="981" height="949" alt="image" src="https://github.com/user-attachments/assets/ddc24bdf-94fb-434a-b1f1-58b54ce649c1" />

> 📸 UDP<br><img width="981" height="949" alt="image" src="https://github.com/user-attachments/assets/76aac754-783d-4f0d-8186-087e051fc681" />

## 🧠 Key Takeaways
* **Layers Dictate the Terminology:** Learned that data dynamically changes its name based on its location in the OSI stack. A *Packet* navigates logical networks via IP addresses, but once it needs to move across physical hardware, it is wrapped in a *Frame* using MAC addresses.
* **Reliability vs. Speed:** Recognized the strategic trade-offs in transport protocols. TCP's Three-Way Handshake is mandatory for secure, reliable communications (like web browsing or SSH), whereas UDP is chosen when speed is critical and minor packet loss is acceptable (like video streaming or DNS queries).
* **Ports are the Network's Doors:** Understood that standard ports (21, 22, 443) act as designated entry points for specific services. Knowing these ports is a fundamental requirement for SOC analysts to monitor authorized traffic and detect malicious scanning activities.
