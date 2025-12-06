# 🌱 **AgriWaste2Fuel – AI-Powered Farm Waste-to-Energy Platform**

<p align="center">
  <img src="https://img.shields.io/badge/AI-AgriTech-green?style=for-the-badge" />
  <img src="https://img.shields.io/badge/ML-YOLOv8-blue?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Backend-FastAPI-yellow?style=for-the-badge" />
  <img src="https://img.shields.io/badge/Frontend-React-orange?style=for-the-badge" />
  <img src="https://img.shields.io/badge/License-MIT-purple?style=for-the-badge" />
</p>

---

## 🚀 **Overview**

**AgriWaste2Fuel** is an AI-driven platform that transforms **agricultural waste** into useful resources such as **biogas or compost**.
It automatically estimates:

* 🌍 **GHG emissions avoided (CO₂e savings)**
* 💰 **Carbon credits generated**
* 🧾 **Downloadable sustainability certificate (PDF)**

This platform helps farmers turn waste into **income**, supports sustainability, and reduces rural pollution caused by waste burning.

---

## 🧩 **Problem Statement**

Agricultural waste is often burned or dumped, releasing:

* Methane (CH₄)
* Carbon dioxide (CO₂)
* Other greenhouse gases

**AgriWaste2Fuel** provides a **smart, data-driven solution** to recommend the best waste treatment method and estimate environmental impact & monetary benefits.

---

## 🎯 **Key Features**

### 🔍 1. AI-Based Waste Classification

* YOLOv8 for image detection
* NLP for manual waste text input

### ⚡ 2. Waste-to-Energy Recommendation

* Biogas or Compost based on waste type & volume

### 🌍 3. GHG Emission Savings

* Calculates CO₂e reductions using standard emission factors

### 💳 4. Carbon Credit Estimation

* 1 ton CO₂e = 1 Carbon Credit
* Converts credits → INR (live rate supported)

### 🧾 5. PDF Certificate Generator

* Auto-generated with QR verification link
* Includes GHG savings & income estimate

---

## 🏗️ **System Architecture**

```
User → Frontend (React) → FastAPI Backend → AI Models → Database → PDF Generator → Output
```

### **Components**

* **Frontend:** React + Tailwind CSS
* **Backend:** FastAPI
* **Models:** YOLOv8, NLP Transformer
* **Database:** PostgreSQL + Firebase Auth
* **Deployment:** Vercel (Frontend) & Render (Backend)

---

## 🧰 **Tech Stack**

| Layer          | Technologies                           |
| -------------- | -------------------------------------- |
| **Frontend**   | React, Tailwind CSS                    |
| **Backend**    | FastAPI, Python                        |
| **ML/AI**      | YOLOv8, HuggingFace Transformers, NLTK |
| **Database**   | PostgreSQL, Firebase                   |
| **PDF**        | ReportLab                              |
| **CI/CD**      | GitHub Actions                         |
| **Deployment** | Vercel, Render                         |

---

## 📂 **Folder Structure**

```
AgriWaste2Fuel/
├── frontend/              # React UI
├── backend/               # FastAPI Engine
│   ├── app/
│   ├── models/            # YOLOv8 weights + NLP
│   ├── routes/            # API endpoints
│   └── utils/             # GHG logic, certificate generator
├── models/                # Pre-trained ML models
├── docs/                  # Architecture diagrams, research
└── README.md
```

---

## 🛠️ **Installation & Setup**

### 🔧 Backend Setup

```bash
git clone https://github.com/<your-username>/AgriWaste2Fuel
cd AgriWaste2Fuel/backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### 💻 Frontend Setup

```bash
cd AgriWaste2Fuel/frontend
npm install
npm run dev
```

---

## 🔌 **API Example Response**

```json
{
  "waste_type": "cow dung",
  "method": "biogas",
  "ghg_savings_tons": 0.42,
  "carbon_credits": 0.42,
  "estimated_income_inr": 840,
  "certificate_url": "/api/download/certificate?id=abc123"
}
```

---

## 📊 **Expected Output**

* Waste category & volume
* Treatment recommendation
* GHG savings (CO₂e tons)
* Carbon credit estimate
* Income projection (INR)
* Downloadable digital certificate

---

## 🚧 **Future Enhancements**

* 🔗 Integration with live carbon credit marketplaces
* 📡 IoT sensors for real-time waste measurement
* 🌐 Multi-language UI
* 🎯 Region-specific dataset training for accuracy

---

## 🙌 **Developed By**

**S.M. Sakthivel**
AI | Machine Learning | Cloud Deployment
📧 **[s.m.sakthivelofficial@gmail.com](mailto:s.m.sakthivelofficial@gmail.com)**

---

## 📜 **License**

This project is licensed under the **MIT License**.

---
