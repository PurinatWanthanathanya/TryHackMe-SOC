# Lab: Intro to LAN

**Role:** Pre-Security Student / Network Infrastructure Trainee

## 🎯 Objective
To understand the architecture and operational mechanics of Local Area Networks (LAN), evaluate network topologies, analyze the core functions of switches and routers, and deconstruct dynamic addressing (DHCP DORA) and address resolution (ARP) workflows.

## 🚀 Execution Steps
1. **Network Topology Architecture Analysis:** 
   * Evaluated physical and logical network layouts, comparing the trade-offs of **Star**, **Bus**, and **Ring** topologies regarding implementation costs, single points of failure, scalability, and maintenance complexity.
2. **Infrastructure Hardware & Subnetting:** 
   * Investigated foundational network hardware roles:
     * **Switches:** Forwarding traffic locally within broadcast domains using MAC address tables.
     * **Routers:** Routing packets between distinct networks using IP routing tables.
   * Analyzed how **Subnetting** divides larger networks into isolated segments, enhancing network performance and security containment.
3. **Address Resolution & Dynamic Configuration Protocols:** 
   * Traced the **Address Resolution Protocol (ARP)** workflow, mapping IP addresses to physical MAC addresses for local frame delivery.
   * Deconstructed the **DHCP** four-step dynamic IP allocation process (**DORA**):
     * **Discover:** Client broadcasts to find available DHCP servers.
     * **Offer:** Server offers an available IP address configuration.
     * **Request:** Client formally requests the offered configuration.
     * **Acknowledge (ACK):** Server confirms the lease agreement.

## 📊 Results & Evidence
* Successfully mapped LAN physical and logical topologies, analyzed local packet forwarding versus routing, and traced ARP resolution and DHCP DORA communication exchanges.

> 📸<img width="908" height="801" alt="image" src="https://github.com/user-attachments/assets/2b20f3d4-66f7-41bf-8381-235491647f90" />

> 📸 ARP<br><img width="823" height="864" alt="image" src="https://github.com/user-attachments/assets/5f53256c-94cb-4ea1-9a89-64cc1f30d6a6" />

> 📸 DHCP<br><img width="636" height="870" alt="image" src="https://github.com/user-attachments/assets/e39c5a94-e44b-41cc-8680-84ebdb5abca6" />


## 🧠 Key Takeaways
* **Star Topology as Standard:** Learned why modern enterprise LANs rely almost exclusively on Star topologies connected via central switches—a failure on one endpoint does not compromise the entire network segment.
* **DORA is Fundamental:** Understood the sequential 4-step DHCP handshake (Discover, Offer, Request, ACK) essential for troubleshooting connectivity failures and detecting rogue DHCP servers on a network.
* **ARP as the LAN Bridge:** Recognized that ARP is critical for Layer 2 to Layer 3 translation, but its lack of native authentication also makes it inherently susceptible to ARP spoofing and poisoning attacks.
