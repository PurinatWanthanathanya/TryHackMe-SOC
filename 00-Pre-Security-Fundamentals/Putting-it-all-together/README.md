# Lab: Putting it all together

**Role:** Pre-Security Student / Web Security Trainee

## 🎯 Objective
To synthesize comprehensive web architecture concepts by analyzing the end-to-end request-response cycle, evaluating infrastructure performance components (Load Balancers, CDNs, WAFs), and successfully sequencing the website loading process to complete a practical investigation.

## 🚀 Execution Steps
1. **Web Infrastructure & Performance Analysis:** 
   * Evaluated the foundational request-response cycle powering modern web applications.
   * Investigated the role of architectural components designed to scale performance and security, including **Load Balancers** (for distributing traffic), **CDNs** (Content Delivery Networks for caching edge content), and **WAFs** (Web Application Firewalls for filtering malicious traffic).
2. **Web Server Configuration & Content Separation:** 
   * Analyzed web server functionalities, focusing on the use of **Virtual Hosts** to manage and host multiple independent domains on a single physical server.
   * Differentiated between **Static Content** (files delivered directly to the client) and **Dynamic Content** (processed on the server side), verifying that backend code execution remains entirely hidden from client visibility.
3. **Practical Sequence Investigation:** 
   * Executed a practical lab challenge requiring the precise logical sequencing of the website loading process.
   * Analyzed network events step-by-step from initial DNS resolution to final browser rendering, successfully isolating key artifacts to retrieve the target flag.

## 📊 Results & Evidence
* Successfully mapped comprehensive web infrastructure layers, differentiated content delivery mechanisms, and correctly sequenced the website loading workflow to capture the lab flag.

> 📸 <img width="981" height="743" alt="image" src="https://github.com/user-attachments/assets/3cb8816e-8666-4315-86be-32df38af73e9" />

> 📸 <img width="954" height="743" alt="image" src="https://github.com/user-attachments/assets/84e5a9e8-4279-4234-9991-4a3c95fd56a8" />

## 🧠 Key Takeaways
* **The Big Picture of Web Architecture:** Learned that a website is not just a single server; modern web applications rely on a complex ecosystem of CDNs, load balancers, and firewalls working in harmony.
* **Backend Isolation:** Reinforced the critical security principle that backend processing logic is strictly hidden from the client, ensuring sensitive operations and database queries cannot be directly manipulated by end users.
* **End-to-End Sequencing:** Recognized that troubleshooting or securing a web application requires a holistic understanding of every single step in the request-response lifecycle—from the moment a user types a URL to the final DOM rendering in the browser.
