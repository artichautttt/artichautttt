# Hi, I'm Malak Laroussi 👋

**Engineering student at École Mohammadia d'Ingénieurs (EMI) · AI & Data specialization**
**Available for a 6-month final-year internship from January 2027, France or Morocco** in applied AI, LLM engineering, data science or data engineering.

I build AI systems that go beyond the notebook: retrieval pipelines that cite their sources, a verification agent that fact-checks another agent's answers, and models that ship with tests, metrics and evaluation.

---

## 🧠 Core skills

| Area | Tools & techniques |
|---|---|
| **LLM & agents** | LangGraph, CrewAI, RAG (hybrid retrieval, cited synthesis), structured outputs, LLM evaluation |
| **LLM providers** | Anthropic Claude, Groq (LLaMA), Hugging Face (local inference, LoRA fine-tuning experiment) |
| **ML & deep learning** | PyTorch, scikit-learn, CLIP / Vision Transformers, multi-task learning, anomaly detection, probability calibration |
| **Data & retrieval** | ChromaDB, vector search, PostgreSQL, BigQuery, dbt, Airflow, PySpark, pandas |
| **Backend** | Python, FastAPI, Flask, Java / Spring Boot |
| **MLOps & DevOps** | Docker, Kubernetes, Terraform, GitHub Actions, MLflow, Prometheus |
| **Quality** | pytest, mypy (strict), Ruff, CI pipelines |

---

## 🚀 Featured projects

### 📄 [Document Intelligence Platform](https://github.com/artichautttt/document-intelligence-platform)
Multi-agent RAG platform for enterprise documents (financial reports, legal contracts).
- PDF/DOCX ingestion, section-based chunking, hybrid retrieval (dense + BM25) on ChromaDB
- LangGraph pipeline (routing → retrieval → cited synthesis), Anthropic Claude by default
- Optional CrewAI verification agent (off by default): fact-checks the synthesis agent's answers against the sources and triggers a regeneration; tested, and evaluated in one documented run
- LoRA fine-tuning experiment (Qwen2.5-0.5B-Instruct, one run): faithfulness 0.293 → 0.839 and citation precision 0.000 → 0.867 vs the base model, but unjustified refusals 0.043 → 0.370, still below Claude
- Evaluation tracked in MLflow, cost tracking, model tiering, Prometheus metrics
- FastAPI + Docker + CI · 504 automated tests, 90% coverage

`LangGraph` `CrewAI` `RAG` `FastAPI` `ChromaDB` `MLflow`

### 🩺 [AI-Assisted Mammography Reporting](https://github.com/artichautttt/mammo)
Generates structured BI-RADS reports from two mammography views (CC + MLO).
- Multi-task model built on a frozen CLIP ViT-B/16, predicting BI-RADS, ACR density and lesion findings
- Similar-case retrieval (top-5, cosine similarity on 1024-D concatenated CC + MLO embeddings)
- Natural-language PDF report drafted by an LLM (LLaMA via Groq), with a mandatory radiologist-review notice
- Two public datasets merged (MVKL + CBIS-DDSM) · FastAPI backend · Angular frontend

`PyTorch` `CLIP` `Computer Vision` `LLM` `Healthcare AI`

### 🛡️ [Mini-SIEM: Network Intrusion Detection](https://github.com/artichautttt/siem)
Security monitoring platform combining rule-based and ML-based detection.
- 7 detection rules mapped to MITRE ATT&CK, risk scoring, threat intelligence enrichment
- Anomaly detection with Isolation Forest
- Flask API, PostgreSQL, JWT role-based access, real-time Angular dashboard
- Docker, Kubernetes, Terraform (AWS), CI/CD, Trivy security scanning

`scikit-learn` `Anomaly Detection` `MITRE ATT&CK` `Kubernetes` `Terraform`

---

## 🛠️ Data Engineering

### 🚕 [GCP Taxi Pipeline](https://github.com/artichautttt/gcp-taxi-pipeline)
ELT pipeline for NYC Yellow Taxi data on BigQuery Sandbox, at €0, run locally with Docker.
- Raw load into BigQuery, dbt star schema (fact table + 4 dimensions), incremental by month
- Idempotent Airflow 3 DAG: re-running a month gives the same row counts and leaves other months untouched
- 61 dbt data tests; the 41 star-schema tests, including a raw-to-fact reconciliation check, pass on each of the 3 months processed
- PySpark path cross-checked against BigQuery (3,253,304 rows on both sides)
- Least-privilege IAM: dedicated service account, custom role limited to `bigquery.jobs.create`, write access to a single dataset, no JSON key (impersonation)

`BigQuery` `dbt` `Airflow` `PySpark` `GCP IAM`

---

## 📊 Data Science

### 📉 [Telco Customer Churn](https://github.com/artichautttt/telco-churn-ml)
Churn prediction on the IBM Telco sample dataset (7,043 fictional customers).
- 3 models compared in stratified 5-fold cross-validation; logistic regression selected by a documented rule
- Test ROC-AUC 0.842; Platt recalibration keeps the ranking unchanged
- Decision threshold chosen with a cost matrix (assumed costs) instead of 0.5
- FastAPI endpoint serving the recalibrated model and its threshold; CI with Ruff and pytest

`scikit-learn` `SHAP` `BigQuery` `MLflow` `FastAPI`

---

## 📜 Certifications

- IBM RAG and Agentic AI · IBM · 2026
- Google AI Essentials · Google · 2026
- Google Cloud Data Analytics · Google Cloud · 2026
- AWS Educate · Generative AI, ML Foundations, Amazon Bedrock · 2026
- EF SET English Certificate · C2 (72/100) · 2026

---

## 📫 Contact

- **Email:** laroussimalak6@gmail.com
- **LinkedIn:** [linkedin.com/in/malaklaroussi](https://www.linkedin.com/in/malaklaroussi)
- **Open to:** 6-month final-year internship from January 2027 · France or Morocco · Applied AI · LLM Engineering · Data Science · Data Engineering
