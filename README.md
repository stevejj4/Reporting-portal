# 🚀 BigQuery-Based Reporting Assistant

## 📌 Project Overview
This project is a **scalable, AI-powered reporting assistant** that integrates with **BigQuery** for real-time analytics. It allows users to generate reports, ask AI-driven questions, and visualize insights dynamically.

## 🏗️ Architecture
### **1️⃣ Data Pipeline (ETL) - Apache Airflow / dbt / PySpark**
- Extracts data from **Google Sheets, APIs**.
- Transforms and loads data into **BigQuery**.

### **2️⃣ Backend API (FastAPI)**
- Handles **authentication (OAuth - Google, Firebase, Microsoft)**.
- Provides endpoints for querying **BigQuery reports**.
- Integrates **AI chatbot (LLM)** for auto-generated insights.

### **3️⃣ Frontend Dashboard (React)**
- Displays **interactive reports and charts**.
- Allows users to **ask AI questions** about data.

## 🛠️ Technologies Used
| Component | Technologies |
|-----------|-------------|
| **Frontend** | React, Tailwind CSS |
| **Backend API** | FastAPI, Python, OAuth2, BigQuery SDK |
| **Database** | Google BigQuery |
| **ETL Pipeline** | Apache Airflow, dbt, PySpark |
| **AI Integration** | OpenAI / Vertex AI for chatbot insights |

## 🔧 Setup Guide
### **1️⃣ Clone Repository**
```bash
git clone https://github.com/yourusername/reporting-assistant.git
cd reporting-assistant
```

### **2️⃣ Backend Setup**
```bash
cd backend
python -m venv venv
source venv/bin/activate  # On Windows use `venv\Scripts\activate`
pip install -r requirements.txt
uvicorn main:app --reload
```

### **3️⃣ Frontend Setup**
```bash
cd frontend
npm install
npm run dev
```

### **4️⃣ Deploying to Google Cloud**
- **BigQuery:** Set up a dataset and load initial data.
- **Cloud Run / GKE:** Deploy backend API.
- **Vercel / Firebase Hosting:** Deploy frontend dashboard.

## 📊 Usage
1️⃣ Upload data via **Google Sheets or API**.  
2️⃣ Run **ETL pipeline (Airflow/dbt)** to update BigQuery.  
3️⃣ Use the **frontend dashboard** to visualize reports.  
4️⃣ Ask the **AI chatbot** for automated insights.  

## 📜 License
MIT License - Open for contributions!
