# Amit Jyala

AI & Data Science graduate (2026). I build AI systems and backend pipelines that work reliably in production, not just in demos.

Currently focused on LLM-powered systems, RAG architectures, and multi-agent orchestration using LangGraph.

---

## Projects

### [retrieval-engine](https://github.com/amits44/retrieval-engine)

A Corrective RAG pipeline that scores retrieved document quality before passing context to the model. If the score is too low, it routes to a live web search fallback via Tavily instead of hallucinating from weak context.

Built by reading the original CRAG paper and LangGraph/ChromaDB docs directly. Full pipeline observability via LangSmith. Iterated through three retrieval strategies (dense, hybrid, reranking) and picked based on measured precision.

**Stack:** Python · LangGraph · ChromaDB · FastAPI · Groq (Llama 3.3 70B) · Tavily · LangSmith · Hugging Face

---

### [retinal-detect](https://github.com/amits44/retinal-detect)

End-to-end medical AI system for detecting retinal diseases from OCT scans. Trained on 1,000+ scans, ~90% accuracy across 4 disease classes. Built with a confidence gating layer (>85% threshold) so unreliable predictions don't reach the output. REST API decoupled from the model layer, model is swappable without touching the contract.

**Stack:** Python · TensorFlow · Node.js · REST APIs · PostgreSQL

---

### [trend-to-video](https://github.com/amits44/Content-factory) *(in progress)*

Multi-agent pipeline that goes from trending topic to published short-form video. Separate LangGraph agents handle trend research (SerpAPI), script generation, voiceover (gTTS), and cross-platform publishing to YouTube and Instagram. Each agent produces structured output the next one consumes, no brittle glue code between steps.

The interesting problem: designing handoff contracts between agents so the pipeline is testable at each stage independently.

**Stack:** Python · LangGraph · FastAPI · SerpAPI · gTTS · Groq

---

## Skills

**Languages:** Python, JavaScript  
**AI / ML:** LangGraph, LangSmith, Hugging Face, ChromaDB, TensorFlow, Scikit-learn, RAG, CRAG, LLMs, Prompt Engineering  
**Backend:** FastAPI, Node.js, Express, REST APIs, Docker  
**Databases:** PostgreSQL, MongoDB, ChromaDB, SQL  
**Frontend:** React, Tailwind CSS, Streamlit  
**Tools:** Git, pytest, LangSmith  

---

## Contact

amitsingjyala@gmail.com | github.com/amits44
