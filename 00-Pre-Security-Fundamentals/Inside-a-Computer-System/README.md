# Lab: Inside a Computer System

**Role:** Pre-Security Student / Computer Architecture Trainee

## 🎯 Objective
To understand the foundational hardware architecture of computer systems, evaluate the functional roles of essential physical components, and analyze the systematic execution of the hardware boot process from firmware execution to operating system handover.

## 🚀 Execution Steps
1. **Core Hardware Architecture Analysis:** 
   * Analyzed system components by mapping their functions conceptually:
     * **CPU (Central Processing Unit):** Functions as the primary processing engine executing computational instructions.
     * **Motherboard:** Acts as the structural and communications backbone interconnecting all hardware components.
     * **RAM (Random Access Memory):** Provides high-speed, volatile short-term memory for active processes.
     * **Storage Devices (HDD/SSD):** Manages non-volatile, long-term data retention.
2. **Peripheral & Subsystem Evaluation:** 
   * Investigated secondary support subsystems, including the **Power Supply Unit (PSU)** for power distribution, **Graphics Cards (GPU)** for visual rendering, and **Network Interface Cards (NIC)** for network communication.
3. **Hardware Boot Sequence Investigation:** 
   * Traced the sequential stages of the system initialization lifecycle:
     1. Power supply activation and voltage stabilization.
     2. Firmware execution (**UEFI / BIOS**).
     3. Execution of the **Power-On Self-Test (POST)** to verify hardware integrity.
     4. Boot device enumeration and prioritization.
     5. Execution of the target **Bootloader** to transition execution to the operating system.

## 📊 Results & Evidence
* Successfully mapped computer hardware architecture components and tracked the end-to-end hardware boot sequence.

> 📸 <img width="907" height="662" alt="image" src="https://github.com/user-attachments/assets/f3e5c0b4-87f1-4789-95cf-270a1da480ae" />

> 📸 <img width="885" height="507" alt="image" src="https://github.com/user-attachments/assets/d35706d1-d00c-4f94-a6c6-a94da4f85de9" />

## 🧠 Key Takeaways
* **Hardware is the Security Foundation:** Learned that software security relies directly on hardware integrity; vulnerabilities at the physical or firmware layer (like BIOS/UEFI) can undermine all OS-level defenses.
* **Volatile vs. Persistent Memory:** Recognized the operational difference between RAM and storage drives, which forms the basis for live volatile memory analysis during incident response.
* **The Boot Chain of Trust:** Understood how the system transitions from raw electrical power to firmware, and finally to the bootloader, forming the critical chain of trust needed for secure boot operations.
