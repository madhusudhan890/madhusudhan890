# Madhu Sudhan Rao

Senior Software Engineer specializing in distributed systems, real-time communication platforms, and AI-native backend infrastructure.

Over the last 4 years, I have designed and built systems ranging from low-latency media ingestion platforms with WebRTC to scalable event-driven backend services handling real-time workloads. More recently, I've been building AI-native backend systems — LangGraph agentic workflows, RAG pipelines with vector databases, and multi-provider LLM orchestration — alongside the real-time and event-driven infrastructure that connects them. My work focuses on solving engineering challenges around concurrency, scalability, observability, and reliability.

## Areas of Interest

- Distributed Systems
- AI Agentic Workflows & RAG
- Real-Time Communication
- Event-Driven Architectures
- High Performance Backend Engineering
- Observability and Monitoring
- Cloud Native Infrastructure

## Current Technology Stack

**Languages**

- Golang
- Python
- TypeScript / JavaScript
- SQL

**AI & LLM**

- LangChain / LangGraph (agentic workflows)
- Retrieval-Augmented Generation (RAG)
- ChromaDB / pgvector (vector databases)
- OpenAI · Gemini · Groq · Anthropic APIs
- Prompt Engineering & Multi-Provider Orchestration
- Faster-Whisper (speech-to-text)

**Backend & Infrastructure**

- FastAPI / Django
- Express Js / Nest Js
- net/http
- Apache Kafka
- Apache Flink
- WebRTC (Pion)
- gRPC
- Docker / Kubernetes
- NATS

**Databases**

- PostgreSQL
- MySQL
- MongoDB
- DynamoDB
- Redis

**Cloud**

- AWS S3
- AWS DynamoDB
- AWS Lambda / EC2

**Observability**

- OpenTelemetry
- SigNoz
- Prometheus

## Featured Engineering Projects

### [Agentic AI Travel Planner — Multi-Agent LangGraph System](https://github.com/madhusudhan890/agentic-travel-planner).

A production-grade travel planning system built on LangGraph's StateGraph, orchestrating 7 specialist agents (flight, hotel, weather, budget, restaurant, visa, currency) in parallel via asyncio.gather, cutting end-to-end planning time from ~35s sequential to ~5s. Features an LLM-as-judge reviewer node that scores draft itineraries and loops back for revision below a quality threshold, a human-in-the-loop approval checkpoint using LangGraph's interrupt()/resume pattern, and a RAG layer (ChromaDB + Gemini embeddings) grounding the planner in a real travel knowledge base. Streams the entire multi-agent pipeline to the UI in real time via Server-Sent Events, with PDF generation and email delivery on completion.

### [Real-Time Media Intelligence Platform](https://github.com/madhusudhan890/media-intelligence-platform)

A Go (Pion WebRTC) media server ingests audio/video frames from browser clients and publishes them to Kafka for downstream processing. Python AI workers run Faster-Whisper transcription and LangGraph-based multi-provider LLM inference (OpenAI, Gemini, Groq, Anthropic), streaming structured meeting insights back to a live dashboard via SSE. Built with Hexagonal Architecture, idempotent Kafka consumers, and end-to-end OpenTelemetry tracing.

### [ChatPDF — Production RAG Document Assistant](https://github.com/madhusudhan890/ChatPDF)

A fully async FastAPI RAG application using ChromaDB and pgvector for retrieval, with a provider-agnostic Factory Pattern supporting both Gemini and OpenAI for LLM inference and embeddings. Includes non-blocking PDF parsing, batch embedding generation, and exponential backoff retry handling — designed as a production system rather than a tutorial clone.

### [Multi-Provider LLM Gateway](https://github.com/madhusudhan890/ai-base-project)

A unified REST gateway that routes chat completion requests across multiple LLM providers (OpenAI, Gemini) using a Strategy/Handler pattern, enabling zero-downtime provider switching via configuration and easy extension to additional providers.

### OpenTelemetry Observability SDK

An internal SDK built on top of OpenTelemetry providing unified trace propagation, structured logging, and custom metrics across Go and Python microservices — integrated with SigNoz for distributed tracing and alerting.

## Engineering Philosophy

I enjoy building systems that remain reliable under scale. My primary interests include reducing latency, improving throughput, designing fault-tolerant architectures, and creating observability-first platforms that are easy to operate and troubleshoot. Lately, that extends to making AI systems — agentic workflows, RAG pipelines, and LLM-integrated services — just as reliable and observable as the infrastructure they run on.

## Currently Exploring

- Multi-Agent Systems & Agentic AI Workflows
- Retrieval-Augmented Generation at Scale
- Large Scale Distributed Systems
- Streaming Data Platforms
- Advanced Kafka Architectures
- Apache Flink Internals
- WebRTC Infrastructure
- Platform Engineering
- Cloud Native Architectures

## Connect

LinkedIn: [linkedin.com/in/madhu-sudhan-rao-korivi](https://www.linkedin.com/in/madhu-sudhan-rao-korivi/)
Email: madhusudhankorivi890@gmail.com
