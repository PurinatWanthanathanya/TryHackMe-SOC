# Lab: How Websites Work

**Role:** Pre-Security Student / Web Security Trainee

## 🎯 Objective
To understand the core architectural components of modern websites, analyze the interaction between clients and servers, evaluate front-end and back-end technologies, and identify basic security risks such as source code exposure and HTML injection.

## 🚀 Execution Steps
1. **Client-Server & Tier Architecture:** 
   * Analyzed the underlying web communication model where a client browser requests resources and a remote server processes and responds.
   * Differentiated between **Front-end** components (rendered locally by the browser) and **Back-end** systems responsible for handling business logic and database interactions.
2. **Web Technologies Evaluation (HTML & JavaScript):** 
   * Investigated core web languages, focusing on **HTML** for structuring web page elements and **JavaScript** for introducing dynamic and interactive functionality.
   * Inspected page source codes to understand how browser rendering engines interpret these scripts.
3. **Web Vulnerability & Security Analysis:** 
   * Examined common security pitfalls in web development, recognizing that improper handling or leaving sensitive data exposed within client-side source code poses severe privacy risks.
   * Analyzed how inadequate input sanitization can lead to **HTML Injection** vulnerabilities, emphasizing the necessity of secure coding practices.

## 📊 Results & Evidence
* Successfully mapped web application request workflows, evaluated front-end script structures, and identified fundamental web security vulnerabilities related to source code handling and input processing.

> 📸 HTML<br><img width="956" height="745" alt="image" src="https://github.com/user-attachments/assets/30e24601-ee1a-4b96-823e-0e9399e7d000" />

> 📸 JS<br><img width="984" height="754" alt="image" src="https://github.com/user-attachments/assets/03a7e0b1-b3af-4297-9c49-4a86c83ac8e2" />

> 📸 Sensitive Data Exposure<br><img width="1599" height="782" alt="image" src="https://github.com/user-attachments/assets/58cf9473-5bfb-4387-8da2-389bd471bfcc" />

> 📸 HTML Injection<br><img width="987" height="749" alt="image" src="https://github.com/user-attachments/assets/bb321ec5-751c-4499-bade-91df4de243f7" />

## 🧠 Key Takeaways
* **The Web is More Than Meets the Eye:** Learned that what users see in a browser (Front-end) is only a fraction of the architecture; robust Back-end systems and secure databases power the underlying functionality.
* **Never Trust the Client:** Recognized that client-side code (HTML/JavaScript) can always be viewed, inspected, and manipulated by the user, meaning critical security checks must *always* be handled on the server side.
* **Sanitization Prevents Exploits:** Understood that failing to properly sanitize user inputs opens the door to injection attacks, making input validation a vital first line of defense in web application security.
