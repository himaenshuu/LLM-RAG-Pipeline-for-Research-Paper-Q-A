
# Implemented LLM RAG Pipeline for Research Paper Q&A using LangChain, Gemini, Grobid & Qdrant

This project demonstrates a cutting-edge Retrieval Augmented Generation (RAG) pipeline that seamlessly integrates advanced language models with both web and academic document retrieval. By combining state-of-the-art LLMs (Google Gemini) with robust vector search (Qdrant, Chroma), this solution enables context-aware, accurate, and up-to-date responses to user queries—making it ideal for research, education, and enterprise knowledge management.

---

## Overview

## Retrieval Augmented Generation (RAG)

Retrieval Augmented Generation (RAG) is a powerful technique that enhances language models by combining them with external knowledge bases. RAG addresses a key limitation of models: models rely on fixed training datasets, which can lead to outdated or incomplete information. When given a query, RAG systems first search a knowledge base for relevant information. The system then incorporates this retrieved information into the model's prompt. The model uses the provided context to generate a response to the query. By bridging the gap between vast language models and dynamic, targeted information retrieval, RAG is a powerful technique for building more capable and reliable AI systems.

## GROBID

GROBID is a machine learning library for extracting, parsing, and re-structuring raw documents.

It is designed and expected to be used to parse academic papers, where it works particularly well. Note: if the articles supplied to Grobid are large documents (e.g. dissertations) exceeding a certain number of elements, they might not be processed.

[GROBID Docker Documentation](https://grobid.readthedocs.io/en/latest/Grobid-docker/)

## Why This Project Stands Out

- **End-to-End RAG Pipeline**: From raw data ingestion (web, PDF, academic papers) to semantic search and LLM-powered answer generation, the workflow is fully automated and modular.
- **Multi-Source Knowledge Integration**: Supports both web scraping (Wikipedia, etc.) and academic PDF parsing (with GROBID), ensuring comprehensive and authoritative context.
- **Modern Embedding & Vector Search**: Utilizes Google Generative AI Embeddings and Qdrant/Chroma vector stores for fast, scalable, and accurate semantic retrieval.
- **Production-Ready Design**: Asynchronous PDF processing, robust error handling, and environment-based configuration make this solution ready for real-world deployment.
- **Clean, Modular Code**: The codebase is organized in Jupyter Notebook format for transparency, reproducibility, and easy experimentation.
- **Human-Centric Output**: Includes advanced response cleaning and formatting for clear, professional answers.

---

## Key Features

- **Web Knowledge Ingestion**: Scrapes and indexes web articles using `langchain_community` loaders.
- **Academic Paper Parsing**: Extracts structured content from PDFs using GROBID, enabling deep research insights.
- **Semantic Chunking**: Splits documents into context-rich chunks for precise retrieval.
- **Vector Database Integration**: Stores embeddings in Qdrant or Chroma for scalable similarity search.
- **LLM-Powered Q&A**: Uses Google Gemini (via LangChain) to generate answers grounded in retrieved context.
- **Interactive & Automated Modes**: Supports both user-driven queries and programmatic workflows.

---

## Example Use Cases

- **Academic Research**: Instantly answer complex questions using both the latest web sources and peer-reviewed papers.
- **Enterprise Knowledge Base**: Build intelligent assistants that combine internal documents with external knowledge.
- **Education**: Provide students with context-aware, up-to-date answers sourced from trusted materials.

---

## How It Works

1. **Setup**: Install dependencies and configure API keys in `.env`.
2. **Ingestion**: Load web pages or academic PDFs; parse and split into semantic chunks.
3. **Embedding & Indexing**: Generate embeddings and store in a vector database.
4. **Query**: User submits a question; the system retrieves relevant chunks.
5. **LLM Generation**: Gemini LLM generates a grounded answer using the retrieved context.
6. **Output**: Clean, human-readable response is displayed.

---

## Technologies Used

- **LangChain**: Orchestrates the RAG pipeline.
- **Google Gemini**: State-of-the-art LLM for answer generation.
- **Qdrant / Chroma**: High-performance vector databases for semantic search.
- **GROBID**: ML-based PDF parser for academic papers.
- **Python, Jupyter Notebook**: For modular, reproducible code.

---

## 🤷‍♀️Why You Should Care

- **Demonstrates Mastery of Modern AI Stack**: Integrates LLMs, embeddings, vector search, and document parsing.
- **Real-World Impact**: Solves practical problems in research, education, and enterprise knowledge management.
- **Scalable & Adaptable**: Easily extendable to new data sources, models, or deployment environments.
- **Clean, Professional Code**: Emphasizes best practices, modularity, and maintainability.

---