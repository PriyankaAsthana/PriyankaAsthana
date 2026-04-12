```
╔══════════════════════════════════════════════════════════════╗
║         why did the model fail? let me find out.            ║
╚══════════════════════════════════════════════════════════════╝
```

# hey, I'm Priyanka 👋

I build AI systems. Then I break them. Then I figure out *why* they broke — and that's the part I care about most.

Final-year BTech CSE (Hons.) @ AKTU | Minor: Robotics | CGPA: 9.01  
Currently: somewhere between "the model works" and "but does it *actually* work?"

---

## the thing that changed everything

I built **DiagnoseAI** — a voice-based symptom checker using constrained LLMs. During testing, it produced an output that was *structurally perfect* and *clinically wrong*. I had no explanation.

That one failure changed how I think about every system I build.  
I stopped asking *"does it work?"* and started asking *"why does it fail?"*

Every project since has been an answer to that question.

---

## what I'm building

<table>
<tr>
<td width="50%" valign="top">

### 🩸 [RAKT](https://github.com/PriyankaAsthana/RAKT_Blood_Bank_Management)
**Spatial-Temporal GeoAI · Blood Allocation**

Blood banks have a race condition problem. When a unit is in transit, nothing stops it from being reallocated to another patient simultaneously. I found this failure, built a token reservation mechanism to fix it, and validated it in simulation.

`Python` `GeoAI` `Priority Clustering` `Token Reservation`

