# Personal AI Memory System (Local RAG)

A **local, privacy-first AI memory system** that stores and retrieves knowledge from **personal notes, PDFs, and chat history** using **Retrieval-Augmented Generation (RAG)**.  
All processing happens **locally**, with **no cloud dependency**, enabling secure and intelligent question answering over your own data.



## 🚀 Key Features

- 🔒 100% **local & privacy-focused** (offline capable)
- 📝 Ingests **notes, PDFs, and chat logs**
- 🧠 Retrieval-Augmented Generation (RAG) pipeline
- 🔎 Semantic search using local embeddings
- 📚 Vector database for long-term memory
- ✨ Intelligent answer generation with source context
- 🧩 Modular, extensible architecture
- 🧪 Test-friendly & research-ready



## 🧠 What Is Local RAG?

Retrieval-Augmented Generation combines:
1. **Retrieval** – find relevant chunks from your personal knowledge base  
2. **Generation** – use those chunks to generate accurate, grounded answers  

This project runs **fully locally**, making it ideal for:
- Personal knowledge management
- Private research notes
- Offline AI assistants



## 🧠 System Workflow

```
Notes / PDFs / Chats
        ↓
Text Cleaning & Chunking
        ↓
Local Embeddings
        ↓
Vector Store (FAISS)
        ↓
Similarity Retrieval
        ↓
Prompt Construction
        ↓
Local LLM Answer Generation
        ↓
Private, Cited Answer
```



## 📁 Project Structure

```
personal-ai-memory-local-rag/
├── app/
│   ├── ingestion/        # Load notes, PDFs, chats
│   ├── preprocessing/   # Cleaning, chunking, metadata
│   ├── embeddings/      # Local embeddings & vector store
│   ├── retrieval/       # Similarity search & reranking
│   ├── generation/      # Prompting & answer generation
│   ├── memory/          # Memory lifecycle management
│   ├── output/          # Answer formatting & citations
│   ├── utils/           # Helpers & validators
│   └── schemas/         # Data models
├── config/              # App, embedding & retrieval configs
├── data/                # Raw data, vectors & memory
├── scripts/             # Ingest, ask, reset memory
├── tests/               # Unit tests
└── docs/                # Architecture & examples
```



## 🛠️ Tech Stack

- **Language:** Python  
- **Embeddings:** Local vector embeddings  
- **Vector Store:** FAISS  
- **Document Parsing:** PyPDF2  
- **ML / Data:** NumPy, Scikit-learn  
- **Validation:** Pydantic  



## ⚙️ Installation

```bash
pip install -r requirements.txt
```



## ▶️ Usage

### 1️⃣ Ingest Data into Memory
```bash
python scripts/ingest.py
```

### 2️⃣ Ask Questions
```bash
python scripts/ask.py
```

Example:
```
Ask your memory: What did I study yesterday?
```



## 📊 Output

- Context-aware answers grounded in your data
- Retrieved knowledge snippets used for generation
- Fully private responses (no external APIs)

Example:
```
[LOCAL LLM ANSWER]
Based on your notes, you studied Retrieval-Augmented Generation...
```



## 🎯 Use Cases

- Personal knowledge management
- Private research assistant
- Student note-based Q&A
- Offline AI companion
- Secure enterprise knowledge bases

