#  RecrutIA — Intelligent CV Parsing & Candidate Stability Prediction Platform

##  Overview

RecrutIA is an end-to-end AI-powered recruitment platform designed to assist HR professionals in automating CV analysis and predicting candidate long-term stability within an organization.

It combines the power of **Large Language Models (LLMs)** for natural language understanding and **Machine Learning** for predictive analytics — all wrapped in a sleek, premium dark UI.

---

##  Features

| Feature | Description |
|---|---|
|  **Intelligent CV Parsing** | Automatically extracts key information from resumes using Llama 3.3 (Groq API) |
|  **Stability Prediction** | Predicts candidate turnover risk using a trained Random Forest model |
|  **Recruitment Recommendations** | Provides automated hiring recommendations based on parsed data and prediction scores |
|  **Dual Input Modes** | Supports both PDF upload and manual text input |
|  **Premium Dark UI** | Clean, professional Streamlit interface with a modern dark theme |
|  **Bias Detection** | Research on detecting and mitigating algorithmic bias in HR AI models |

---

## 🛠️ Tech Stack

| Tool | Role |
|---|---|
|  Python 3.10+ | Core language |
|  Streamlit | Frontend / UI |
|  Groq API — Llama 3.3 | LLM for CV parsing |
|  Scikit-learn | Random Forest (stability prediction) |
|  Pandas / NumPy | Data processing |
|  PyPDF2 | PDF text extraction |
|  Matplotlib / Seaborn | Data visualization |

---

##  Getting Started

### Prerequisites

- Python >= 3.10
- A Groq API Key → https://console.groq.com

### Installation

```bash
# Clone the repository
git clone https://github.com/SalamaBsd/RecrutIA-Intelligent-CV-Parsing-Candidate-Stability-Prediction-Platform.git

# Navigate to the project folder
cd RecrutIA-Intelligent-CV-Parsing-Candidate-Stability-Prediction-Platform

# Install dependencies
pip install -r requirements.txt
```

### Configuration

Create a `.env` file at the root and add your Groq API key:

```env
GROQ_API_KEY=your_groq_api_key_here
```

### Run the App

```bash
streamlit run app_finale.py
```

```
📂 RecrutIA/
├── 📂 .devcontainer/                → Dev container configuration
├── 📂 code_preprocessing_training/  → Model training & preprocessing scripts
├── 📂 dataset/                      → Training dataset
├── 📂 models/                       → Trained ML models (.pkl)
├── 📄 app_finale.py                 → Main Streamlit application
├── 📄 requirements.txt              → Python dependencies
├── 📄 .gitignore
├── 📊 Prerentation_projet_python.pptx → Project presentation slides
└── 📑 Rapport_Détection_et_mitigation_des_biais_algorithmiques.pdf → Research report
```

##  How It Works

1.  User uploads a CV (PDF) or enters candidate info manually
2.  Llama 3.3 (Groq) parses the resume and extracts structured data
3.  Random Forest model predicts candidate stability score (0–100%)
4.  Platform generates an automated recruitment recommendation

---

##  Research Report

This project is accompanied by a full research report on:

> **"Détection et mitigation des biais algorithmiques dans les modèles de prédiction du turnover des ressources humaines"**
> *(Detection and mitigation of algorithmic bias in HR turnover prediction models)*

The report covers:
- Sources of bias in HR datasets
- Fairness metrics (demographic parity, equalized odds)
- Mitigation strategies (re-sampling, re-weighting, post-processing)

---
