# 🚀 FinPilot AI

### Autonomous Financial Intelligence & Risk Analytics Platform

FinPilot AI is an end-to-end financial intelligence platform that combines **financial analytics, machine learning, risk detection, explainable AI, Generative AI, Agentic AI, and Retrieval-Augmented Generation (RAG)** into a unified system.

The platform analyzes historical market data, evaluates financial health, forecasts future prices, detects unusual market patterns, explains ML predictions, and allows users to interact with financial intelligence through an AI analyst.

---

## 🎯 Project Objective

FinPilot AI is designed to transform raw financial data into structured, explainable and actionable analytical insights.

The platform focuses on:

- 📊 Financial performance analysis
- 💰 Financial health evaluation
- 🔮 Machine learning forecasting
- ⚠️ Risk and anomaly detection
- 🔍 Explainable AI
- 🤖 Generative AI financial analysis
- 🧠 Agentic AI tool orchestration
- 📚 Financial document intelligence using RAG
- 🖥️ Interactive financial intelligence dashboard

---

## 🧠 Key Features

### 📈 Market Intelligence

Analyzes historical market data using:

- OHLC prices
- Trading volume
- Daily returns
- Moving averages
- Rolling volatility
- Drawdown analysis

---

### 💰 Financial Health Analysis

Evaluates company financial information using:

- Revenue
- Net Income
- Operating Income
- Total Assets
- Equity
- Total Debt
- Current Assets
- Current Liabilities
- Operating Cash Flow
- Free Cash Flow

Derived financial indicators include:

- Net Profit Margin
- Operating Margin
- Return on Assets
- Return on Equity
- Debt-to-Equity
- Current Ratio
- Free Cash Flow Margin
- Revenue Growth

FinPilot also generates a heuristic financial health score across multiple dimensions.

---

### 🔮 ML Forecasting

FinPilot uses machine learning to estimate the next closing price.

Current forecasting model:

**XGBoost Regressor**

Features include:

- Open
- High
- Low
- Close
- Volume
- Daily Return
- Price Change
- MA 7
- MA 30
- MA 50
- MA 200
- Rolling Volatility

Model evaluation includes:

- MAE
- RMSE
- Time-series cross-validation

---

### ⚠️ Risk & Anomaly Detection

FinPilot identifies unusual market behaviour using statistical features and **Isolation Forest**.

Risk signals include:

- Extreme price movements
- High volatility
- Significant drawdowns
- Unusual market patterns
- Anomaly scores

The system distinguishes between normal and potentially unusual observations for further analysis.

---

### 🔍 Explainable AI

FinPilot uses **SHAP (SHapley Additive exPlanations)** to interpret machine-learning predictions.

The XAI layer provides:

- Global feature importance
- Prediction-level explanations
- Positive contributors
- Negative contributors
- Human-readable model explanations

This helps users understand **why the forecasting model produced a particular prediction**.

---

### 🤖 Generative AI Financial Analyst

FinPilot integrates Generative AI to provide natural-language analysis of financial information.

Users can ask questions such as:

> "Analyze the company's financial health."

> "What are the major risk factors?"

> "Explain the latest forecast."

The AI analyst is grounded in available FinPilot data and is instructed not to invent unsupported financial facts.

---

### 🧠 Agentic AI

FinPilot includes an agentic architecture capable of selecting analytical tools based on the user's question.

Available tools include:

- Market Analysis
- Financial Health
- Forecasting
- Risk Analysis
- Explainable AI
- Document Search

The agent follows a:

**Question → Planning → Tool Selection → Tool Execution → AI Response**

workflow.

---

### 📚 RAG Financial Knowledge Base

FinPilot uses Retrieval-Augmented Generation to answer questions from uploaded financial documents.

Pipeline:

