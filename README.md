
<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E14,25:1E1B4B,50:134E4A,75:5EEAD4,100:A78BFA&height=280&section=header&text=Priyanka%20Asthana&fontSize=70&fontColor=FFFFFF&animation=twinkling&fontAlignY=38&desc=NLP%20%26%20Constrained%20LLM%20Systems%20%7C%20Reliability%20Engineering%20%7C%20Research&descAlignY=57&descSize=19&descColor=5EEAD4"/>

</div>

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=700&size=22&duration=3000&pause=1000&color=A78BFA&center=true&vCenter=true&width=900&height=60&lines=→+I+build+reasoning+systems+at+scale;→+then+I+find+where+they+fail+first;→+patent+holder+%7C+Springer+Nature+reviewer+%7C+ERA:AI+finalist" alt="Research Focus" />

<br/>

<div align="center">

### 🔬 Research Vectors

[![ResearchGate](https://img.shields.io/badge/ResearchGate-Papers-00CCBB?style=for-the-badge&logo=researchgate&logoColor=white)](https://www.researchgate.net)
[![ArXiv](https://img.shields.io/badge/arXiv-Preprints-b31b1b?style=for-the-badge&logo=arxiv&logoColor=white)](https://arxiv.org)
[![Google Scholar](https://img.shields.io/badge/Scholar-Citations-4285F4?style=for-the-badge&logo=google-scholar&logoColor=white)](https://scholar.google.com)
[![Portfolio](https://img.shields.io/badge/Portfolio-Research_Dossier-F0B429?style=for-the-badge&logo=vercel&logoColor=0A0E14)](https://priyankaasthana.github.io)

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000&section=header" />
</div>

## 🎯 Research Statement

```
┌─────────────────────────────────────────────────────────────┐
│  Where do LLM systems fail when confidence ≠ correctness?   │
│  How do we engineer reliability into constrained systems?   │
│  What metrics actually predict real-world failure modes?    │
└─────────────────────────────────────────────────────────────┘
```

I investigate **failure modes in large language models**, specifically in constrained reasoning systems where confident-and-wrong is catastrophic. My work spans:

- **Constrained LLM Engineering**: Semantic parsing → constraint layers → semantic validation
- **NLP Reliability**: Quantifying hallucination, measuring constraint enforcement, predicting failure surfaces
- **Real-World Domains**: Medical diagnostics, emergency logistics, cultural heritage systems
- **Empirical Validation**: Benchmarking embedding models, stress-testing under distributional shift

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 📑 Publications & Patents

<table>
<tr>
<td align="center" width="50%">

### 📜 Under Review
<img src="https://img.shields.io/badge/Springer_Nature-Under_Review-134E4A?style=flat-square&labelColor=0A0E14"/>

</td>
<td align="center" width="50%">

### 🏆 Patent Holder
<img src="https://img.shields.io/badge/202611012869-Published_Mar_2026-A78BFA?style=flat-square&labelColor=0A0E14"/>

</td>
</tr>
</table>

| Project | Status | Focus | Publication |
|---------|--------|-------|-------------|
| **RAKT** — Race Conditions in Emergency Blood Logistics | Under Review | GeoAI + token reservation for real-time allocation conflicts | [Zenodo Preprint](https://doi.org/10.5281/zenodo.18149564) |
| **KashiVani** — Hallucination in Cultural Heritage RAG | Under Review | Embedding model benchmarking via RAGAS metrics | [Zenodo Preprint](https://doi.org/10.5281/zenodo.20399130) |
| **DiagnoseAI** — Constrained Clinical LLM | Patent (Published) | Semantic parsing + constraint enforcement + validation layers | [GitHub](https://github.com/PriyankaAsthana/DiagnoseAI---AI-MEDICAL-DIAGNOSIS-SYSTEM-) |

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 🧪 Case Studies: From Theory to Systems

<div align="center">

### ⚕️ DiagnoseAI: Medical-Grade Constraint Layers
<img src="https://img.shields.io/badge/Patented-Mar_2026-5EEAD4?style=flat-square&labelColor=10151E&logo=patent"/>
<img src="https://img.shields.io/badge/Accuracy-92%25-A78BFA?style=flat-square&labelColor=10151E"/>
<img src="https://img.shields.io/badge/Scenarios_Tested-500%2B-F0B429?style=flat-square&labelColor=10151E"/>

**Problem**: Voice → text → LLM → clinical report. Standard models hallucinate confidently on medical data, risking patient harm.

**Solution**:
```
voice_input
    ↓ [Speech-to-Text Encoder]
semantic_parse
    ↓ [Multi-Agent Orchestration]
constrained_generation
    ↓ [Token-Level Constraint Layer]
validated_output
    ↓ [Clinical Compliance Check]
safe_report
```

**Key Innovation**: Constraint layer prevents generation of unvalidated medical entities.

🔧 **Stack**: LangChain · Multi-Agent · Speech Recognition · Custom Constraint Engine

[View Repository ↗](https://github.com/PriyankaAsthana/DiagnoseAI---AI-MEDICAL-DIAGNOSIS-SYSTEM-)

---

### 🚑 RAKT: Temporal Consistency in Logistics
<img src="https://img.shields.io/badge/Springer_Nature-Under_Review-134E4A?style=flat-square&labelColor=10151E"/>
<img src="https://img.shields.io/badge/Allocation_Efficiency-100%25-5EEAD4?style=flat-square&labelColor=10151E"/>
<img src="https://img.shields.io/badge/Distance_Reduction-6.6%25-A78BFA?style=flat-square&labelColor=10151E"/>

**Problem**: Emergency blood bank logistics (India's e-Raktkosh) experience concurrent reallocation conflicts. Units marked for delivery get reallocated while in transit → stock mismatches.

**Solution**: Time-bound token reservation protocol
```
REQUEST: blood_unit(type=O-, hospital=Delhi)
    ↓ [K-Means Clustering on GeoAI]
RESERVE: token(unit_id, expiry_timestamp, route_vector)
    ↓ [No concurrent reallocation within TTL]
DELIVER: with_token_validation(unit_id)
```

**Dataset**: Real e-Raktkosh transaction logs, 10,000+ allocation events

🔧 **Stack**: GeoPy · K-Means · Redis (token store) · GIS analysis

[View Preprint ↗](https://doi.org/10.5281/zenodo.18149564)

---

### 📚 KashiVani: Embedding Model Reliability
<img src="https://img.shields.io/badge/1st_Place-Abhyuday_2026-F0B429?style=flat-square&labelColor=10151E"/>
<img src="https://img.shields.io/badge/Hallucination_Reduction-40%25-5EEAD4?style=flat-square&labelColor=10151E"/>
<img src="https://img.shields.io/badge/Competition-National-A78BFA?style=flat-square&labelColor=10151E"/>

**Problem**: Standard RAG on cultural heritage corpus (Varanasi temples) produces plausible-but-false outputs. No systematic approach to embedding model selection.

**Solution**: Benchmark embedding models against RAGAS metrics instead of accuracy alone
```
CORPUS: cultural_heritage_docs(Varanasi, Sanskrit_OCR)
    ↓ [Test 12 embedding models]
METRICS: RAGAS(faithfulness, relevance, coherence, precision)
    ↓ [Rank by failure mode]
SELECT: sentence-transformers/paraphrase-multilingual-mpnet-base-v2
    ↓ [40% hallucination reduction]
VALIDATE: human_annotation(200 samples)
```

**Datasets**: 5,000+ cultural heritage documents, 500+ manual annotations

🔧 **Stack**: FAISS · RAGAS · Sentence-Transformers · Langchain · Ollama

[View Competition ↗](https://kashivani.onrender.com/)

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 💼 Professional Experience

<table>
<tr>
<td width="25%"><b>FEB – JUL 2026</b><br/><sub>NLP Engineer Intern</sub></td>
<td width="75%">

**IIT BHU** — Resolved 20+ live parsing failures across production NLP pipeline.
- **Impact**: +25% reliability on 1,000+ daily text inputs
- **Tech**: Transformer-based parsers, error analysis, constraint validation
- **Output**: Automated failure detection system for domain-specific NLP

</td>
</tr>

<tr>
<td width="25%"><b>DEC 2025 – FEB 2026</b><br/><sub>AI Research Intern</sub></td>
<td width="75%">

**Bharat Space Education Research Centre** — Sensor fusion for Unmanned Aerial Systems.
- **Impact**: −20% trajectory latency across 5 UAS modules
- **Tech**: Kalman filtering, multi-sensor fusion, real-time optimization
- **Contribution**: Flight dynamics simulation + hardware integration

</td>
</tr>

<tr>
<td width="25%"><b>JUL – SEP 2025</b><br/><sub>Business Analyst Intern</sub></td>
<td width="75%">

**Hindalco Industries** (Aditya Birla Group) — Data pipeline optimization.
- **Impact**: −25% manual processing time via Oracle ERP → Tableau automation
- **Tech**: SQL, Oracle, Tableau dashboards, ETL optimization
- **Scale**: 10,000+ daily transactions analyzed

</td>
</tr>
</table>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 🎓 Education & Credentials

<table>
<tr>
<td align="center">

#### 🏫 BTech (Hons) Computer Science & Engineering
**AKTU** · 2022–2026  
**CGPA**: 8.63/10 · **Gold Medalist**

</td>
<td align="center">

#### 🏆 Fellowships & Recognition
**ERA:AI** Technical Track Finalist · Cambridge  
**2x Springer Nature** Papers (Under Review)  
**Azure AI-900 / AI-102** Certified  
**Oracle AI Vector Search** Certified

</td>
</tr>
</table>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 🛠️ Technical Stack

<div align="center">

### Languages & Core
<img src="https://skillicons.dev/icons?i=python,pytorch,tensorflow,sklearn&theme=dark" />

### ML/AI Specialization
```
NLP Pipeline Design    → Transformers, Semantic Parsing, Constraint Enforcement
Vector Databases       → FAISS, Redis, Milvus, ChromaDB
Evaluation Metrics     → RAGAS, BLEU, F1, Embedding Similarity
Logging & Monitoring   → Prometheus, Weights & Biases, Custom Dashboards
```

### Full-Stack
<img src="https://skillicons.dev/icons?i=react,nodejs,docker,git,vscode&theme=dark" />

### Frameworks & Libraries
```
LLM Orchestration      → LangChain, LlamaIndex, Semantic Kernel
ML/Data              → Pandas, NumPy, SciPy, Scikit-Learn
Retrieval Systems    → FAISS, Sentence-Transformers, Dense Passage Retrieval
Analytics            → SQL, Tableau, Plotly, Seaborn
```

### Deployment & Infrastructure
```
Cloud Platforms      → Azure (AI-900/AI-102 Certified), Render, Vercel
Containerization     → Docker, Docker Compose
Version Control      → Git, GitHub, GitHub Actions
CI/CD               → GitHub Actions, Azure Pipelines
```

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 📊 Research Interests

<div align="center">

| Area | Specific Focus |
|------|---|
| **Constrained LLM Systems** | Semantic parsing, constraint layers, validation frameworks |
| **Failure Mode Analysis** | Hallucination quantification, distributional shift, edge cases |
| **Reliability Engineering** | Benchmarking, metrics selection, robustness testing |
| **Domain-Specific NLP** | Medical, legal, cultural heritage systems |
| **Empirical Validation** | Real-world datasets, human annotation, stress testing |
| **GeoAI & Logistics** | Spatial reasoning, temporal consistency, resource allocation |

</div>

---

<div align="center">
<img src="https://capsule-render.vercel.app/api?type=rect&color=0:A78BFA,50:5EEAD4,100:F0B429&height=4&width=1000" />
</div>

## 🔗 Get in Touch

<div align="center">

[![Email](https://img.shields.io/badge/Email-asthanapriyanka829@gmail.com-A78BFA?style=for-the-badge&logo=gmail&logoColor=white)](mailto:asthanapriyanka829@gmail.com)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Priyanka_Asthana-5EEAD4?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/priyanka-asthana-1b9a74250)
[![Research Portfolio](https://img.shields.io/badge/Full_Dossier-Research_Website-F0B429?style=for-the-badge&logo=vercel&logoColor=white)](https://priyankaasthana.github.io)
[![Twitter/X](https://img.shields.io/badge/Twitter-Research_Updates-5EEAD4?style=for-the-badge&logo=x&logoColor=white)](https://twitter.com)

</div>

---

<div align="center">

### 🧬 System Uptime: Since 2022 · Last Updated: 2026

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A0E14,25:1E1B4B,50:134E4A,75:5EEAD4,100:A78BFA&height=150&section=footer&animation=twinkling"/>

</div>

