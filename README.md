# JanSahayak-AI
**An AI-powered assistant that helps citizens discover, check eligibility, and apply for government schemes using chat or voice in regional languages.**
The goal: Reduce information barriers and improve scheme access for rural and low-literacy users.

---

## 🧠 Core Features

### 1️⃣ Conversational AI (Scheme Discovery)

Users can ask queries like:

* “What schemes are available for farmers in Maharashtra?”
* “Any scholarships for engineering students?”
* “Schemes for women entrepreneurs?”

The AI agent:

* Searches a scheme knowledge base
* Retrieves relevant schemes
* Explains them in simple language

**Example Output:**

```
You may be eligible for:
1. PM Kisan Samman Nidhi
2. Maharashtra Krushi Yojana
3. Soil Health Card Scheme
```

---

### 2️⃣ Smart Eligibility Checker

Users enter details or upload a simple form:

**Example Inputs:**

* State
* Income
* Occupation
* Age
* Land ownership
* Category

The AI system evaluates eligibility rules stored in the database.

**Example Output:**

```
You are eligible for:
✓ PM Kisan
✓ Crop Insurance Scheme

Not Eligible:
✗ PM Awas Yojana (income exceeds limit)
```

Saves users hours of manual research.

---

### 3️⃣ Step-by-Step Application Guide

After selecting a scheme, the agent provides:

* Application Steps
* Portal links
* Account registration instructions
* Form filling guidance
* Document checklist

**Example Documents:**

* Aadhaar Card
* Bank Passbook
* Land Records
* Income Certificate

---

### 4️⃣ Voice Search for Rural Users 🎤

Users can speak instead of typing.

**Example:**

* User: “Maharashtra mein kisan ke liye kya yojana hai?”
* System: Converts speech → text → AI response → voice + text output

**Possible Free APIs:**

* Web Speech API (browser)
* Vosk
* Mozilla DeepSpeech

---

### 5️⃣ Regional Language Support 🌏

Supports multiple languages:

* Marathi
* Hindi
* Tamil
* English

AI automatically translates responses using:

* Google Translate API
* IndicTrans

---

## 🤖 Agentic AI Layer (Advanced)

Instead of a simple chatbot, multiple AI agents handle different tasks:

| Agent                        | Function                                                             |
| ---------------------------- | -------------------------------------------------------------------- |
| Query Understanding Agent    | Understands user intent and extracts context (e.g., state, category) |
| Scheme Retrieval Agent       | Searches scheme database using vector embeddings (FAISS, Pinecone)   |
| Eligibility Evaluation Agent | Applies eligibility rules on user profile                            |
| Application Helper Agent     | Guides step-by-step, generates checklist, explains forms             |

---

## 🗂 Dataset Sources

* **Government Open Data:** data.gov.in
* **Ministry of Agriculture & Farmers Welfare**
* **National Informatics Centre**
* **State Portals:** e.g., Government of Maharashtra schemes portal

---

## 🧱 Suggested Tech Stack

**Frontend:** React + TailwindCSS + Voice UI
**Backend:** Node.js + Express.js
**Database:** MongoDB (stores scheme info, eligibility rules, documents)
**AI Layer:** LLM + Retrieval (OpenAI API, LLaMA)
**Semantic Search:** Embeddings + Vector DB

---

## 🏗 System Architecture

```
User (Chat / Voice)
      │
      ▼
Frontend (React)
      │
      ▼
Backend API (Node.js)
      │
      ▼
AI Agent Layer
├─ Query Agent
├─ Scheme Search Agent
├─ Eligibility Agent
└─ Application Guide Agent
      │
      ▼
Database (MongoDB + Vector DB)
```

---

## 🚀 Future Extensions

* **Document Auto-Fill:** Upload Aadhaar → auto-fill scheme forms
* **Location-Based Schemes:** Show schemes by district or village
* **WhatsApp Integration:** Access AI agent via WhatsApp for rural adoption
* **Government Dashboard:** Analytics for policymakers (search trends, awareness gaps)

---

## 💡 Why This Idea Is Powerful

* Solves a national problem: 1000+ schemes exist but citizens lack awareness
* Simplifies application process for rural and low-literacy users
* Strong candidate for:

  * Hackathons
  * Final year projects
  * Startups & GovTech solutions

---
