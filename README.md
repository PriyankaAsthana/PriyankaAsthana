# Priyanka Asthana

**NLP & Constrained LLM Systems | Reliability Engineering | Research**

---

## 🎯 Research Focus

```
Where do LLM systems fail when confidence ≠ correctness?
How do we engineer reliability into constrained systems?
What metrics actually predict real-world failure modes?
```

I investigate **failure modes in large language models**, specifically in constrained reasoning systems where confident-and-wrong is catastrophic. My work spans constrained LLM engineering, NLP reliability quantification, and empirical validation in real-world domains.

---

## 🔬 Research Vectors

| Platform | Link |
|----------|------|
| **Google Scholar** | https://scholar.google.com/citations?user=_cNMAsEc3DcC |
| **Portfolio** | https://priyankaasthana.github.io |

---

## 📑 Publications & Patents

### Under Review (Springer Nature)
- **RAKT** — Race Conditions in Emergency Blood Logistics
  - GeoAI + token reservation for real-time allocation conflicts
  - [Zenodo Preprint](https://doi.org/10.5281/zenodo.18149564)

- **KashiVani** — Hallucination in Cultural Heritage RAG
  - Embedding model benchmarking via RAGAS metrics
  - [Zenodo Preprint](https://doi.org/10.5281/zenodo.20399130)

### Patent (Published Mar 2026)
- **DiagnoseAI** — Constrained Clinical LLM System
  - Patent ID: 202611012869
  - Semantic parsing + constraint enforcement + validation layers
  - [GitHub Repository](https://github.com/PriyankaAsthana/DiagnoseAI---AI-MEDICAL-DIAGNOSIS-SYSTEM-)

---

## 🧪 Case Studies

### ⚕️ DiagnoseAI: Medical-Grade Constraint Layers

**Status:** Patented (Mar 2026) | **Accuracy:** 92% | **Test Scenarios:** 500+

**Problem:** Voice → text → LLM → clinical report. Standard models hallucinate confidently on medical data, risking patient harm.

**Solution:**
```
voice_input
    ↓
speech_to_text_encoder
    ↓
semantic_parse
    ↓
multi_agent_orchestration
    ↓
constrained_generation
    ↓
token_level_constraint_layer
    ↓
validated_output
    ↓
clinical_compliance_check
    ↓
safe_report
```

**Innovation:** Constraint layer prevents generation of unvalidated medical entities.

**Stack:** LangChain · Multi-Agent Orchestration · Speech Recognition · Custom Constraint Engine

[View Repository →](https://github.com/PriyankaAsthana/DiagnoseAI---AI-MEDICAL-DIAGNOSIS-SYSTEM-)

---

### 🚑 RAKT: Temporal Consistency in Emergency Logistics

**Status:** Under Review (Springer Nature) | **Allocation Efficiency:** 100% | **Distance Reduction:** 6.6%

**Problem:** India's e-Raktkosh (emergency blood bank logistics) experiences concurrent reallocation conflicts. Units marked for delivery get reallocated while in transit → stock mismatches and delivery failures.

**Solution:** Time-bound token reservation protocol

```
REQUEST: blood_unit(type=O-, hospital=Delhi)
    ↓
k_means_clustering_on_geoai
    ↓
RESERVE: token(unit_id, expiry_timestamp, route_vector)
    ↓
no_concurrent_reallocation_within_ttl
    ↓
DELIVER: with_token_validation(unit_id)
```

**Dataset:** Real e-Raktkosh transaction logs (10,000+ allocation events)

**Stack:** GeoPy · K-Means Clustering · Redis (token store) · GIS Analysis

[View Preprint →](https://doi.org/10.5281/zenodo.18149564)

---

### 📚 KashiVani: Embedding Model Reliability

**Status:** 1st Place - Abhyuday'26 | **Hallucination Reduction:** 40% | **Competition:** National

**Problem:** Standard RAG on cultural heritage corpus (Varanasi temples) produces plausible-but-false outputs. No systematic approach to embedding model selection for specialized domains.

**Solution:** Benchmark embedding models against RAGAS metrics (not accuracy alone)

```
CORPUS: cultural_heritage_docs(Varanasi, Sanskrit_OCR)
    ↓
test_12_embedding_models
    ↓
METRICS: RAGAS(faithfulness, relevance, coherence, precision)
    ↓
rank_by_failure_mode
    ↓
SELECT: sentence-transformers/paraphrase-multilingual-mpnet-base-v2
    ↓
hallucination_reduction_40%
    ↓
VALIDATE: human_annotation(200 samples)
```

**Datasets:** 5,000+ cultural heritage documents, 500+ manual annotations

**Stack:** FAISS · RAGAS · Sentence-Transformers · LangChain · Ollama

[View Project →](https://kashivani.onrender.com/)

---

## 💼 Professional Experience

| Period | Role | Organization | Impact |
|--------|------|--------------|--------|
| **FEB – JUL 2026** | NLP Engineer Intern | IIT BHU | Resolved 20+ live parsing failures; +25% pipeline reliability on 1,000+ daily inputs |
| **DEC 2025 – FEB 2026** | AI Research Intern | Bharat Space Education Research Centre | Sensor fusion across 5 UAS modules; −20% trajectory latency |
| **JUL – SEP 2025** | Business Analyst Intern | Hindalco Industries (Aditya Birla Group) | Oracle ERP → Tableau automation; −25% manual processing time |

---

## 🎓 Education & Credentials

**BTech (Hons) Computer Science & Engineering** — AKTU (2022–2026)
- CGPA: 8.63/10 · Gold Medalist

**Fellowships & Recognition**
- ERA:AI Technical Track Finalist (Cambridge)
- 2x Springer Nature Papers (Under Review)
- Azure AI-900 / AI-102 Certified
- Oracle AI Vector Search Certified

---

## 🛠️ Technical Stack

### Core Languages
- Python (primary)
- PyTorch, TensorFlow
- Scikit-Learn

### NLP & ML Specialization
- **LLM Orchestration:** LangChain, LlamaIndex, Semantic Kernel
- **Vector Databases:** FAISS, Redis, Milvus, ChromaDB
- **Evaluation Metrics:** RAGAS, BLEU, F1, Embedding Similarity
- **ML/Data:** Pandas, NumPy, SciPy, Scikit-Learn

### Retrieval & Search
- Sentence-Transformers
- Dense Passage Retrieval
- FAISS indexing

### Deployment & Infrastructure
- **Cloud:** Azure (AI-900/AI-102 Certified), Render, Vercel
- **Containerization:** Docker, Docker Compose
- **CI/CD:** GitHub Actions, Azure Pipelines
- **Analytics:** SQL, Tableau, Plotly, Seaborn

### Frontend & Full-Stack
- React
- Node.js
- Git & GitHub

---

## 📊 Research Interests

| Area | Focus |
|------|-------|
| **Constrained LLM Systems** | Semantic parsing, constraint layers, validation frameworks |
| **Failure Mode Analysis** | Hallucination quantification, distributional shift, edge cases |
| **Reliability Engineering** | Benchmarking, metrics selection, robustness testing |
| **Domain-Specific NLP** | Medical, legal, cultural heritage systems |
| **Empirical Validation** | Real-world datasets, human annotation, stress testing |
| **GeoAI & Logistics** | Spatial reasoning, temporal consistency, resource allocation |

---

## 📡 Connect With Me

- **Email:** [asthanapriyanka829@gmail.com](mailto:asthanapriyanka829@gmail.com)
- **LinkedIn:** [Priyanka Asthana](https://www.linkedin.com/in/priyanka-asthana-1b9a74250)
- **Research Website:** [Full Dossier](https://priyankaasthana.github.io)

---

<div align="center">

**System Uptime: Since 2022 · Last Updated: 2026**

</div>
