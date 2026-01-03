# AICP: AI - Crime Prevention

![Project Banner](https://github.com/user-attachments/assets/a39473b1-97a9-4c26-9a94-dd9d05f85915)

> **Graduation Thesis Project** | *University of Economics - The University of Da Nang*

## Introduction

**AI-PCTP** is a comprehensive web application designed to empower users against cyber threats. It combines educational resources with advanced AI tools to detect phishing URLs, analyze fraudulent images (SMS/Emails), and provide real-time cybersecurity intelligence.

The platform leverages **Generative AI (LLM)** for a context-aware chatbot and computer vision models for visual threat analysis.

## Key Features

### 1. Cybersecurity Knowledge Hub
An immersive educational section featuring interactive video scrolling, articles on common threats (Ransomware, MITM, Phishing), and visual storytelling.

| Immersive Hero Section | Threat Topics |
|:---:|:---:|
| ![About Hero](https://github.com/user-attachments/assets/a8432cc1-151b-4071-95e8-c1f7c51d5e8e) | ![Topics](https://github.com/user-attachments/assets/1b695cec-9221-48ee-aae1-20269a83e6a9) |
| *Interactive scroll-based learning* | *Detailed info on cyber threats* |

### 2. Real-time Threat Intelligence
Integration with global security databases to provide up-to-date information.
* **Live Cyber Threat Map:** Visualizes real-time attacks via Kaspersky API.
* **CVE Database:** Searchable Microsoft CVE vulnerability list.

| Live Threat Map | CVE Database |
|:---:|:---:|
| ![Map](https://github.com/user-attachments/assets/142acad2-d5fe-4c24-8023-bd2ac7cd1b66) | ![CVE](https://github.com/user-attachments/assets/5017cc9a-601d-4639-ba41-74597a929ca8) |

### 3. AI Assistant (RAG Chatbot)
A smart chatbot capable of answering cybersecurity queries. It uses **RAG (Retrieval-Augmented Generation)** to fetch data from the internal CVE database and provides accurate answers via Groq SDK.

![Chat Interface](https://github.com/user-attachments/assets/7b6b16e6-72d8-45ee-9fbe-d81abe639fb2)
*Features: Markdown support, Chat History, Typing effects, and Context-aware responses.*

### 4. URL Verifier (Dual-Engine Scanning)
Checks URLs for safety using a hybrid approach:
1.  **VirusTotal API:** Checks against known blacklists.
2.  **Visual AI Analysis:** Captures a screenshot of the website and uses AI to visually detect phishing elements (fake login forms, logos).

| Verify Interface | AI Visual Analysis |
|:---:|:---:|
| ![Verify UI](https://github.com/user-attachments/assets/5cda04f6-df6e-4077-8395-f8d31c44cfaa) | ![Verify Result](https://github.com/user-attachments/assets/b0b04ffe-e545-4376-9ae3-a7964c07fa9e) |

### 5. AI Fraud Scanner (OCR + NLP)
Users can upload screenshots of suspicious messages (SMS, Zalo, Email). The system uses **OCR** to extract text and **NLP** to analyze the intent, identifying potential scams and providing actionable advice.

| Upload Interface | Scan Result | Recommendations |
|:---:|:---:|:---:|
| ![Scan UI](https://github.com/user-attachments/assets/ff97e0e5-cbe5-4f3f-b927-c5652640e7f9) | ![Result](https://github.com/user-attachments/assets/dd177c76-84a0-4d17-8b93-389ad262642c) | ![Advice](https://github.com/user-attachments/assets/e6f86e1f-747a-462b-8b5f-d7c23040b17f) |

### 6. Security Awareness Quiz
A gamified test to evaluate user knowledge regarding cybersecurity practices.

![Quiz](https://github.com/user-attachments/assets/c2660f75-f491-4e1c-9c41-90f696d2a54c)

---

## Tech Stack

### Frontend
* **React.js (Vite):** Core framework for a fast, SPA experience.
* **Tailwind CSS:** For modern, responsive styling.
* **Framer Motion:** High-performance animations and transitions.

### Backend
* **Node.js & Express:** RESTful API server.
* **MongoDB:** User authentication and profile management.
* **SQLite:** High-performance local database for CVE data.

### AI & Services
* **Python Microservice:** Handles heavy AI tasks (OCR, Visual Analysis).
* **Groq SDK:** Ultra-fast LLM inference for the Chatbot.
* **VirusTotal API:** URL reputation checking.
* **Microsoft Security API:** Fetching latest vulnerabilities.
