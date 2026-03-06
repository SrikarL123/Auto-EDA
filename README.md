# 🤖 Auto EDA — Agentic AI Pipeline

> Upload a messy CSV and let 3 AI agents automatically clean, analyse, and recommend visualizations for your data.

![Auto EDA Banner](https://img.shields.io/badge/AI-Agentic%20Pipeline-00ff88?style=for-the-badge)
![Node.js](https://img.shields.io/badge/Node.js-Backend-339933?style=for-the-badge&logo=node.js)
![Groq](https://img.shields.io/badge/Groq-LLaMA%203.3-orange?style=for-the-badge)

🔗 **Live Demo:** [https://auto-eda-1.onrender.com/](https://auto-eda-1.onrender.com/)

---

## 💡 What It Does

Most people still do Exploratory Data Analysis by hand. This project automates the entire process using 3 specialized AI agents powered by LLaMA 3.3 via Groq.

You drop in a messy CSV file. The agents handle the rest.

---

## 🧠 The 3 Agents

| Agent | Role |
|-------|------|
| 🧹 **Cleaner Agent** | Identifies missing values, duplicates, wrong data types, and formatting issues — then tells you exactly how to fix them |
| 🔬 **Analyst Agent** | Detects patterns, anomalies, outliers and correlations across your dataset like a senior data scientist |
| 📊 **KPI Expert** | Recommends specific KPIs, chart types, and dashboard layouts for Power BI and Tableau based on your actual data |

---

## 🛠️ Tech Stack

- **Frontend** — Vanilla HTML, CSS, JavaScript
- **Backend** — Node.js + Express
- **AI Model** — LLaMA 3.3 70B via Groq API
- **Security** — API key stored in `.env`, never exposed to frontend

---

## 🚀 Getting Started

### 1. Clone the repo
```bash
git clone https://github.com/yourusername/auto-eda.git
cd auto-eda
```

### 2. Install dependencies
```bash
npm install
```

### 3. Add your Groq API key
Create a `.env` file in the root folder:
```
GROQ_API_KEY=your_groq_api_key_here
```
Get a free API key at [console.groq.com](https://console.groq.com)

### 4. Start the server
```bash
node server.js
```

### 5. Open the app
Go to `http://localhost:3000` in your browser

---

## 📁 Project Structure

```
auto-eda/
├── server.js        # Express backend — handles Groq API calls
├── package.json     # Dependencies
├── .env             # Your API key (never commit this)
└── public/
└── eda_agent.html   # Frontend UI
```

---

## 📊 How To Use

1. Start the server with `node server.js`
2. Open `http://localhost:3000`
3. Upload any messy `.csv` file
4. Click **Run All 3 Agents**
5. Click **View** on each agent card to read the output

---

## 🔒 Security Note

Your Groq API key is stored only in `.env` and never exposed in the frontend code. If you fork or share this project, others need to add their own `.env` file with their own key.

---

⚠️ Note: This app is hosted on Render's free tier. If it hasn't been used for a while, it may take 30-60 seconds to wake up on the first visit. Just wait a moment and try again!

## 📌 Inspired By

This project was inspired by the article [Agentic AI Pipeline to Automate EDA](https://amanxai.com) by Aman Kharwal, extended with a Node.js backend, secure API handling, a KPI Expert agent, and a full web interface.

---

## 🙌 Author

Built by **Srikar Lokai** — feel free to connect on [LinkedIn](https://www.linkedin.com/in/srikar-lokai/)