📄 Under review @ Springer Nature  
🔗 [Preprint on Zenodo](https://doi.org/10.5281/zenodo.18149564)

</td>
<td width="50%" valign="top">

### 🗣️ [DiagnoseAI](https://diagnoseai-ai-medical-system.onrender.com/)
**Voice-First · Constrained LLM · Medical NLP**

Speech → semantic parsing → constrained LLM → structured clinical report. The constraint layer is the interesting part — it's what stops the model from hallucinating its way into a dangerous recommendation.

`Python` `NLP Pipelines` `LLM Reasoning` `Speech-to-Text`

🏛️ **Indian Patent No. 202611012869** · Published March 2026  
✅ 92% accuracy · 500+ patient scenarios

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 🏛️ [KashiVani](https://kashivani.onrender.com/)
**Multi-Agent · RAG · Hallucination Reduction**

A knowledge retrieval system for Varanasi's cultural heritage. Standard RAG wasn't enough — the hallucination rate was too high. I had to go deeper into *where* similarity measures break down semantically before the 40% reduction was possible.

`RAG` `Multi-Agent NLP` `LangChain` `Vector Search`

🥇 1st Place · Abhyuday'26 State-Level Techno-Cultural Fest

</td>
<td width="50%" valign="top">

### 📚 [DSA Quest](https://github.com/PriyankaAsthana/PriyankaDSAQuest)
**Java · Algorithms · Clean Notes**

My running repository of DSA solutions and notes in Java. Not glamorous. But graph algorithms and complexity analysis show up in research more than people admit.

`Java` `Algorithms` `Data Structures`

</td>
</tr>
</table>

---

## what I'm actually good at

```python
skills = {
    "research_focus"  : ["hallucination mitigation", "constrained LLM reasoning",
                          "retrieval-augmented generation", "NLP reliability"],
    "ml_stack"        : ["PyTorch", "TensorFlow", "Scikit-learn", "LangChain"],
    "languages"       : ["Python", "Java", "JavaScript"],
    "tools"           : ["Pandas", "NumPy", "OpenCV", "Git"],
    "currently_reading": ["optimal transport for NLP", "geometric ML", 
                           "trustworthy AI systems"]
}
```

---

## where I've been

```
Feb 2026 → now   NLP Engineer Intern · IIT BHU
                 fixed 20+ parsing failures in real-time NLP systems

Dec 2025 → Jan 2026   AI Research Intern · ISRO (Bharat Space Education Research Centre)
                       ML for UAS control · real-time sensor data fusion

Jul 2025 → Aug 2025   IT Intern · Hindalco Industries (Aditya Birla Group)
                       ERP pipeline automation · analytical dashboards
```

---

## output so far

```
📄  1 paper under review  ──  Springer Nature, Journal of Computational Social Science
🔬  1 preprint            ──  doi.org/10.5281/zenodo.18149564
🏛️  1 patent published    ──  Indian Patent No. 202611012869 (March 2026)
🥇  1 competition win     ──  Abhyuday'26, State Level, 1st Place
```

---

## what's next

PhD in NLP or trustworthy AI.  
Specifically: why do language models fail in constrained, high-stakes environments — and what does it take to fix that at a theoretical level, not just an engineering one.

---

<sub>
📬 asthanapriyanka829@gmail.com &nbsp;·&nbsp;
<a href="https://www.linkedin.com/in/priyanka-asthana-1b9a74250">LinkedIn</a> &nbsp;·&nbsp;
<a href="https://diagnoseai-ai-medical-system.onrender.com/">Portfolio</a>
</sub>

**NLP researcher in progress.** Final-year BTech (Hons.) CSE student at Ashoka Institute of Technology and Management, Varanasi (AKTU) | Minor: Robotics | CGPA: 9.01/10

I build AI systems for healthcare and study why they fail. My work sits at the intersection of constrained LLM reasoning, retrieval-augmented generation, and real-world deployment — specifically how language models break in high-stakes environments and what it takes to make them reliable.

---

## Research Interests

- Hallucination detection and mitigation in large language models
- Retrieval-Augmented Generation (RAG) for knowledge-grounded systems
- Constrained reasoning in NLP pipelines
- AI reliability and trustworthiness in healthcare applications
- Spatial-temporal decision systems

---

## Projects

### [DiagnoseAI — Voice-Based Medical Symptom Assessment](https://diagnoseai-ai-medical-system.onrender.com/)
A voice-first NLP system integrating speech-to-text, semantic parsing, and a constrained LLM pipeline for real-time symptom assessment. Tested on 500+ patient scenarios with 92% accuracy. The system's failure — a structurally valid but clinically incorrect output — redirected my entire research focus toward understanding *why* language models fail.

**→ Indian Patent No. 202611012869, published March 2026**

---

### [RAKT — Spatial-Temporal GeoAI Blood Allocation Framework](https://github.com/PriyankaAsthana/RAKT_Blood_Bank_Management)
Designed a priority-weighted spatial-temporal decision model for emergency blood allocation. The core contribution is a time-bound token reservation mechanism that prevents concurrent reallocation of blood units in transit — a failure mode I identified in existing systems independently. Achieved 100% high-priority allocation and 6.6% distance reduction in scarcity simulations.

**→ Manuscript under review at Springer Nature (Journal of Computational Social Science)**  
**→ Preprint: [doi.org/10.5281/zenodo.18149564](https://doi.org/10.5281/zenodo.18149564)**

---

### [KashiVani — Multi-Agent RAG System for Cultural Knowledge](https://kashivani.onrender.com/)
A multi-agent NLP system for culturally grounded knowledge generation about Varanasi's heritage. Built a custom RAG pipeline that reduced hallucinations by 40% compared to baseline — achieved only after identifying the exact points where standard similarity measures failed to capture semantic accuracy.

**→ 1st Place, Project Presentation — Abhyuday'26 State-Level Techno-Cultural Fest**

---

## Publications & Patents

| Type | Title | Status |
|------|-------|--------|
| Journal Paper | Priority-Weighted Spatial Framework for Emergency Blood Allocation | Under review, Springer Nature |
| Preprint | Same | [Zenodo, 2026](https://doi.org/10.5281/zenodo.18149564) |
| Patent | AI-Driven Conversational Medical Voice Assistant | Published, March 2026 (No. 202611012869) |

---

## Experience

**AI Intern (NLP Engineer) — IIT BHU** *(Feb 2026 – Mar 2026)*  
NLP-driven test automation; resolved 20+ parsing failures in real-time systems.

**AI Research Intern — Bharat Space Education Research Centre (ISRO)** *(Dec 2025 – Jan 2026)*  
AI-driven control algorithms for UAS; ML applied to real-time sensor data fusion.

**IT Intern — Hindalco Industries, Aditya Birla Group** *(Jul 2025 – Aug 2025)*  
Analytical dashboards and ERP data pipeline automation.

---

## Technical Skills

**AI/ML:** PyTorch, TensorFlow, Scikit-learn, LangChain, RAG frameworks, constrained LLM reasoning  
**NLP:** Text processing pipelines, semantic parsing, hallucination mitigation, multi-agent systems  
**Programming:** Python, Java, JavaScript  
**Tools:** Pandas, NumPy, OpenCV, Git

---

## Certifications

- Microsoft Azure AI-102 — Designing and Implementing AI Solutions
- Microsoft Azure AI-900 — AI Fundamentals
- Oracle AI Vector Search Professional (2025)
- McKinsey Forward Program (2025)

---

## Contact

[asthanapriyanka829@gmail.com](mailto:asthanapriyanka829@gmail.com) · [LinkedIn](https://www.linkedin.com/in/priyanka-asthana-1b9a74250) · [Portfolio](https://diagnoseai-ai-medical-system.onrender.com/)

---

*Long-term goal: PhD in NLP / trustworthy AI.*
