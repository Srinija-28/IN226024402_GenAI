# 🧠 AI Resume Screening System with LangChain & LangSmith

## 🚀 Overview

This project implements an **AI-powered Resume Screening System** using **LangChain**.
It evaluates candidates by comparing resumes with a job description and provides:

* ✅ Skill Extraction
* ✅ Matching Analysis
* ✅ Scoring (0–100)
* ✅ Explainable Results
* ✅ Tracing using LangSmith

---

## 🎯 Objective

To build an intelligent system that helps recruiters automatically screen resumes based on job requirements and provide explainable insights.

---

## 🏗️ Pipeline Architecture

Resume → Skill Extraction → Matching → Scoring → Explanation → Tracing

---

## ⚙️ Technologies Used

* 🐍 Python
* 🔗 LangChain
* 📊 LangSmith (Tracing & Debugging)
* 🤖 HuggingFace / OpenAI (LLM)
* 📓 Jupyter Notebook

---

## 🔍 Features

### 1️⃣ Skill Extraction

* Extracts skills, experience, and tools from resume
* Ensures no hallucination

### 2️⃣ Matching Logic

* Compares resume with job description
* Identifies:

  * Matching skills
  * Missing skills

### 3️⃣ Scoring System

* Assigns a score between **0–100**
* Based on skill relevance

### 4️⃣ Explanation

* Provides:

  * Strengths
  * Weaknesses
  * Final reasoning

### 5️⃣ LangSmith Tracing

* Tracks each pipeline step
* Helps debug errors
* Shows run history

---

## ▶️ How to Run

### Step 1: Install Dependencies

```bash
pip install langchain langchain-core langchain-openai langchain-huggingface openai python-dotenv
```

---

### Step 2: Set Environment Variables

```python
import os

os.environ["LANGCHAIN_TRACING_V2"] = "true"
os.environ["LANGCHAIN_API_KEY"] = "your_langsmith_key"
os.environ["LANGCHAIN_PROJECT"] = "resume-screening"
```

(Optional for OpenAI)

```python
os.environ["OPENAI_API_KEY"] = "your_openai_key"
```

(Optional for HuggingFace)

```python
os.environ["HUGGINGFACEHUB_API_TOKEN"] = "your_token"
```

---

### Step 3: Run Notebook

* Open `main.ipynb`
* Run all cells
* Execute pipeline for:

  * Strong candidate
  * Average candidate
  * Weak candidate

---

## 📊 Sample Output

* Extracted skills
* Matching results
* Score (0–100)
* Explanation

---

## 📸 Screenshots

Include:

* LangSmith tracing dashboard
* Output results
* Debug/error case

---

## 🐞 Debug Case

An intentionally weak/incorrect resume is used to test system robustness and debugging.

---

## 📌 Key Learnings

* Built modular LLM pipelines
* Implemented prompt engineering
* Used LangSmith for tracing & debugging
* Developed explainable AI system

---



## 👩‍💻 Author

**Srinija Thippani**

---

## ⭐ Conclusion

This project demonstrates how **GenAI + LangChain** can be used to build real-world AI applications like resume screening systems with explainability and monitoring.

---

