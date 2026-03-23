# 🧠 LLM Text-to-SQL System (SQLite + Fraud Analytics)

## Overview

This project builds a **progressive Text-to-SQL system** using LLMs on a SQLite database.
The goal is not just query generation, but evolving toward a **decision-making data system** with memory, visualization, and ML integration.

---

## 🚀 Project Roadmap

### ✅ Phase 1: Basic Text-to-SQL (Completed)

* Natural Language → SQL generation
* Execution on SQLite (`fraud.db`)
* Handles simple analytical queries

**Example**

* Input: *"Top 5 users by transaction amount"*
* Output: SQL + result

---

### ⚙️ Phase 2: Memory + Visualization (In Progress)

* Context-aware querying (multi-turn memory)
* Retains previous query context
* Auto-visualization of results (charts/plots)
* Improved prompt engineering with schema awareness

---

### 🔥 Phase 3: Tool Calling + ML Integration (Planned)

* LLM decides when to:

  * Generate SQL
  * Call ML model
* Integration with:

  * XGBoost fraud detection model
  * SHAP for explainability
* Hybrid system:

  * Data retrieval (SQL)
  * Prediction (ML)
  * Explanation (SHAP)

---

## 🏗️ Architecture (High-Level)

User Query
↓
LLM (Prompt + Schema Context)
↓
SQL Generation
↓
SQLite Execution
↓
Result

Future:

* Memory Layer
* Visualization Layer
* Tool Calling (ML models)

---

## 🧪 Tech Stack

* Python
* SQLite
* LLM APIs (OpenAI / others)
* Pandas
* Matplotlib / Plotly (planned)
* XGBoost (planned)
* SHAP (planned)

---

## 📂 Project Structure

```
TEXT_TO_SQL/
│── .env.example
│── .gitignore
│── requirements.txt
│── text_to_SQL_basic.ipynb
│── README.md
```

---

## ⚙️ Setup

1. Clone the repository
2. Create `.env` file:

```
OPENAI_API_KEY=your_api_key
```

3. Install dependencies:

```
pip install -r requirements.txt
```

4. Run the notebook:

```
text_to_SQL_basic.ipynb
```

---

## ⚠️ Notes

* `fraud.db` is not included (size constraints)
* Users can plug in their own SQLite database
* Schema-aware prompting improves performance significantly

---

## 🎯 Key Learnings

* LLMs can generate SQL but need guardrails
* Schema context is critical for accuracy
* Memory enables multi-step analytical workflows
* Tool calling bridges analytics + ML decision systems

---

## 🔮 Future Improvements

* Query validation & safety layer
* RAG-based schema retrieval
* Evaluation framework (accuracy, execution success)
* Streamlit / UI interface
* Deployment as API

---

## 👤 Author

Prathik Kundaragi
Data Scientist |Fraud Analytics


