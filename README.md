# 🌱 **AgroCycle.AI – Smart Farm Waste-to-Energy Platform**

**Developed by:** *S.M. Sakthivel*
*AI • ML • Data Engineering • Cloud Deployment*

---

## 🚀 **Project Overview**

**AgroCycle.AI** is an AI-powered web platform that converts **agricultural waste** into valuable resources like **compost or biogas**, while automatically estimating **greenhouse gas (GHG) savings**, calculating **carbon credits**, and generating a **digital sustainability certificate**.

This project showcases the integration of **Artificial Intelligence and Sustainability**, helping farmers monetize agricultural residues through **carbon credit estimation** and **eco-friendly waste management**.

---

## 🧩 **Problem Statement**

**Domain:** AgriTech & Environment
**Challenge:** Rural areas often burn or discard farm waste, releasing large amounts of methane and CO₂. AgroCycle.AI introduces a **data-driven solution** that recommends waste conversion methods while quantifying the environmental benefits.

---

## 🧠 **Key Objectives**

* Detect and classify farm waste using AI
* Recommend optimal conversion method (Biogas / Compost)
* Estimate GHG emissions avoided (CO₂e saved)
* Convert GHG savings into **carbon credits**
* Generate an automatically downloadable **PDF certificate**

---

## 🧱 **System Architecture**

### **Layers Overview**

1. **User Layer** – Image upload or manual waste type input
2. **Frontend (React)** – Displays classification results and downloadable certificate
3. **Backend (FastAPI)** – Handles model inference, logic, and APIs
4. **Processing Layer**

   * YOLOv8 for waste classification
   * NLP for manual waste description
   * GHG & carbon credit estimation
   * ReportLab-based certificate generation
5. **Database Layer**

   * PostgreSQL: Waste data, emission factors, credit rates
   * Firebase: Authentication & logs
6. **Deployment**

   * Frontend → Vercel
   * Backend → Render

---

## ⚙️ **System Modules**

### 1️⃣ Waste Detection & Classification

* Image-based classification using **YOLOv8**
* NLP handles manual waste text inputs

### 2️⃣ Biogas or Compost Recommendation

* Suggests conversion method based on waste type & volume

### 3️⃣ GHG Savings & Carbon Credit Estimation

* Formula-based CO₂e computation
* 1 ton CO₂e = 1 Carbon Credit
* Converts credits to INR using live rate data

### 4️⃣ Certificate Generation

* Automated PDF certificate
* Displays GHG savings, carbon credits, and QR validation link

---

## 🧰 **Tech Stack**

| Layer             | Tools / Frameworks                     |
| ----------------- | -------------------------------------- |
| **Frontend**      | React.js, Tailwind CSS                 |
| **Backend**       | FastAPI (Python)                       |
| **ML/AI**         | YOLOv8, HuggingFace Transformers, NLTK |
| **Database**      | PostgreSQL, Firebase                   |
| **PDF Generator** | ReportLab                              |
| **Deployment**    | Vercel (Frontend), Render (Backend)    |
| **Infra / CI**    | GitHub Actions, TorchServe             |

---

## 🧪 **Setup Instructions**

### 🔧 Backend Setup

```bash
git clone https://github.com/<your-repo>/AgroCycle.AI
cd backend
pip install -r requirements.txt
uvicorn main:app --reload
```

### 💻 Frontend Setup

```bash
cd frontend
npm install
npm run dev
```

---

## 🧪 **Sample API Response**

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

## 📁 **Folder Structure**

```
AgroCycle.AI/
├── frontend/          # React UI
├── backend/           # FastAPI APIs
│   ├── app/
│   ├── models/        # YOLOv8 + NLP logic
│   ├── routes/        # API endpoints
│   └── utils/         # PDF, recommender, GHG logic
├── models/            # Pre-trained weights
├── docs/              # Architecture diagrams & reports
└── README.md
```

---

## 📊 **Expected Output**

* Waste category & quantity
* Recommended waste treatment method
* GHG savings (in tons of CO₂e)
* Estimated carbon credits & INR value
* Auto-generated sustainability certificate

---

## 🚧 **Future Enhancements**

1. Integration with live carbon credit APIs
2. IoT-based real-time waste measurement
3. Multi-language dashboard for rural users
4. AI model fine-tuning with region-specific datasets

---

## 🧑‍💻 **Developed By**

**S.M. Sakthivel**
AI / ML & Cloud Developer
📧 **[s.m.sakthivelofficial@gmail.com](mailto:s.m.sakthivelofficial@gmail.com)**

---

✅ **Summary:**
**AgroCycle.AI** transforms agricultural waste management into a measurable, income-generating sustainability solution — merging **AI, Environment, and Data Science** for a cleaner, smarter planet.

---
