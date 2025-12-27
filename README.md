# HireLens 🔍📄  
AI-Powered Resume Analysis & Ranking System

HireLens is a smart resume screening tool that analyzes CVs against job descriptions and assigns a matching score in percentage form (e.g., 78.5%). It also ranks multiple resumes based on relevance, helping recruiters and hiring managers make faster, data-driven decisions.

---

## 🚀 Features

- 📄 Analyze a single CV against a job description
- 📊 Generate match scores in percentage format
- 🏆 Rank multiple CVs based on relevance
- 📂 Supports PDF resume uploads
- ⚡ Fast and lightweight API using FastAPI
- 🤖 Uses semantic similarity with transformer-based embeddings

---

## 🧠 How It Works

1. User provides:
   - Job Description
   - One or more CVs (PDF format)
2. Text is extracted from PDFs
3. Sentence embeddings are generated using transformer models
4. Semantic similarity is calculated
5. CVs are scored and ranked based on relevance

---

## 🛠 Tech Stack

### Backend
- **FastAPI** – REST API framework
- **Python**

### Machine Learning & NLP
- **Sentence Transformers** – semantic text embeddings
- **Scikit-learn** – similarity calculations
- **NumPy** – numerical operations

### PDF Processing
- **pdfplumber** – extract text from resumes

---

## 📦 Dependencies

txt
fastapi==0.126.0
numpy==2.4.0
pdfplumber==0.11.8
scikit_learn==1.8.0
sentence_transformers==5.2.0

▶️ Getting Started
1️⃣ Clone the repository
git clone https://github.com/your-username/hirelens.git
cd hirelens

2️⃣ Install dependencies
pip install -r requirements.txt

3️⃣ Run the application
uvicorn app.main:app --reload
