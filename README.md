# Retrieval-Augmented Generation (RAG) Question Answering System

This project implements a Retrieval-Augmented Generation (RAG) pipeline that combines document retrieval with a Large Language Model (LLM) to generate context-aware answers from custom knowledge sources.

The system retrieves relevant documents using vector similarity search and feeds them into an LLM to generate accurate, grounded responses.

## Features
- Document ingestion and preprocessing
- Text chunking for efficient retrieval
- Embedding generation using transformer models
- Vector database indexing (FAISS / Chroma)
- Semantic similarity search
- Context-aware answer generation using LLM
- Source document reference display
- Interactive query interface

## Technologies Used
- Python
- LangChain
- HuggingFace Transformers / OpenAI API
- FAISS or ChromaDB
- Sentence Transformers
- Pandas
- NumPy

## Methodology
- Load documents (PDF / TXT / CSV)
- Split documents into smaller text chunks
- Generate embeddings for each chunk
- Store embeddings in a vector database
- Convert user query into embedding
- Retrieve top-k relevant chunks using similarity search
- Pass retrieved context + query to LLM
- Generate grounded response

## RAG Pipeline
- Document Loading
- Text Chunking
- Embedding Generation
- Vector Indexing
- Similarity Retrieval
- Context Injection
- LLM Response Generation

## System Flow
User Query
    ↓
Query Embedding
    ↓
Vector Similarity Search
    ↓
Top-K Relevant Chunks
    ↓
LLM with Context
    ↓
Generated Answer

## Results
- Improved factual accuracy compared to standalone LLM
- Reduced hallucination by grounding responses in retrieved context
- Efficient semantic retrieval using vector search

## Project Structure
rag-question-answering/
│
├── documents/
├── embeddings/
├── vector_store/
├── rag_pipeline.py
├── app.py
├── requirements.txt
└── README.md

## How to Run

Install dependencies:

```bash
pip install langchain faiss-cpu chromadb sentence-transformers transformers openai pandas numpy
```

Run the RAG pipeline:

```bash
python rag_pipeline.py
```

Run the interactive application:

```bash
python app.py
```

## Example Query
- "What are the key findings in the uploaded research paper?"
- "Summarize the company's annual revenue growth."
- "Explain the methodology described in section 3."

The system retrieves relevant context and generates an informed response.
