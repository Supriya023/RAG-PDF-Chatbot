# RAG-PDF-Chatbot
Java Spring Boot RAG chatbot for academic PDFs using ChromaDB, Ollama, hybrid retrieval (BM25 + Vector Search), and citation-based question answering.

# RAG PDF Chatbot

## Overview

A Java Spring Boot based Retrieval-Augmented Generation (RAG) chatbot that allows users to upload PDF documents and ask questions about their content. The system extracts text from PDFs, stores embeddings in ChromaDB, retrieves relevant information using hybrid retrieval (Vector Search + BM25), and generates answers using Ollama with source citations.

## Features

* PDF upload and processing
* PDF text extraction using Apache PDFBox
* Text chunking and embedding generation
* ChromaDB vector database integration
* Hybrid Retrieval (Vector Search + BM25)
* Citation-based answers
* Local LLM support through Ollama

## Tech Stack

* Java
* Spring Boot
* Maven
* ChromaDB
* Ollama
* Apache PDFBox
* BM25
* HTML/CSS/JavaScript

## How to Run

### Start ChromaDB

```powershell
.\.venv\Scripts\chroma.exe run --path .\chroma_db --host 127.0.0.1 --port 8000
```

### Start Spring Boot Application

```powershell
& ".\.tools\apache-maven-3.9.16\bin\mvn.cmd" -s ".\maven-settings.xml" spring-boot:run
```

### Open Application

http://localhost:8080

## Future Enhancements

* OCR support for scanned PDFs
* User authentication
* Multi-user support
* Advanced citation highlighting
* Cloud deployment support
