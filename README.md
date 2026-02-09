# 🧠 Retrieval-Augmented Generation (RAG) with LangChain, ChromaDB, and Grok API

## 📘 Project Overview
This project demonstrates how to build a **Retrieval-Augmented Generation (RAG)** system using **LangChain**, **ChromaDB**, and **Grok API**.  
The goal is to improve LLM responses by grounding them in **document-based context** (e.g., PDFs or research material).

---

## ⚙️ Workflow Summary
1. **PDF Data Extraction**  
   - Load and split PDF content using `langchain_community.document_loaders`.
   - Clean and preprocess text for embedding.

2. **Vector Embedding & Storage**  
   - Convert text chunks into vector embeddings.
   - Store vectors in **ChromaDB** for efficient retrieval.

3. **User Query Handling**  
   - Convert user input into a vector using the same embedding model.
   - Perform similarity search in the vector database.

4. **Response Generation**  
   - Combine retrieved context with the user query.
   - Pass the prompt to **Grok API (LLM)** to generate a factually grounded response.

---
## 🧩 Tech Stack

| Component | Technology |
|------------|-------------|
| **Framework** | LangChain |
| **Vector Database** | ChromaDB |
| **LLM Provider** | Grok API |
| **Embedding Source** | LangChain Embeddings |
| **Data Source** | PDF Documents |

---

## 🧠 Architecture Overview

```text
PDF → Text Splitter → Embeddings → ChromaDB
                                    ↑
                                   Query → Embedding → Similarity Search → Context → Grok LLM
---
## My own summary of the project :
 Overall i have used my work form KrishNaik Notebook , which made the work so fast and my learning of the basic so easy .....
This RAG which made on GROK api gives a good response ...which reduce the Halucunation ..
There is 2 main steps involved :
      1.injection
      2.retrival
These main steps are main core principal of a RAG 

