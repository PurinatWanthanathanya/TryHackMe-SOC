# Lab: What is Networking?

**Role:** Pre-Security Student / Network Fundamentals Trainee

## 🎯 Objective
To understand the foundational architecture of computer networks, explore the historical evolution of the internet, analyze network addressing mechanisms (IPv4, IPv6, and MAC addresses), and utilize diagnostic utilities like ping to evaluate end-to-end network connectivity.

## 🚀 Execution Steps
1. **Network Architecture & Evolution Analysis:** 
   * Examined the fundamental purpose of computer networks: establishing communication and data exchange channels across diverse endpoints (workstations, mobile devices, IoT, IP cameras).
   * Traced the historical evolution of the Internet, exploring its origins from ARPANET to the modern World Wide Web as a global decentralized information platform.
2. **Addressing & Identification Schemes:** 
   * **Logical Addressing (IP):** Analyzed the structural differences between **IPv4** (32-bit addresses facing address exhaustion) and **IPv6** (128-bit addresses providing a virtually inexhaustible address pool).
   * **Physical Addressing (MAC):** Evaluated 12-character hexadecimal **MAC addresses**, analyzing their structure where the initial 6 characters represent the Organizationally Unique Identifier (OUI/manufacturer code) and the remaining 6 represent the unique Network Interface Controller (NIC) identifier.
3. **Connectivity Verification via ICMP:** 
   * Deployed the command-line utility `ping` to evaluate network availability and latency.
   * Analyzed **Internet Control Message Protocol (ICMP)** Echo Request and Echo Reply packets to measure round-trip time (RTT) and verify network route reachability.

## 📊 Results & Evidence
* Successfully differentiated between logical (IP) and physical (MAC) network addressing layers, decoded manufacturer prefixes from MAC addresses, and diagnosed network latency via ICMP utilities.

> 📸 <img width="946" height="247" alt="image" src="https://github.com/user-attachments/assets/62ebb6e6-3e8b-4314-a3b2-5910d01ace97" />

## 🧠 Key Takeaways
* **Dual Layer Identification:** Learned that network communication strictly relies on both logical addresses (IPs for routing across networks) and physical addresses (MAC addresses for local segment delivery).
* **The Transition to IPv6:** Recognized the operational necessity of IPv6 adoption due to the exhaustion of public IPv4 address spaces in modern enterprise environments.
* **ICMP as the First Line of Troubleshooting:** Understood that simple diagnostic tools like `ping` provide immediate visibility into network reachability, packet loss, and latency before diving into deep packet analysis.
