# Lab: Operating Systems: Introduction

**Role:** Pre-Security Student / Operating Systems Trainee

## 🎯 Objective
To understand the foundational architecture of modern operating systems, evaluate resource management mechanisms, analyze the security boundaries between User Space and Kernel Space, and explore diverse OS deployment environments.

## 🚀 Execution Steps
1. **Core OS Functionality & Resource Management:** 
   * Analyzed the operating system's role as a central control unit managing core hardware and software resources.
   * Investigated primary resource subsystems:
     * **Process Management:** Scheduling and executing application threads.
     * **Memory Management:** Allocating and isolating physical and virtual address spaces.
     * **File System Management:** Organizing data storage, hierarchical paths, and access permissions.
     * **Device & User Management:** Controlling peripheral hardware access and authenticating user identities.
2. **Privilege Boundaries & System Architecture:** 
   * Examined security isolation between execution modes:
     * **User Space:** Restricted execution environment for user applications to prevent system crashes.
     * **Kernel Space:** Privileged layer with unrestricted hardware access and execution authority.
   * Traced how applications safely request hardware-level actions via **System Calls** interfacing directly with the kernel and Instruction Set Architecture (ISA).
3. **Environment Classification & User Interfaces:** 
   * Evaluated operating systems tailored for specific use cases, including Desktop, Server, Mobile, Embedded, and Cloud-based environments.
   * Contrasted interaction paradigms, analyzing system control via **Command-Line Interfaces (CLI)** versus **Graphical User Interfaces (GUI)**.

## 📊 Results & Evidence
* Successfully mapped the core architectural layers of an operating system, analyzed User Space versus Kernel Space isolation, and traced system call execution flows.

> 📸 <img width="358" height="255" alt="image" src="https://github.com/user-attachments/assets/96b4285f-3cb4-41e8-b343-b38b93446213" />

> 📸 <img width="927" height="785" alt="image" src="https://github.com/user-attachments/assets/53ca7454-aa83-4a25-a66f-48d3f035fa83" />

## 🧠 Key Takeaways
* **The Kernel is the Ultimate Authority:** Learned that the kernel holds unrestricted access to hardware; securing kernel space is paramount, as any kernel-level compromise bypasses all OS security boundaries.
* **Separation of Privilege via System Calls:** Recognized that user applications cannot access hardware directly; they must transition through system calls, which act as security gates to validate requests.
* **Architecture Dictates Security Posture:** Understood that the operational profile of an OS (Server, Desktop, or Cloud-native) determines its attack surface, services, and defense strategies.
