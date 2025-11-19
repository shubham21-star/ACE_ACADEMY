# 📘 AI Handbook Assistant (RAG-Based Project)

## 📌 Project Overview
This project implements a **Retrieval-Augmented Generation (RAG)** pipeline that answers user questions based on a set of provided documents (PDF/TXT).  
Instead of depending only on the LLM, the system retrieves the most relevant document chunks and uses them as **grounded context** to generate accurate responses.

**Goal:** Build a clean, modular, and fully functional RAG assistant using embeddings, vector search, and context-based answer generation.

---

## 🎯 Objective
- Ingest 2–3 documents (PDF or text files)  
- Chunk the text into smaller, meaningful sections  
- Generate vector embeddings using **sentence-transformers**  
- Store embeddings in a simple **NumPy-based vector search** system  
- Retrieve top-k relevant chunks for any query  
- Produce grounded answers using an **LLM (OpenAI API)**  

---

## 🔧 RAG Pipeline Structure

### **1. Document Loading**
Documents are loaded from PDF or TXT format using:
- `PyPDF2` for PDFs  
- Standard file reading for `.txt`  

The extracted text is cleaned and prepared for chunking.

---

### **2. Text Chunking**
Text is divided into smaller blocks for better retrieval.

**Configuration used:**
- Chunk size: **300–400 characters**  
- Overlap: **50–60 characters**  

This prevents loss of continuity while avoiding oversized chunks.

---

### **3. Embedding Generation**
Model used:
A lightweight and fast embedding model.

Every chunk is converted into a **semantic embedding vector**.

---

### **4. Vector Store (NumPy-Based)**
Since FAISS does not install reliably on Windows, the project uses:
- Pure **NumPy cosine similarity search**  
- Zero external dependencies  
- Ideal for small/medium datasets  

This simple vector store allows efficient similarity search.

---

### **5. Retrieval**
For each user query:
1. Convert query → embedding  
2. Compute cosine similarity with all chunk embeddings  
3. Return **top-k (k=3)** most relevant chunks  

These retrieved chunks act as the knowledge base for the final answer.

---

### **6. Response Generation**
The retrieved chunks + user’s query are sent to an LLM (OpenAI API).  
This ensures the responses remain accurate and grounded in the provided documents.

---

## 🧪 Test Queries & Sample Outputs

| Query | Description |
|-------|-------------|
| **“What is a variable in Python?”** | Retrieved from Python basics document; provides grounded explanation. |
| **“Explain git commit?”** | Pulled from Git command notes. |
| **“How do functions work in Python?”** | Combines multiple relevant chunks for a detailed answer. |

Each test query retrieved 2–3 relevant chunks and produced accurate results.

---

## ✅ What Worked Well
- Chunking + embeddings provided highly relevant search results  
- NumPy-based retrieval avoided FAISS installation issues  
- MiniLM embeddings were reliable and fast  
- RAG responses were noticeably more accurate than direct LLM replies  

---

## ⚠️ Challenges Faced
- PDF extraction produced some formatting noise  
- Required manual cleaning for better chunk quality  
- FAISS installation failed on Windows → switched to NumPy retriever  
- Chunk size tuning was needed for optimal performance  

---

## 📂 Deliverables
- **`rag_assistant.ipynb`** – Complete RAG pipeline notebook  
  *(Loading → Chunking → Embedding → Retrieval → Generation → Testing)*  

- **`sample_outputs/`** – Screenshots of at least 3 successful query outputs  

- **`RAG_Report.md`** – Short summary of what worked and key challenges  

---

## 🏁 Conclusion
This project demonstrates a clean and beginner-friendly RAG workflow.  
By combining embeddings, retrieval, and LLM-based generation, the system produces **accurate and context-grounded answers** directly from source documents.

The pipeline is modular, extendable, and serves as a strong foundation for any future document-based AI assistant.

