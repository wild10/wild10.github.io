---
layout: page
title: RAG Chatbot 
description: RAG chatbot agent using Pinecone, openai/ollama for document Q&A.
img: assets/img/projects/rag_preview.png
importance: 1
category: Generative AI 
giscus_comments: false #true
---

## Overview

This project implements an enterprise-grade RAG (Retrieval-Augmented Generation) chatbot that combines large language models with external knowledge bases. The system processes PDF documents, creates semantic embeddings, and provides accurate, context-aware responses by retrieving relevant information before generating answers.

<div class="row justify-content-sm-center g-2">
    <div class="col-sm-6 mt-4 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/B_J-R_X-2JQ" class="rounded z-depth-1" width="100%" height="250" %}
    </div>
    <div class="col-sm-6 mt-4 mt-md-0">
        {% include video.liquid path="https://www.youtube.com/embed/3CC6itsH6Dk" class="rounded z-depth-1" width="100%" height="250" %}
    </div>
</div>

<div class="caption text-center">
    2 videos demo of the RAG Chatbot system testing.
</div>


---

### System Architecture

**Core Components**:
1. **Cloud Storage**: PDF documents storaage in S3 bucket of AWS(cloud storage)
2. **Document Processing**: PDF parsing and intelligent text chunking
3. **Embedding Generation**: Semantic vector representations using OpenAI/Ollama
4. **Vector Storage**: Pinecone cloud database for scalable similarity search
5. **Retrieval System**: Top-K similarity search with metadata filtering
6. **LLM Integration**: LLaMA 3 or GPT-4 for response generation
7. **Prompt Engineering**: Custom prompts for context-aware responses
8. **Interactive UI**: easy to use interface for users to interact with Gradio

**RAG Pipeline**:
<!-- ```
PDF Documents → Text Extraction → Chunking → Embeddings → Pinecone
                                                              ↓
User Query → Embedding → Similarity Search → Context → LLM → Response
``` -->
<div class="row  justify-content-sm-center ">
    <div class="col-sm-6 mt-3 mt-md-0">
        <a href="{{ site.baseurl }}/assets/img/projects/x_rag.png" data-fancybox="project" title="Example Image" class="zoom" >
        {% include figure.liquid path="assets/img/projects/x_rag.png" title="example image" class="img-fluid rounded z-depth-1" %}
        </a>
    </div>
</div>
<div class="caption">
    The general arquitecture diagram of the proposed RAG chatbot system.
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
- <2% hallucination rate (thanks to RAG grounding)

---

### Technology Stack
you can checkout :point_right: my [github](https://github.com/wild10/Rag_ChatbotAI/tree/main) repository for further details, and sorry againt this may be a bit mess and in spanish but it is a demo project used as MVP(minimal viable product).

---

*This project demonstrates expertise in RAG systems, scalable vector databases*Pinecone*, and production AI deployment(using docker + kubernetes), and monitoring of KPIs(key Performance Indicators). For collaboration opportunities or more clarifications, please [contact me](/about/).*