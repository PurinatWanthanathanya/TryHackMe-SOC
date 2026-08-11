# Lab: Virtualisation Basics

**Role:** Pre-Security Student / IT Fundamentals Trainee

## 🎯 Objective
To understand the core mechanics of virtualization, differentiate between hypervisor deployment models (Type 1 vs. Type 2), and analyze containerization as a lightweight alternative for modern infrastructure and isolated testing environments.

## 🚀 Execution Steps
1. **Hardware Abstraction Analysis:** 
   * Analyzed how virtualization resolves the inherent inefficiencies of the traditional "one server, one application" architecture.
   * Investigated the role of the hypervisor in dynamically provisioning and partitioning physical hardware resources into multiple, independent Virtual Machines (VMs).
2. **Hypervisor Deployment Evaluation:** 
   * Differentiated between hypervisor architectures based on operational requirements.
   * Identified **Type 1 (Bare Metal)** hypervisors as the standard for enterprise production data centers due to direct hardware access.
   * Identified **Type 2 (Hosted)** hypervisors as optimal for individual testing, learning environments, and local malware analysis.
3. **Containerization Fundamentals:** 
   * Examined containers as a highly efficient, lightweight alternative to traditional VMs.
   * Evaluated how containers share the underlying host's operating system kernel, making them ideal for executing small, agile applications and microservices without the overhead of a full guest OS.

## 📊 Results & Evidence
* Successfully evaluated core virtualization models, identified appropriate hypervisor solutions for varying security environments, and distinguished the architectural differences between Virtual Machines and Containers.

> 📸 <br><img width="1350" height="1080" alt="image" src="https://github.com/user-attachments/assets/34b03c08-399f-47a4-a4ff-c1786bad228e" />

> 📸 <br><img width="731" height="470" alt="image" src="https://github.com/user-attachments/assets/167a73fc-e5bc-4628-ab09-5176867dad21" />

> 📸 <br><img width="913" height="863" alt="image" src="https://github.com/user-attachments/assets/4a85e59a-34dd-466b-b58f-7ae2bd8ebc6a" />

> 📸 <br><img width="951" height="738" alt="image" src="https://github.com/user-attachments/assets/ef22e2be-ec55-4240-900a-45599529692f" />

## 🧠 Key Takeaways
* **Maximizing Hardware Efficiency:** Learned that virtualization fundamentally transforms IT infrastructure by allowing a single physical server to securely host multiple isolated systems, drastically reducing hardware waste and operational costs.
* **Choosing the Right Hypervisor:** Recognized that while Type 1 hypervisors offer the performance and scalability required for enterprise data centers, Type 2 hypervisors provide the convenience and isolation necessary for an analyst's local workstation.
* **The Evolution of Containers:** Understood that containerization offers unprecedented speed and agility by bypassing the need to boot a full operating system for every application, representing the modern standard for application deployment.
