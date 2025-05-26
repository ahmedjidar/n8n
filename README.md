# 🚀 n8n Automations Suite

> A collection of three powerful n8n workflows that supercharge your CRM and knowledge-base processes.

[![n8n Workflow](https://img.shields.io/badge/n8n-%23FF6C00?style=for-the-badge&logo=n8n)](https://n8n.io)  
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](/LICENSE)  
[![Made with ❤️](https://img.shields.io/badge/Made%20with-%E2%9D%A4-red.svg)]()

---

## 📦 Table of Contents

1. [Overview](#overview)  
2. [Workflows](#workflows)  
   - [Smart CRM Agent](#1-smart-crm-agent)  
   - [Smart CRM AutoFill](#2-smart-crm-autofill)  
   - [Simple RAG Agent](#3-simple-rag-agent)  
3. [Getting Started](#getting-started)  
4. [Configuration & Usage](#configuration--usage)  
5. [Contributing](#contributing)  

---

## 🔍 Overview

This repo houses three n8n workflows designed to:

- **Automate** repetitive CRM tasks  
- **Extract** and **process** data from emails & attachments  
- **Enable** context-aware, retrieval-augmented AI queries  

Each workflow is plug-and-play: import into your n8n instance, configure credentials, and you’re ready to go!

---

## 🛠️ Workflows

### 1. Smart CRM Agent

> Automatically executes Salesforce tasks based on natural-language prompts.

| Feature                   | Description                                      |
| ------------------------- | ------------------------------------------------ |
| Prompt-driven actions     | “Create a follow-up task with due date …”         |
| Salesforce integration    | Leverages REST API to read/write records          |
| Error handling & logging  | Built-in retry logic and detailed execution logs |

![Smart CRM Agent](https://github.com/user-attachments/assets/d7e5c8d5-fe5a-463c-a5b5-4d2ca4da5c34)

---

### 2. Smart CRM AutoFill

> From email attachments → OCR → CRM update, fully hands-off.

| Stage                     | Details                                                   |
| ------------------------- | --------------------------------------------------------- |
| Email ingestion           | Extract attachments via Gmail node + regex filters       |
| OCR processing            | Send docs to OCR API for text extraction                  |
| CRM update                | Map parsed fields into your CRM (HubSpot, Salesforce…)   |

![Smart CRM AutoFill](https://github.com/user-attachments/assets/cbcbd29e-e84e-4dce-98bd-0df2e81ba380)

---

### 3. Simple RAG Agent

> Retrieval-Augmented Generation over your custom data set.

| Component                 | Description                                                         |
| ------------------------- | ------------------------------------------------------------------- |
| Vector store              | Supabase embeddings + pgvector                                       |
| Text splitting            | Recursive character splitter for optimal chunking                   |
| LLM orchestration         | Query your data, get precise answers with minimal prompt engineering |

![Simple RAG Agent](https://github.com/user-attachments/assets/b397a5ae-81de-4b24-8008-0b67703634e6)

---

## 🚀 Getting Started

1. **Clone the repo**  
   git clone https://github.com/ahmedjidar/n8n.git
   cd n8n-automations

2. **Import into n8n**

   * Open your n8n editor
   * Click **Import** → paste the JSON from `workflows/`
3. **Configure credentials**

   * Create API credentials (Salesforce, Gmail, OCR service, Supabase, OpenAI, etc.)
   * Add them to your n8n **Credentials** tab

---

## ⚙️ Configuration & Usage

Each workflow comes with a `README.md` in its folder outlining:

* Required **environment variables**
* **Endpoints** & webhooks to expose
* **Example payloads** for testing

> 💡 Tip: Use n8n’s **Test** mode to step through each node on first run.

---

## 🤝 Contributing

1. Fork this repo
2. Create a branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -am 'Add new workflow'`)
4. Push to branch (`git push origin feature/your-feature`)
5. Open a Pull Request


