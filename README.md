# 🧠 Conversational RAG System using Groq + HuggingFace Embeddings

This repository implements a **Conversational Retrieval-Augmented Generation (RAG)** system using:

- 🔍 **HuggingFace sentence-transformer embeddings** for document encoding
- 🧠 **LLaMA3** (via **Groq API**) as the LLM
- 📄 **PDF-based document ingestion**
- 💬 Context-aware **conversational question-answering**
- 🧠 Simulated persona: **25-year experienced researcher**
- ⚙️ Built using the **LangChain** framework and **FAISS** for vector search

---

## 📌 Features

- 📚 Upload your PDF and ask natural questions about it
- 💬 Understands follow-up questions using chat history
- 🧠 Responds like a highly experienced domain researcher
- ⚡ Extremely fast generation using Groq’s LLaMA3 backend
- ❌ No OpenAI dependency – uses free HuggingFace embeddings

---

## 🏗️ Architecture

User Query ➝ Condense Prompt (Chat History + Follow-up)
➝ Standalone Question ➝ FAISS Retriever (PDF Chunks)
➝ Groq LLaMA3 ➝ Final Answer
