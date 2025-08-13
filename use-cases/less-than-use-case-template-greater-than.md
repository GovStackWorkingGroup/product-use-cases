---
description: Derived from implementation case in Kenya
---

# EGOV-1 - AI Chatbot for Discoverability of Government Services

## Product Use Case Summary

| ID      | EGOV-1                                                         |
| ------- | -------------------------------------------------------------- |
| Name    | GovBot - AI Chatbot for Discoverability of Government Services |
| Sector  | Digital Government (eGovernment), Public Service Delivery      |
| Version | 1.0                                                            |
| Status  | Published                                                      |

This use case describes the implementation of an AI-powered conversational chatbot designed to improve citizen access to digital government services.&#x20;

{% hint style="info" %}
**Case of Kenya**

The chatbot, built using PydanticAI agents and Retrieval Augmented Generation (RAG), allows users to interact through text in English and Kiswahili. It guides citizens through various digitized services—such as business registration, film permits, and data protection compliance—by leveraging structured data, document repositories, and knowledge bases from government entities.

The chatbot uses the GovStack Building Block Approach and adheres to principles of open-source development, digital public goods (DPGs), data privacy, and responsible AI. It has been developed for pilot collaboration with Kenya's Directorate of Citizen Services (eCitizen), the Kenya ICT Authority, and the Konza Technopolis. The architecture allows for the onboarding of chatbots from Ministries, Departments, and Agencies (MDAs) within the Kenya government by using a reusable open design.

The solution offers multi-channel access via REST API and web interfaces, and is built for reuse across different sectors and institutions. The chatbot integrates vector databases, document processing pipelines, and comprehensive analytics to provide accurate, relevant, and timely information to citizens while tracking usage and performance metrics.

More Information: [Technical Design Document (Google Docs)](https://docs.google.com/document/d/15MoFvdgJflQ2xINYxwxMfRt818R_ZXUx7LmcFtW0_hA/edit?tab=t.0#heading=h.uo603mk0hacp)
{% endhint %}

## Stakeholders

A list of the stakeholders (Kenya specific) that have some engagement with this use case, including how they are involved:

| Citizens (English & Kiswahili speakers)                                       | End users of the chatbot                   |
| ----------------------------------------------------------------------------- | ------------------------------------------ |
| Directorate of Citizen Services (eCitizen)                                    | Government implementation partner          |
| ICTA (ICT Authority)                                                          | Government implementation partner          |
| KoTDA (Konza Technopolis Development Authority)                               | Government implementation partner          |
| GIZ FAIR Forward & GiZ Kenya - Digital Transformation Center (DTC) & GovStack | Technical and financial support partner    |
| ITU - International Telecommunications Union                                  | Technical Support                          |
| Tech Innovators Network (THiNK) Ltd                                           | Contractor / Developer                     |
| Local AI/NLP community                                                        | Knowledge transfer and model contributions |
| Government MDAs                                                               | Content providers and service owners       |

## Sustainable Development Goals (SDGs)

* Goal 9.C – Significantly increase access to information and communications technology and strive to provide universal and affordable access to the Internet.
* Goal 16.6 – Develop effective, accountable and transparent institutions at all levels.
* Goal 17.6 – Enhance cooperation on and access to science, technology, and innovation.

## Building Blocks

* Information Mediator
* Identity
* Consent
* Messaging
* Workflow
* Registration
* Registry

## Source Documents

* [GovStack Building Block Specifications](https://specs.govstack.global/)
* [Kenya Data Protection Act](https://kenyalaw.org/kl/fileadmin/pdfdownloads/LegalNotices/2021/LN263_2021.pdf)

## Preconditions / Triggers

* Citizen must initiate a service-related query through any supported channel (USSD, webchat, SMS, WhatsApp, voice)
* Internet or network access must be available depending on the channel

## Steps

### 1 - User Inquiry Initiation

A citizen initiates a query to the chatbot through text, asking for guidance on accessing a government service (e.g., "How do I register a business?").

**Workflows**

* Receives user message (SMS, web, WhatsApp)
* Identify if user is registered; optionally prompt for sign-in

**Building Blocks**

* Messaging
* Identity
* Registration

### 2 - Intent & Entity Extraction

The chatbot uses specialized AI agents to determine the intent (e.g., "business registration") and extract relevant entities (location, service type).

**Workflows**

* AI agent processes user message with type-safe validation
* RAG pipeline queries ChromaDB vector database for relevant document chunks
* LlamaIndex retrieval system assembles context from multiple government collections

**Building Blocks**

* Workflow (PydanticAI orchestration)
* Registry (ChromaDB vector storage)
* Information Mediator (RAG pipeline integration)

### 3 - Service Discovery and Information Retrieval

The bot retrieves relevant service information from indexed document collections and web-crawled content via the RAG system.

**Workflows**

* ChromaDB semantic search across indexed government documents and webpages
* Content retrieved from collections including KFC, BRS, KFCB, and ODPC knowledge bases
* MinIO object storage provides document access with presigned URLs

**Building Blocks**

* Information Mediator (Document and webpage retrieval)
* Workflow (Multi-source content aggregation)
* Consent (Data access permissions via collection management)

### 4 - Response Generation & User Guidance

Chatbot returns a human-like conversational response, with source attribution and confidence scoring.

**Workflows**

* LLM processes retrieved context to generate comprehensive answers
* Response includes source citations, confidence scores, and recommended follow-up questions
* Message persistence with conversation history maintenance

**Building Blocks**

* Messaging (Structured response delivery)
* Consent (Source attribution and transparency)
* Workflow (Response quality assurance)

### 5 - Feedback and Continuous Learning

The bot asks for feedback (e.g., thumbs up/down) to learn and improve its answers over time.

**Workflows**

* Real-time event tracking via WebSocket and REST API endpoints
* Analytics module captures user demographics, usage patterns, and business metrics
* Comprehensive audit trail system logs all user actions and system operations

**Building Blocks**

* Registry (Analytics and audit logging)
* Workflow (Performance monitoring and optimization)

## Contributors

* Brian Omwenga – Team Lead, Tech Innovators Network (THiNK)
* Nick Mumero - Lead AI Architect, Tech Innovators Network (THiNK)
* Angela Kanyi - DevOps Engineer, Tech Innovators Network (THiNK)
* Paul Ecil - Fullstack Software Engineer, Tech Innovators Network (THiNK)
* Aisha Mohamed Nur – AI/ML Engineer, Tech Innovators Network (THiNK)
* GIZ DTC & FAIR Forward (Kenya)Teams
* eCitizen, ICTA, KoTDA – Pilot Partners
* IndabaX NLP Community – Peer Review and Knowledge Exchange
