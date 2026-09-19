# Lab: Cryptography Concepts

**Role:** Pre-Security Student / Cryptography Trainee

## 🎯 Objective
To understand the foundational principles of modern cryptography, evaluate the mathematical mechanics of symmetric and asymmetric encryption, analyze the key distribution challenge, and deconstruct hybrid encryption implementations such as HTTPS.

## 🚀 Execution Steps
1. **Cryptographic Foundations & Key Terminology:** 
   * Deconstructed fundamental concepts: Plaintext, Ciphertext, Secret Keys, and Cryptographic Algorithms used to preserve data confidentiality and integrity across networks.
2. **Symmetric vs. Asymmetric Cryptosystems:** 
   * Analyzed **Symmetric Encryption** (e.g., AES), which relies on a single shared secret key for both encryption and decryption; evaluated its primary operational vulnerability—the key distribution problem.
   * Investigated **Asymmetric Encryption** (Public-Key Cryptography) utilizing mathematically paired Public and Private keys, where data encrypted with the public key can only be decrypted by the corresponding private key.
3. **Hybrid Encryption Architecture (Real-World Application):** 
   * Examined modern secure communication protocols (e.g., HTTPS/TLS) that combine both cryptosystems:
     * Utilizing asymmetric encryption during the initial handshake to securely exchange a shared session key.
     * Transitioning to high-performance symmetric encryption for subsequent bulk data transmission.

## 📊 Results & Evidence
* Successfully differentiated encryption architectures, evaluated key exchange mechanics, and analyzed real-world hybrid encryption workflows in secure protocols.

> 📸 <img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/f575185d-e2ba-4823-9fe4-55ba44c98295" />

> 📸<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/9d435a6a-ac5d-45e8-833d-15049c7e8e51" />

> 📸 <img width="865" height="742" alt="image" src="https://github.com/user-attachments/assets/f587916a-ae90-4763-9360-b07dae4b77d8" />

> 📸<img width="1200" height="800" alt="image" src="https://github.com/user-attachments/assets/eec8b544-2c14-4476-a73a-b8e8d0577a58" />

## 🧠 Key Takeaways
* **Symmetric for Speed, Asymmetric for Key Exchange:** Learned that symmetric encryption is computationally fast and ideal for large datasets, while asymmetric encryption solves the key exchange dilemma across untrusted networks.
* **Hybrid Approach Powers the Modern Web:** Recognized that real-world secure protocols rarely rely on one method alone; systems like HTTPS leverage the strengths of both symmetric and asymmetric algorithms.
* **Key Management is Paramount:** Understood that the ultimate strength of any cryptographic system lies in key generation, secure storage, and strict lifecycle management—if the key is compromised, encryption provides no defense.
