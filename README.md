# Project: Linear-Doc-RAG (Local Knowledge Retrieval)

## Overview
This project implements a high-performance, **local-first Question-Answering system** built on a **Retrieval-Augmented Generation (RAG)** architecture. Unlike standard AI tools that rely on cloud APIs, this pipeline processes PDF documents entirely on your local machine or private environment.

## Technical Architecture
- **Generative QA Model**: `google/flan-t5-large` - A sequence-to-sequence model that generates natural answers based on retrieved context.
- **Embedding Model**: `sentence-transformers/all-MiniLM-L6-v2` - Transforms raw text into 384-dimensional semantic vectors.
- **Retrieval Engine**: Uses **Cosine Similarity** to match user queries against document embeddings stored as PyTorch tensors.
- **Data Privacy**: Entirely offline execution ensures no sensitive document data leaves the local runtime environment.
