---
Title: System Architecture

Version: 1.0.0

Status: Draft

Author: Hiwa Majidpour

Technical Lead: OpenAI ChatGPT

Last Updated: YYYY-MM-DD

Classification: Public
---

# System Architecture

Aegis AI follows a modular, service-oriented architecture designed to support AI-assisted space mission analysis through Retrieval-Augmented Generation (RAG), IBM Granite models, and modern web technologies.

The architecture separates presentation, business logic, AI orchestration, and data persistence to improve maintainability, scalability, and extensibility.

## High-Level Components

The system consists of the following logical layers:

- Presentation Layer
- API Layer
- AI Orchestration Layer
- Retrieval Layer
- Knowledge Base
- Data Layer

| Layer | Technology |
|--------|------------|
| Frontend | Next.js + React + TypeScript |
| Styling | Tailwind CSS |
| Backend | FastAPI |
| AI Model | IBM Granite |
| Development | IBM Bob |
| Embedding | Granite Embedding Model |
| Vector Database | ChromaDB |
| RAG Framework | LangChain |
| Document Parsing | Docling |
| Database | PostgreSQL |
| Authentication | JWT |
| Deployment | Docker |

+------------------------+
|      Web Browser       |
+-----------+------------+
            |
            v
+------------------------+
| Next.js Frontend       |
+-----------+------------+
            |
            v
+------------------------+
| FastAPI Backend        |
+-----------+------------+
            |
            +----------------+
            |                |
            v                v
     AI Service         Auth Service
            |
            v
+------------------------+
| LangChain Orchestrator |
+-----------+------------+
            |
            +---------------------+
            |                     |
            v                     v
     ChromaDB              IBM Granite
            |
            v
      Mission Documents

## Design Principles

- Separation of Concerns
- Modular Components
- Scalable Architecture
- AI-first Design
- Explainable AI
- Secure by Design
- API-first Development

## Architectural Goals

- Support Retrieval-Augmented Generation
- Enable scalable document processing
- Provide explainable AI responses
- Ensure maintainability
- Support future cloud deployment

## Future Extensions

- Multi-agent AI
- Satellite telemetry integration
- Real-time anomaly detection
- Multi-language support
- Cloud-native deployment

End of Document