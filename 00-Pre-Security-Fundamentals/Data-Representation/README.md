# Lab: Data Representation

**Role:** Pre-Security Student / Computing Fundamentals Trainee

## 🎯 Objective
To understand how computing systems encode, store, and process information at the machine level, master numerical base conversions (Binary, Octal, Hexadecimal), and analyze practical applications such as memory addressing and 24-bit color representations.

## 🚀 Execution Steps
1. **Machine-Level Data Units:** 
   * Analyzed the foundational architecture of digital data storage based on **Bits** (binary digits representing 0 or 1) and **Bytes** (groups of 8 bits).
   * Traced how transistor states correspond to raw binary machine logic.
2. **Number System Transitions & Conversions:** 
   * Deconstructed different numbering systems utilized across operating systems and network communications:
     * **Binary (Base-2):** Machine-level execution and bitwise representations.
     * **Octal (Base-8):** File permission notations in Unix/Linux systems.
     * **Hexadecimal (Base-16):** Human-readable compact notation for large binary strings, memory addresses, and MAC addresses.
   * Executed manual and algorithmic conversion methods across Binary, Decimal, and Hexadecimal representations.
3. **Practical Implementation & Color Models:** 
   * Evaluated real-world encoding schemes, including **24-bit True Color (RGB)** mapping.
   * Deconstructed hex color codes into individual 8-bit Red, Green, and Blue intensity channels, demonstrating how binary values manifest visually.

## 📊 Results & Evidence
* Successfully converted numerical values across multiple bases (Base-2, Base-10, Base-16) and mapped byte-level values to memory addresses and visual digital representations.

> 📸 <img width="896" height="782" alt="image" src="https://github.com/user-attachments/assets/e7ea9646-ee69-4783-a98e-a96b897f8c18" />

## 🧠 Key Takeaways
* **Hexadecimal Simplifies Complexity:** Learned that Hexadecimal notation is not just an alternative number system; it is the industry standard for reading memory dumps, shellcode, and raw packet captures because 1 byte maps cleanly to exactly 2 hex characters.
* **Granular Security Analysis:** Recognized that deep-level security investigations (such as malware analysis, cryptography, and network packet dissection) require fluency in binary and hexadecimal to understand what is occurring below the application layer.
* **Standardized Encoding:** Understood that whether data represents an integer, text character, memory location, or pixel color, it is fundamentally stored as structured bit sequences interpreted according to standardized protocols.
