# Lab: HTTP in Detail

**Role:** Pre-Security Student / Web Protocol Trainee

## 🎯 Objective
To deconstruct the mechanics of Hypertext Transfer Protocol (HTTP/HTTPS), evaluate the architectural anatomy of Uniform Resource Locators (URLs), analyze standard HTTP request methods and status codes, and inspect request/response headers and browser cookies during live client-server communication.

## 🚀 Execution Steps
1. **URL Structural Anatomy Deconstruction:** 
   * Deconstructed the anatomical components of a standard URL:
     * **Scheme:** Defining the transmission protocol (e.g., `http://`, `https://`).
     * **Host & Port:** Specifying the target domain or IP address and service port.
     * **Path & Query String:** Identifying the specific server-side resource path and passed parameters.
2. **HTTP Request Methods & Status Codes Evaluation:** 
   * Analyzed RESTful interaction methods utilized to interact with server-side resources:
     * **GET:** Retrieving data from a designated endpoint.
     * **POST:** Submitting client data to create or process resources.
     * **PUT & DELETE:** Updating existing records or removing designated server resources.
   * Categorized HTTP status code responses:
     * **2xx (Success):** Standard confirmations such as `200 OK`.
     * **3xx (Redirection):** Route forwarding indicators.
     * **4xx (Client Errors):** Endpoint or authorization issues (e.g., `403 Forbidden`, `404 Not Found`).
     * **5xx (Server Errors):** Backend server failures (e.g., `500 Internal Server Error`).
3. **Header Inspection, Cookies & Simulated Requests:** 
   * Inspected critical HTTP headers including `Content-Type` for payload definition and `User-Agent` for client identification.
   * Examined **Cookies** within browser developer tools to analyze state-tracking and session handling.
   * Executed simulated HTTP requests to observe dynamic client-server handshake workflows and header exchanges.

## 📊 Results & Evidence
* Successfully parsed complex URL parameters, evaluated HTTP request/response lifecycles, and mapped web communication flows via Developer Tools and simulated query utilities.

> 📸 <img width="1140" height="270" alt="image" src="https://github.com/user-attachments/assets/33518d43-865f-4bdf-a155-b85d0829492d" />

> 📸 <img width="1140" height="800" alt="image" src="https://github.com/user-attachments/assets/5551b3d0-3aab-4c1b-87ec-83b711de0264" />

> 📸 <img width="950" height="627" alt="image" src="https://github.com/user-attachments/assets/6ef2ae98-2e17-4b80-9832-24fa4f30c2f7" />

## 🧠 Key Takeaways
* **HTTP is Inherently Stateless:** Learned that HTTP requires mechanisms like Cookies and Session Tokens to maintain user states and authentication across subsequent requests.
* **Headers Reveal Context:** Recognized that request and response headers provide vital operational telemetry for security analysts, from identifying client device types (User-Agent) to detecting backend server technologies.
* **Granular Status Code Triage:** Understood how HTTP status codes accelerate incident triage—spikes in 4xx codes often indicate web scanning or brute-force attempts, while 5xx codes point to application layer denial-of-service or exploitation attempts.
