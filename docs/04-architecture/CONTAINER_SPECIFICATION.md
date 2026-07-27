---
Title: Container Specification

Document ID: ARCH-SPEC-001

Version: 1.0.0

Status: Draft

Author: Hiwa Majidpour

Technical Lead: OpenAI ChatGPT

Reviewer: Architecture Review Team

Last Updated: 2026-07-27

Classification: Public
---

# Container Specification

## Document Information

| Property | Value |
|----------|-------|
| Project | Aegis AI |
| Document | Container Specification |
| Version | 1.0 |
| Status | Approved |
| Author | Hiwa Majidpour |
| Reviewer | Architecture Review Team |
| Date | 2026-07-27 |

---

# Purpose

This document defines all software containers used in the Aegis AI platform.

The specification serves as the primary reference for:

- System architecture
- Software implementation
- Container Diagram (ARCH-002)
- API development
- Deployment planning
- Future maintenance

---

# Overall Architecture

The system follows a layered architecture.

```
End User

↓

Next.js Frontend

↓

FastAPI Backend

↓

AI Services Layer

↓

Data Layer
```

---

# Container 1 — Frontend

## Name

Frontend Application

## Technology

Next.js

React

TypeScript

Tailwind CSS

## Responsibility

Provides the graphical user interface.

Responsible for:

- Authentication
- Dashboard
- AI Chat
- Mission Planning
- Document Upload
- Visualization
- User Settings

## Interfaces

REST API

HTTPS

## Dependencies

FastAPI Backend

---

# Container 2 — Backend

## Name

Backend API

## Technology

FastAPI

Python

Pydantic

Uvicorn

## Responsibility

Acts as the central orchestrator.

Responsible for:

- Authentication
- API endpoints
- Request validation
- AI orchestration
- Business logic
- Database access

## Interfaces

REST API

JSON

HTTPS

## Dependencies

IBM Granite

LangChain

Docling

PostgreSQL

ChromaDB

---

# Container 3 — IBM Granite

## Name

Granite Foundation Models

## Technology

IBM Granite

watsonx

## Responsibility

Provides Large Language Model capabilities.

Responsible for:

- Text Generation
- Reasoning
- Summarization
- Technical Analysis
- Question Answering

---

# Container 4 — LangChain

## Name

AI Orchestration Layer

## Technology

LangChain

## Responsibility

Coordinates AI workflows.

Responsible for:

- Prompt Templates
- RAG
- Chains
- Agents
- Tool Calling
- Memory

---

# Container 5 — Docling

## Name

Document Processing Service

## Technology

IBM Docling

## Responsibility

Processes uploaded documents.

Responsible for:

- PDF Parsing
- OCR
- Table Extraction
- Image Extraction
- Markdown Conversion

---

# Container 6 — ChromaDB

## Name

Vector Database

## Technology

ChromaDB

## Responsibility

Stores document embeddings.

Responsible for:

- Semantic Search
- Similarity Search
- Vector Storage

---

# Container 7 — PostgreSQL

## Name

Relational Database

## Technology

PostgreSQL

## Responsibility

Stores application data.

Responsible for:

- Users
- Sessions
- Projects
- Missions
- Logs
- Metadata

---

# External Systems

The platform interacts with:

- IBM Granite
- NASA
- ESA
- arXiv

---

# Communication

| Source | Destination | Protocol |
|---------|-------------|----------|
| Browser | Frontend | HTTPS |
| Frontend | Backend | REST |
| Backend | Granite | API |
| Backend | LangChain | Python |
| Backend | Docling | Python |
| Backend | ChromaDB | Python |
| Backend | PostgreSQL | SQL |

---

# Security

The architecture implements:

- HTTPS
- JWT Authentication
- Input Validation
- Secure API Communication
- Environment Variables
- Role-Based Access Control (Future)

---

# Deployment

Containers are designed for Docker deployment.

Future deployment targets include:

- Docker Compose
- Kubernetes
- IBM Cloud
- Azure
- AWS

---

# Related Documents

- ARCH-001 System Context
- ARCH-002 Container Diagram
- ADR Collection

---

**End of Document**