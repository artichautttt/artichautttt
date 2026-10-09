# Hi, I'm Malak Laroussi 👋

**Applied AI Engineer · Multi-Agent Systems & LLM Applications**
Engineering student at École Mohammadia d'Ingénieurs (EMI), Rabat. **Looking for a final-year internship (PFE) in 2027** in applied AI, LLM engineering or multi-agent systems.

I build AI systems that go beyond the notebook: retrieval pipelines that cite their sources, agents that check each other's work, and models that ship with tests, metrics and evaluation.

---

## 🧠 Core skills

| Area | Tools & techniques |
|---|---|
| **LLM & agents** | LangGraph, CrewAI, RAG (hybrid retrieval, cited synthesis), structured outputs, prompt engineering, LLM evaluation |
| **LLM providers** | Anthropic Claude, OpenAI, Mistral, Hugging Face (local inference, LoRA fine-tuning), Groq |
| **ML & deep learning** | PyTorch, scikit-learn, CLIP / Vision Transformers, multi-task learning, anomaly detection |
| **Data & retrieval** | ChromaDB, vector search, PostgreSQL, BigQuery, pandas |
| **Backend** | Python, FastAPI, Flask, Java / Spring Boot |
| **MLOps & DevOps** | Docker, Kubernetes, Terraform, GitHub Actions, MLflow, Prometheus, OpenTelemetry |
| **Quality** | pytest, mypy (strict), Ruff, CI pipelines |

---

## 🚀 Featured projects

### 📄 [Document Intelligence Platform](https://github.com/artichautttt/document-intelligence-platform)
Multi-agent RAG platform for enterprise documents (financial reports, legal contracts).
- PDF/DOCX ingestion, structural chunking, hybrid retrieval on ChromaDB
- LangGraph pipeline (routing → retrieval → cited synthesis) plus a CrewAI verification agent
- Pluggable LLM layer: Claude, OpenAI, Mistral, local Hugging Face models with LoRA fine-tuning
- Evaluation tracked in MLflow, cost tracking, model tiering, Prometheus metrics
- FastAPI + Docker + CI · 186 automated tests

`LangGraph` `CrewAI` `RAG` `FastAPI` `ChromaDB` `MLflow`

### 🩺 [AI-Assisted Mammography Reporting](https://github.com/artichautttt/mammo)
Generates structured BI-RADS reports from two mammography views (CC + MLO).
- Multi-task model built on a frozen CLIP ViT-B/16, predicting BI-RADS, ACR density and lesion findings
- Similar-case retrieval (top-5, cosine similarity on 1024-D embeddings)
- Natural-language PDF report drafted by an LLM (LLaMA via Groq), with a mandatory radiologist-review notice
- Trained on 1,930 merged cases (MVKL + CBIS-DDSM) · FastAPI backend · Angular frontend

`PyTorch` `CLIP` `Computer Vision` `LLM` `Healthcare AI`

### 🛡️ [Mini-SIEM: Network Intrusion Detection](https://github.com/artichautttt/siem)
Security monitoring platform combining rule-based and ML-based detection.
- 5 detection rules mapped to MITRE ATT&CK, risk scoring, threat intelligence enrichment
- Anomaly detection with Isolation Forest
- Flask API, PostgreSQL, JWT role-based access, real-time Angular dashboard
- Docker, Kubernetes, Terraform (AWS), CI/CD, Trivy security scanning

`scikit-learn` `Anomaly Detection` `MITRE ATT&CK` `Kubernetes` `Terraform`

---

## 📜 Certifications

- Generative AI with LLMs · DeepLearning.AI × AWS · 2026
- IBM RAG and Agentic AI · IBM · 2026
- AWS Educate · Generative AI, ML Foundations, Bedrock · 2026

---

## 📫 Contact

- **Email:** laroussimalak6@gmail.com
- **LinkedIn:** [linkedin.com/in/malaklaroussi](https://www.linkedin.com/in/malaklaroussi)
- **Open to:** PFE internship 2027 · Applied AI · LLM Engineering · Multi-Agent Systems
