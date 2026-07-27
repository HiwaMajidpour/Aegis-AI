---
Title: System Context

Version: 1.0.0

Status: Draft

Author: Hiwa Majidpour

Technical Lead: OpenAI ChatGPT

Last Updated: YYYY-MM-DD

Classification: Public
---

# System Context

The Aegis AI platform provides an AI-assisted decision support environment for space mission planning, technical document analysis, and scientific knowledge retrieval.

The system integrates modern AI technologies with enterprise software architecture to support engineers, researchers, mission planners, and students.

## External Actors

### Mission Planner

Uses AI for mission planning and operational decision support.

---

### Aerospace Engineer

Uploads technical reports and analyses engineering documents.

---

### Researcher

Searches scientific publications and mission documentation.

---

### Student

Uses the platform for learning and educational purposes.

## External Systems

### IBM Granite

Generates AI responses.

---

### IBM Bob

Primary AI-assisted development platform.

---

### ChromaDB

Stores document embeddings.

---

### PostgreSQL

Stores application data.

---

### NASA / ESA Public Documents

Knowledge source for RAG.

---

### Docling

Extracts text from uploaded documents.

## System Responsibilities

The system shall:

- Answer mission-related questions
- Retrieve relevant knowledge
- Analyse uploaded documents
- Generate AI-assisted summaries
- Provide explainable AI responses
- Store conversations securely

# System Context Diagram

Diagram ID: ARCH-001

Location:

docs/diagrams/ARCH-001-System-Context.drawio

Description

The System Context Diagram illustrates the interaction between users, the Aegis AI platform, and external systems.

External systems include AI models, document processing services, databases, and public space knowledge sources.

The diagram represents the highest level of the software architecture and serves as the foundation for all subsequent architecture diagrams.