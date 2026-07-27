---
Title: Container Layout Specification

Document ID: ARCH-SPEC-002

Version: 1.0.0

Status: Draft

Author: Hiwa Majidpour

Technical Advisor: OpenAI ChatGPT

Reviewer: Architecture Review Team

Last Updated: 2026-07-27

Classification: Public
---

# Container Layout Specification

## Purpose

This document defines the visual layout standards for the ARCH-002 Container Diagram.

The objective is to ensure consistency across all architecture diagrams throughout the Aegis AI project.

---

# Diagram Standard

Architecture Model

C4 Model

Level

Level 2 – Container Diagram

Diagram ID

ARCH-002

---

# Layout

The diagram follows a top-down architecture.

```
End User

↓

Frontend

↓

Backend

↓

AI Layer

↓

Data Layer
```

---

# Containers

## User

Position

Top Center

Color

Light Blue

Border

#0F62FE

---

## Frontend

Technology

Next.js

Position

Center

Color

IBM Blue

Border

#0F62FE

---

## Backend

Technology

FastAPI

Position

Below Frontend

Color

IBM Blue

Border

#0F62FE

---

## AI Services

Includes

- IBM Granite
- LangChain
- Docling

Position

Right Side

Color

Orange

Border

#FF832B

---

## Databases

Includes

- ChromaDB
- PostgreSQL

Position

Bottom

Color

Green

Border

#24A148

---

## External Knowledge

Includes

- NASA
- ESA
- arXiv

Position

Left Side

Color

Light Gray

Border

#8D8D8D

---

# Connections

Browser → Frontend

Frontend → Backend

Backend → IBM Granite

Backend → LangChain

Backend → Docling

Backend → PostgreSQL

Backend → ChromaDB

Backend → External Knowledge

LangChain → ChromaDB

Docling → ChromaDB

---

# Visual Rules

All containers must have equal width.

All containers must have equal height.

Rounded corners.

No crossing lines.

Orthogonal connectors.

Centered labels.

Consistent spacing.

---

# Typography

Title

20 pt

Container Title

16 pt

Technology

12 pt

Description

11 pt

---

# Export

Required formats

- Draw.io
- SVG
- PNG

---

# Related Documents

ARCH-001

Container Specification

ADR Collection

---

**End of Document**