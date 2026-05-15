# Retrieval-Augmented Generation (RAG) Question Answering System

A lightweight end-to-end Retrieval-Augmented Generation (RAG) pipeline for open-domain question answering using Wikipedia retrieval, semantic search, and transformer-based language models.

---

## Live Demo

Streamlit Application:

[Launch RAG QA App](YOUR_STREAMLIT_LINK)

> Note: The demo is hosted temporarily using Streamlit + ngrok on Google Colab.

---

# Project Highlights

- Wikipedia-powered retrieval system
- Dense semantic embeddings using BGE
- FAISS vector similarity search
- Grounded answer generation using FLAN-T5
- Interactive Streamlit web application
- End-to-end RAG pipeline implementation
- Evaluation using EM, F1, and Retrieval Hit Rate

---

# System Architecture

```text
User Question
      ↓
Wikipedia Retrieval
      ↓
Text Chunking
      ↓
BGE Embeddings
      ↓
FAISS Vector Search
      ↓
Top Relevant Chunks
      ↓
FLAN-T5-small
      ↓
Generated Answer
```

---

# Models Used

| Component | Model |
|---|---|
| Embedding Model | BAAI/bge-small-en-v1.5 |
| Generation Model | google/flan-t5-small |
| Vector Store | FAISS |

---

# Technologies

- Python
- HuggingFace Transformers
- Sentence Transformers
- FAISS
- Streamlit
- Wikipedia API
- Google Colab

---

# Evaluation Results

Evaluation performed on a subset of the Natural Questions (NQ) dataset.

| Metric | Score |
|---|---|
| Exact Match (EM) | 0.10 |
| F1 Score | 0.162 |
| Retrieval Hit Rate | 0.34 |

---

# Key Observations

- The system produced grounded factual answers for many open-domain questions.
- Qualitative performance was significantly stronger than Exact Match alone suggested.
- Strict lexical metrics underestimated semantic correctness in generative QA tasks.
- Lightweight deployment constraints influenced model selection and retrieval design.

---

# Example Questions

- Who invented Python programming language?
- Who wrote the Harry Potter series?
- What is the capital of Australia?
- Who discovered penicillin?
- Where is the Great Barrier Reef located?

---

# Streamlit Application

The project includes an interactive Streamlit-based interface that allows users to:
- ask factual questions
- retrieve relevant Wikipedia context
- generate grounded answers in real time

---

# Installation

Install required dependencies:

```bash
pip install \
transformers \
sentence-transformers \
faiss-cpu \
wikipedia \
streamlit \
pandas \
numpy \
tqdm
```

---

# Run Streamlit App

```bash
streamlit run app.py
```

---

# Project Structure

```text
project/
│
├── final_rag_pipeline_notebook.ipynb
├── app.py
├── README.md
└── requirements.txt
```

---

# Challenges Faced

- Lightweight deployment constraints
- Dynamic Wikipedia retrieval variability
- Evaluation mismatch between semantic correctness and Exact Match
- Memory limitations during reranking experiments

---

# Future Improvements

- Larger instruction-tuned LLMs
- Better reranking pipelines
- Hybrid retrieval systems
- Persistent vector databases
- Cloud deployment
- Pre-indexed Wikipedia corpora

---

# Conclusion

This project demonstrates a complete Retrieval-Augmented Generation workflow including:
- semantic retrieval
- dense embeddings
- vector similarity search
- grounded answer generation
- evaluation
- deployment

The final system successfully balances:
- lightweight infrastructure
- qualitative QA performance
- deployment simplicity
- interactive usability

---

# Author

[Your Name]
