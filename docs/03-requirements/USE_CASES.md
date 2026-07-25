---
Title: Use Cases

Version: 1.0.0

Status: Approved

Author: Hiwa Majidpour

Technical Lead: OpenAI ChatGPT

Last Updated: YYYY-MM-DD

Classification: Public
---

# Use Cases

This document describes the interactions between users and the Aegis AI platform.

The use cases define the functional behaviour of the system and serve as the foundation for system architecture, API design, and implementation.

## UC-001 — Ask AI Assistant

### Primary Actor

Mission Planner

### Goal

Receive an AI-generated answer based on mission knowledge.

### Preconditions

- User is authenticated.
- Knowledge base is available.

### Main Flow

1. User opens AI Assistant.
2. User enters a question.
3. System validates the request.
4. RAG retrieves relevant documents.
5. IBM Granite generates the response.
6. References are displayed.
7. Conversation is stored.

### Alternative Flow

- No relevant document found.
- AI requests clarification.

### Postconditions

- Answer displayed.
- Chat saved.

## UC-002 — Upload Technical Document

Primary Actor

Engineer

Goal

Upload a technical report for AI analysis.

Main Flow

1. Upload document.
2. Document validation.
3. Text extraction.
4. Embedding generation.
5. Vector database update.
6. Confirmation message.

## UC-003 — Search Mission Knowledge

Primary Actor

Researcher

Goal

Search mission documentation semantically.

Main Flow

1. Enter keywords.
2. Semantic search.
3. Rank results.
4. Display documents.

## UC-004 — Generate Mission Summary

Primary Actor

Mission Planner

Goal

Generate an executive mission summary.

Main Flow

1. Select mission.
2. AI analyses documents.
3. Summary generated.
4. Export as PDF.

## UC-005 — View Dashboard

Primary Actor

Any User

Goal

Monitor project activity and AI usage.

Main Flow

1. Open dashboard.
2. View statistics.
3. View recent chats.
4. View uploaded documents.

## Diagram

The Use Case Diagram will be added after the system architecture is completed.