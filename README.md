# Advanced RAG Pipelines

A collection of experiments and implementations exploring **Retrieval-Augmented Generation (RAG)** systems, embeddings, vector databases, and agentic retrieval workflows.

The goal of this repository is to understand how modern AI applications retrieve, process, and utilize external knowledge to generate accurate and context-aware responses.

---

## 🚀 Overview

Large Language Models (LLMs) are powerful but have limitations:

- They may not have access to private or updated information
- They can hallucinate without relevant context
- They require high-quality retrieval to generate reliable answers

Retrieval-Augmented Generation (RAG) improves LLM applications by combining retrieval systems with language models.


User Query
|
▼
Retriever
|
▼
Relevant Context
|
▼
LLM
|
▼
Generated Response

This repository explores different approaches to designing and improving RAG pipelines.

---

# 🧠 Concepts Explored

## 1. Document Processing Pipeline

Explored the complete workflow from raw documents to searchable knowledge bases:

- Document loading
- Text splitting
- Chunking strategies
- Embedding generation
- Vector indexing
- Context retrieval

A key learning:

> Retrieval quality directly impacts the quality of the final LLM response.

---

## 2. Vector Databases & Search Systems

Experimented with different retrieval technologies and their trade-offs.

### FAISS

A lightweight similarity search library.

**Advantages:**
- Fast vector similarity search
- Lightweight
- Easy experimentation

**Trade-offs:**
- Persistence requires additional handling
- Metadata filtering needs extra implementation

---

### ChromaDB

A developer-friendly vector database used for rapid RAG prototyping.

Explored:

- Persistent storage
- Embedding management
- Similarity search
- Metadata filtering

---

### Typesense

A search engine supporting:

- Keyword search
- Vector search
- Hybrid search
- Filtering
- Typo tolerance

Explored how traditional search capabilities can complement vector retrieval.

---

# 3. Agentic RAG

Explored retrieval workflows where an AI agent decides:

- Whether retrieval is required
- Which information source to use
- How to use retrieved context

## Traditional RAG


Question
|
Retriever
|
Context
|
LLM
|
Answer

## Agentic RAG


Question
|
AI Agent
|
Decision Making
|
Tools / Retrieval
|
Context
|
LLM
|
Answer

Agentic RAG provides more flexibility for complex AI workflows.

---

# 🛠️ Tech Stack

- Python
- LangChain
- LLM APIs
- Embeddings
- FAISS
- ChromaDB
- Typesense
- Vector Search
- Retrieval Pipelines

---

# 📂 Repository Structure


advanced-rag-pipelines/

├── data/
├── notebooks/
├── embeddings/
├── retrievers/
├── vectorstores/
├── agents/
├── requirements.txt
└── README.md

---

# 📌 Key Learnings

Through these implementations, I explored:

- Designing end-to-end RAG pipelines
- How chunking affects retrieval quality
- How embeddings represent semantic meaning
- Differences between vector search systems
- Retrieval strategies for improving LLM responses
- Agent-based retrieval workflows

---

# 🔮 Future Improvements

Planned additions:

- Advanced RAG evaluation
- Reranking models
- Query rewriting
- Hybrid retrieval pipelines
- Retrieval evaluation metrics
- Production RAG APIs using FastAPI
- Observability with LangSmith

---

## Author

**Saif Mukadam**

AI & Machine Learning Engineer  
GenAI | RAG | Agentic AI | LLM Applications
