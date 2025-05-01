# 🧠 Question Answering on Google Privacy Policy using RAG + BART

This project demonstrates how to implement and compare **RAG-based** and **non-RAG** question answering (QA) pipelines using a real-world legal document—**Google's Privacy Policy**. It showcases skills in **text processing**, **embedding generation**, **deep learning model integration**, and **evaluation of NLP pipelines**.

---

## 📂 Project Overview

In this notebook, we:

- Extracted and cleaned text from a legal PDF document using `PyPDF2`.
- Tokenized and chunked the document into meaningful sentence groups using `nltk`.
- Generated dense sentence embeddings using **Sentence-BERT** (`all-MiniLM-L6-v2`).
- Implemented:
  - ✅ A **RAG (Retrieval-Augmented Generation)** pipeline using BART, integrating similarity-based context retrieval.
  - 🚫 A **non-RAG baseline** using BART alone for comparison.
- Evaluated both methods by posing queries and analyzing the quality and relevance of their answers.

---

## 🧰 Technologies & Libraries

- Python
- Jupyter Notebook
- `PyPDF2`, `nltk`, `re`
- `SentenceTransformers` for semantic embeddings
- `transformers` by Hugging Face for BART-based QA
- `sklearn.metrics.pairwise` for cosine similarity

---

## 🧪 Key Concepts Demonstrated

- PDF Text Extraction: Reading and parsing real-world policy documents.
- Text Preprocessing: Sentence tokenization, cleaning, and chunking for better input formatting.
- Embeddings & Semantic Search: Using `Sentence-BERT` to find contextually relevant passages.
- RAG vs Non-RAG: Understanding how retrieval impacts generative models like BART.
- Evaluation: Comparing generated answers to highlight the value of context-aware generation.

---

## 🔍 Sample Use Case

> "What does Google collect from users?"  
The RAG system retrieves the most relevant passage from the document and uses it to generate a context-aware answer, unlike the non-RAG model that attempts to respond without prior context.

---

## 🎯 Why This Matters

This project is an excellent showcase of:

- Retrieval-augmented QA techniques
- Applied transformer-based NLP
- Working with real-world legal text (not synthetic or simplified)
- Model evaluation and comparison skills