```text
Financial Document
        ↓
Text Extraction
        ↓
Text Chunking
        ↓
Sentence Embeddings
        ↓
FAISS Vector Index
        ↓
Semantic Retrieval
        ↓
Gemini AI
        ↓
Grounded Answer


System Architecture:-
                ┌─────────────────────┐
                │   Financial Data    │
                │ Yahoo Finance / PDF  │
                └──────────┬──────────┘
                           │
                           ▼
                ┌─────────────────────┐
                │  Data Engineering   │
                │ Cleaning & Features  │
                └──────────┬──────────┘
                           │
             ┌─────────────┼─────────────┐
             ▼             ▼             ▼
       ┌──────────┐  ┌──────────┐  ┌──────────┐
       │Analytics │  │ ML Model │  │   Risk   │
       │  Engine  │  │ XGBoost  │  │ Detection│
       └────┬─────┘  └────┬─────┘  └────┬─────┘
            │             │             │
            └─────────────┼─────────────┘
                          ▼
                  ┌───────────────┐
                  │ Explainable AI│
                  │     SHAP      │
                  └───────┬───────┘
                          │
             ┌────────────┴────────────┐
             ▼                         ▼
      ┌─────────────┐          ┌─────────────┐
      │ Agentic AI  │          │     RAG     │
      │ Tool System  │          │ FAISS + LLM │
      └──────┬──────┘          └──────┬──────┘
             │                         │
             └───────────┬─────────────┘
                         ▼
                ┌────────────────────┐
                │  GenAI Financial   │
                │      Analyst       │
                └─────────┬──────────┘
                          ▼
                ┌────────────────────┐
                │  Gradio Dashboard  │
                └────────────────────┘


🛠️ Technology Stack
Programming
Python
Data & Analytics
Pandas
NumPy
Matplotlib
Plotly
Financial Data
Yahoo Finance
yfinance
Machine Learning
Scikit-learn
XGBoost
Explainable AI
SHAP
Generative AI
Google Gemini
RAG
PyPDF
Sentence Transformers
FAISS
Dashboard
Gradio
Storage
CSV
JSON
SQLite
Development
Google Colab
Git
GitHub
📁 Project Structure
finpilot-ai/
│
├── data/
│   ├── raw/
│   └── processed/
│
├── models/
│   └── reliance_xgboost_forecaster.pkl
│
├── rag/
│   ├── documents/
│   └── index/
│
├── reports/
│   ├── feature_importance.csv
│   ├── forecast_cv_results.csv
│   ├── latest_forecast.csv
│   ├── genai_financial_context.json
│   └── reliance_financial_analysis.json
│
├── src/
│
└── streamlit_app.py
🔄 FinPilot Development Pipeline
Phase 1  → Data Engineering
Phase 2  → Financial Analytics
Phase 3  → Financial Health
Phase 4  → ML Forecasting
Phase 5  → Risk & Anomaly Detection
Phase 6  → Explainable AI
Phase 7  → GenAI Financial Analyst
Phase 8  → Agentic AI
Phase 9  → RAG
Phase 10 → Interactive Dashboard
Phase 11 → Backend & Database
📊 Current Dataset

The current implementation uses historical market data for:

Reliance Industries Limited

Ticker:

RELIANCE.NS

Historical data analyzed:

2020-01-01 → 2026-01-01

The architecture is designed so additional companies and financial documents can be incorporated in future versions.

▶️ Getting Started
1. Clone the repository
git clone https://github.com/Omkar-1710/finpilot-ai.git
cd finpilot-ai
2. Create a virtual environment
python -m venv venv
3. Activate the environment

Windows:

venv\Scripts\activate

Linux / macOS:

source venv/bin/activate
4. Install dependencies
pip install pandas numpy matplotlib seaborn yfinance scikit-learn xgboost plotly shap pypdf sentence-transformers faiss-cpu gradio google-genai
5. Configure Gemini API

Set your API key as an environment variable.

Windows PowerShell:

$env:GEMINI_API_KEY="YOUR_API_KEY"

Do not commit API keys to GitHub.

🖥️ Dashboard

The FinPilot dashboard provides modules for:

Market Intelligence
Financial Health
AI Forecast
Risk & Anomaly Detection
Explainable AI
AI Financial Analyst
Financial Document Search

The dashboard is built using Gradio.

⚠️ Important Disclaimer

FinPilot AI is an analytical and educational technology project.

Forecasts, anomaly scores, financial health scores and generated explanations are model-based analytical outputs and should not be treated as guaranteed predictions or personalized financial, investment, or trading advice.

An anomaly does not automatically indicate fraud, financial misconduct, or a future price decline.

🚀 Future Development

Planned improvements include:

Backend API
Production database
Multi-company analysis
Automated financial reports
Portfolio-level analytics
Real-time data pipelines
Advanced financial risk scoring
Cloud deployment
Automated model monitoring
Expanded financial document knowledge base
👨‍💻 Author

Omkar Wankar

AI & Data Science Engineering

Interests:

Artificial Intelligence
Machine Learning
Data Science
Generative AI
Agentic AI
Financial Analytics
⭐ Project

If you find FinPilot AI interesting, feel free to explore the repository and follow the development.

FinPilot AI — Turning Financial Data into Intelligent Insights.


### Step 2

README editor में यह पूरा content paste करने के बाद नीचे **Commit changes** button दबाना.

Commit message में रहने दो:

```text
Create README.md
