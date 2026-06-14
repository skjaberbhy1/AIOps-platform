# 🚀 AIOps Intelligent Network Automation Platform

![AI](https://img.shields.io/badge/AI-RAG%20%2B%20LLM-blue)
![Backend](https://img.shields.io/badge/FastAPI-Python-green)
![Architecture](https://img.shields.io/badge/Architecture-Multi--VM-orange)
![Nautobot](https://img.shields.io/badge/Network-Nautobot-red)

> AI-powered Network Operations Platform with RAG, LLM, and Nautobot integration for real-time infrastructure intelligence.



## 👨‍💻 Project Overview

This project is a production-grade **AIOps (AI for IT Operations) platform** built using a distributed multi-VM architecture.  
It integrates **RAG (Retrieval Augmented Generation), Vector Search, LLM inference, and Nautobot-based network automation** to create an intelligent infrastructure assistant.

The system enables real-time network intelligence, automated troubleshooting, and AI-powered chatbot interaction for IT operations teams.

---

## 🏗️ System Architecture (Multi-VM Design)

### 🖥️ VM 1 – RAG Embedding Pipeline
- Document ingestion and preprocessing
- Chunking and embedding generation
- Converts knowledge base into vector format
- Feeds data into vector database

---

### 🗄️ VM 2 – Vector Database Layer
- Stores embeddings for semantic search
- Enables fast context retrieval
- Powers RAG-based AI responses
- Acts as knowledge memory layer

---

### 🤖 VM 3 – AI Model Server
- Hosts LLM inference engine
- Combines user query + retrieved context
- Performs reasoning and response generation
- Hybrid AI (RAG + Tool Calling)

---

### 🌐 VM 4 – Web API & Chatbot (FastAPI + Nautobot)
- Chatbot backend built with FastAPI
- Intelligent query routing system
- Nautobot integration for network source of truth
- ELK + Observium integration for monitoring

---

## ⚙️ Key Features

### 🧠 AI Capabilities
- Retrieval-Augmented Generation (RAG)
- Context-aware response generation
- Intent detection (IP / Device / Logs / Alerts)
- Tool-based reasoning with LLM

---

### 🌐 Network Automation (Nautobot Integration)
- Device → IP resolution
- IP → Device mapping
- Network inventory lookup
- Real-time infrastructure queries

---

### 📡 Observability & Monitoring
- ELK stack log analysis
- Device down detection via Observium
- Incident-aware responses
- Centralized monitoring intelligence

---

### 💬 AI Chatbot Interface
Natural language interface for IT operations.

#### Example Queries:
- What is the IP of device X?
- Which device is using IP 10.x.x.x?
- Show me down devices
- Fetch logs for router issue

---

## 🧩 Technology Stack

- **Backend:** FastAPI, Python
- **AI/LLM:** Local LLM + RAG Pipeline
- **Vector DB:** Qdrant (or custom implementation)
- **Network Source of Truth:** Nautobot
- **Monitoring:** ELK Stack, Observium
- **Architecture:** Distributed Multi-VM System
- **Communication:** REST APIs

---

## 🔄 System Workflow

```
User Query
↓
Chatbot API (VM4)
↓
Intent Detection (LLM Router)
↓
┌──────────────────────────────┐
│ │
│ RAG System (VM1 + VM2) │
│ Nautobot API Queries │
│ Monitoring Tools │
│ │
└──────────────────────────────┘
↓
AI Model Server (VM3)
↓
Final Structured Response
```

## 🎯 Use Cases

- ISP / Telecom Network Automation
- NOC / SOC Operations Assistant
- Infrastructure Troubleshooting
- AI-based IT Support Chatbot
- Real-time Network Intelligence Platform

---

## 📈 Impact

- ⚡ Reduced manual network lookup time
- ⚡ Centralized infrastructure intelligence
- ⚡ Faster incident resolution
- ⚡ AI-powered operational efficiency
- ⚡ Unified chat-based IT operations system

---

## 👨‍💻 Author

**Sheikh Jaber Bin Ahmed Bhuiyan**  
DevOps & AI Infrastructure Engineer  

### Expertise:
- DevOps, AIOps & Network Automation
- LLM + RAG Systems
- Elasticsearch / Monitoring Systems
- Infrastructure Engineering

---

## 🚀 Future Improvements

- React-based Chat UI Dashboard
- Slack / Microsoft Teams Bot Integration
- Kubernetes deployment version
- Multi-tenant SaaS AIOps platform
- Real-time alert intelligence engine

---

## 📌 Summary

This project demonstrates a full-stack **AI-powered Network Operations platform** combining:

- Distributed systems
- AI reasoning (LLM + RAG)
- Network automation (Nautobot)
- Observability integration

It acts as an intelligent assistant for modern IT infrastructure teams

## 📸 System Screenshots

### 1. Chatbot + Nautobot Integration
Shows end-to-end IP ↔ Device resolution via Nautobot source of truth.

![Chatbot Demo](/docs/screenshots/03_nautobot_chatbot_end_to_end_demo.png)

---

## 2. RAG Retrieval Pipeline (Qdrant)

This section shows the complete Retrieval-Augmented Generation (RAG) workflow including query embedding, vector search, similarity scoring, and context retrieval.

### Step 1: Query + Embedding
![RAG Step 1](/docs/screenshots/04_rag_query_embedding_search.png)


### Step 2: Vector Search (Qdrant) – Personal Knowledge Retrieval

Retrieves semantically similar chunks related to the user query (Jaber profile data) from the vector database.

![RAG Step 2 - Jaber Query Retrieval](/docs/screenshots/02_rag_flow.png)


### Step 3: Retrieved Context + LLM Response
![RAG Step 3](/docs/screenshots/05_qdrant_retrieval_llm_answer.png)


---

### 3. LLM Inference (Ollama - qwen2.5:7b)
Local AI model response generated via Ollama runtime.

![LLM Inference](/docs/screenshots/06_ollama_qwen2_5_model_inference.png)
