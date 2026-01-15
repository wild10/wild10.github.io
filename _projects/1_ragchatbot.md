---
layout: page
title: RAG  Chatbot
description: RAG chatbot using Pinecone,openai/ollama for document Q&A.
img: assets/img/projects/rag_preview.png
importance: 1
category: Generative AI 
giscus_comments: false #true
---

## Overview

This project implements an enterprise-grade RAG (Retrieval-Augmented Generation) chatbot that combines large language models with external knowledge bases. The system processes PDF documents, creates semantic embeddings, and provides accurate, context-aware responses by retrieving relevant information before generating answers.

---

### System Architecture

**Core Components**:
1. **Document Processing**: PDF parsing and intelligent text chunking
2. **Embedding Generation**: Semantic vector representations using OpenAI/Ollama
3. **Vector Storage**: Pinecone cloud database for scalable similarity search
4. **Retrieval System**: Top-K similarity search with metadata filtering
5. **LLM Integration**: LLaMA 3 or GPT-4 for response generation

**RAG Pipeline**:
<!-- ```
PDF Documents → Text Extraction → Chunking → Embeddings → Pinecone
                                                              ↓
User Query → Embedding → Similarity Search → Context → LLM → Response
``` -->
<div class="row  justify-content-sm-center ">
    <div class="col-sm mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/x_rag.png" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/x_rag.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
    <div class="col-sm mt-3 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/watch?v=B_J-R_X-2JQ&t=22s" class="img-fluid rounded z-depth-1" %}
    </div>
</div>
---

### Technical Implementation

**Technology Stack**:
- **Vector Database**: Pinecone (1536-dim vectors, cosine similarity)
- **LLM Options**: LLaMA 3 (via Ollama) or GPT-4.1-mini
- **Framework**: LangChain for RAG orchestration
- **Document Processing**: PyMuPDF for PDF text extraction

**Key Features**:
- Multi-document support with cross-document retrieval
- Conversation memory for context-aware interactions
- Source citations linking to specific pages/sections
- Hybrid search with metadata filtering

---

### Deployment

**Infrastructure**:
- FastAPI for REST API
- Docker containerization
- Kubernetes deployment on AWS EKS
- Redis caching for performance optimization

**Performance Metrics**:
- <3 seconds end-to-end response time
- 100+ queries per second throughput
- 99.9% uptime
- <2% hallucination rate (thanks to RAG grounding)

---

<!-- ### Use Cases

- **Document Q&A**: Legal contracts, medical literature, financial reports
- **Knowledge Management**: Internal wikis, product documentation
- **Customer Support**: Automated assistance with company policies
- **Resume Analysis**: CV screening and candidate matching

--- -->

### Technology Stack
you can checkout my [github here](https://github.com/wild10/Rag_ChatbotAI/tree/main) 

---

*This project demonstrates expertise in RAG systems, vector databases, and production AI deployment. For collaboration opportunities, please [contact me](/contact/).*
