Enterprise AI Integration Solutions

Welcome! My name is Rishabh Sharda. I am a Technical Strategist and Solutions Engineer specializing in bridging complex enterprise platforms (SAP, ServiceNow) with modern AI workflows (LLMs, Agentic Pipelines).

Because my work heavily involves proprietary enterprise cloud environments (SAP BTP, ServiceNow instances) and visual orchestrators (n8n), traditional source code does not capture the full scope of my integrations.

Instead, this repository serves as an architectural portfolio showcasing my recent Proof of Concepts (POCs) and integration designs.

Featured Project: SAP + ServiceNow AI Document Pipeline

🎥 [Watch the Architecture Demo on YouTube](https://youtu.be/djuqj1pChkc)

📌 Overview

An end-to-end integration designed to reduce ServiceNow instance storage costs and automate business document classification using a hybrid of cloud automation and AI APIs.

🏗️ Architecture & Data Flow

Trigger: Unstructured business documents are ingested via SAP/ServiceNow workflows.

Orchestration: A custom n8n proxy intercepts heavy attachments to prevent ServiceNow storage bloat.

AI Classification:

Gemini API is utilized to classify the unstructured documents.

Local Gemma Models are used in a dual-pipeline setup for knowledge distillation and secure, localized processing.

Cloud Storage Routing: Classified documents are streamed securely to Google Drive via API.

Data Purge: A callback webhook confirms successful Drive storage and purges the original heavy attachment from ServiceNow.

🛠️ Tech Stack

Enterprise: SAP ECC / S4HANA, SAP CPI, ServiceNow

AI & Orchestration: n8n, Gemini API, Local LLMs (Gemma / Ollama)

Languages & Protocols: Python, REST APIs, OAuth2, Webhooks

If you are reviewing this for a Solutions Engineer or Strategist role, I would love to walk you through the business value and technical challenges of this architecture in person!

Academic ML Coursework (IIT Bombay)

🏏 IPL Cricket Broadcast Image Analysis (Collaborator)

* **[Link](https://github.com/goyaljai/PML-IITB-SEM1)** 

Project Scope:
A foundational Machine Learning project to detect and count cricket players from a custom, balanced dataset of 1,005 IPL broadcast images. Images were divided into an $8 \times 8$ grid (64 cells) to predict franchise presence and player counts per cell.

Technical Constraint:
Strictly utilized hand-crafted feature engineering for image classification. Deep learning frameworks, CNNs, and automatic feature extractors were prohibited to ensure mastery of core ML principles and modeling. The final trained model was serialized via .pkl.

My Specific Contribution:
I owned the algorithm and logic for the player counting task across highly diverse match conditions (varying lighting, occlusions, crowd backgrounds).

Performance: Achieved an $82.4\%$ accuracy margin ($\pm 1$ player) and a $47\%$ exact match rate.

If you are reviewing this for a Solutions Engineer or Strategist role, I would love to walk you through the business value and technical challenges of these architectures in person!
