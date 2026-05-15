# 🚀 Retrieval-Augmented Generation (RAG) Question Answering System

<p align="center">

![Python](https://img.shields.io/badge/Python-3.10-blue?style=for-the-badge&logo=python)

![Transformers](https://img.shields.io/badge/HuggingFace-Transformers-yellow?style=for-the-badge)

![FAISS](https://img.shields.io/badge/VectorDB-FAISS-green?style=for-the-badge)

![Streamlit](https://img.shields.io/badge/Frontend-Streamlit-red?style=for-the-badge&logo=streamlit)

![Colab](https://img.shields.io/badge/Platform-Google%20Colab-orange?style=for-the-badge&logo=googlecolab)

</p>

---

# 📌 Project Overview

This project implements a lightweight **Retrieval-Augmented Generation (RAG)** pipeline for open-domain question answering using:

- 📚 Wikipedia Retrieval
- 🧠 Dense Semantic Embeddings
- 🔍 FAISS Vector Search
- 🤖 FLAN-T5 Answer Generation
- 🌐 Streamlit Deployment

The system retrieves relevant context from Wikipedia and generates grounded factual answers using transformer-based language models.

---

# 🌐 Live Demo

## 🔗 Streamlit Application

👉 **[Launch RAG QA App](YOUR_STREAMLIT_LINK)**

> ⚠️ Demo is hosted temporarily using Streamlit + ngrok on Google Colab.

---

# ✨ Features

✅ Wikipedia-powered retrieval  
✅ Dense semantic embeddings using BGE  
✅ FAISS vector similarity search  
✅ Grounded answer generation  
✅ Streamlit interactive web app  
✅ End-to-end RAG pipeline  
✅ Evaluation metrics included  

---

# 🏗️ System Architecture

```text
User Question
      ↓
📚 Wikipedia Retrieval
      ↓
✂️ Text Chunking
      ↓
🧠 BGE Embeddings
      ↓
🔍 FAISS Vector Search
      ↓
📄 Top Relevant Chunks
      ↓
🤖 FLAN-T5-base
      ↓
✅ Generated Answer
```

---

# 🤖 Models Used

| Component | Model |
|---|---|
| Embedding Model | `BAAI/bge-small-en-v1.5` |
| Generation Model | `google/flan-t5-base` |
| Vector Database | `FAISS` |

---

# 🛠️ Technologies Used

- Python
- HuggingFace Transformers
- Sentence Transformers
- FAISS
- Streamlit
- Wikipedia API
- Google Colab

---

# 📊 Evaluation Results

Evaluation performed on a subset of the **Natural Questions (NQ)** dataset.

| Metric | Score |
|---|---|
| 🎯 Exact Match (EM) | **0.10** |
| 📈 F1 Score | **0.162** |
| 🔍 Retrieval Hit Rate | **0.34** |

---

# 🧠 Key Observations

- The system produced grounded factual answers for many open-domain questions.
- Qualitative performance was significantly stronger than Exact Match alone suggested.
- Strict lexical metrics underestimated semantic correctness in generative QA tasks.
- Lightweight deployment constraints influenced model selection and retrieval design.

---

# 💬 Example Questions

```text
Who invented Python programming language?

Who wrote the Harry Potter series?

What is the capital of Australia?

Who discovered penicillin?

Where is the Great Barrier Reef located?
```

---

# 🌐 Streamlit Application

The project includes an interactive Streamlit-based interface that allows users to:

- ask factual questions
- retrieve relevant Wikipedia context
- generate grounded answers in real time

---

# ⚙️ Installation

Install dependencies:

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

# ▶️ Run Streamlit App

```bash
streamlit run app.py
```

---

# 📂 Project Structure

```text
project/
│
├── 📓 final_rag_pipeline_notebook.ipynb
├── 🌐 app.py
├── 📄 README.md
└── 📦 requirements.txt
```

---

# 🚧 Challenges Faced

- Lightweight deployment constraints
- Dynamic Wikipedia retrieval variability
- Evaluation mismatch between semantic correctness and Exact Match
- Memory limitations during reranking experiments

---

# 🚀 Future Improvements

- Larger instruction-tuned LLMs
- Better reranking pipelines
- Hybrid retrieval systems
- Persistent vector databases
- Cloud deployment
- Pre-indexed Wikipedia corpora

---

# ✅ Conclusion

This project demonstrates a complete Retrieval-Augmented Generation workflow including:

- semantic retrieval
- dense embeddings
- vector similarity search
- grounded answer generation
- evaluation
- deployment

The final system successfully balances:

✅ lightweight infrastructure  
✅ qualitative QA performance  
✅ deployment simplicity  
✅ interactive usability  

---

# 👨‍💻 Author

**[Jyoti Bhardwaj]**

---

# ⭐ If you found this project useful, consider giving it a star!
