<h1 align="center">Hosam Ghareeb</h1>

<h3 align="center">Senior .NET Backend Engineer · Technical Lead, Search &amp; AI Platforms</h3>

<p align="center">
  <b>One engineer. One search engine. Three businesses. Millions of customers.</b>
</p>

<p align="center">
  I am the technical owner, sole creator and maintainer of Jahez Group's AI search platform.<br>
  I started it from an empty repository, wrote 90%+ of its 670+ commits, and I own it end to end.
</p>

<p align="center">
  <a href="mailto:hosamkhaled1001@gmail.com"><img alt="Email me" src="https://img.shields.io/badge/Email_me-D14836?style=for-the-badge&logo=gmail&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/hosam-ghareeb-212133207"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge"></a>
</p>

<div align="center">
<table>
<tr>
<td align="center" width="25%"><h3>1 engine</h3>3 businesses,<br>millions of customers</td>
<td align="center" width="25%"><h3>30,000+</h3>stores and millions<br>of products searched</td>
<td align="center" width="25%"><h3>90%+</h3>of its 670+ commits<br>written by me</td>
<td align="center" width="25%"><h3>15+</h3>relevance signals<br>fused into one ranking</td>
</tr>
<tr>
<td align="center"><h3>~97%</h3>less vector memory,<br>a 32x cut</td>
<td align="center"><h3>&lt; 1 minute</h3>from catalog change<br>to search index</td>
<td align="center"><h3>100+</h3>tests running the real<br>pipeline end to end</td>
<td align="center"><h3>5+ years</h3>building high-scale<br>backend systems</td>
</tr>
</table>
</div>

## The search platform I built from scratch

**Jahez Group** is a Tadawul-listed Saudi technology group with 110+ million orders in 2025. I built its Search Platform from scratch, and it replaced the group's legacy search: one .NET 10 hybrid search engine on Elasticsearch, Qdrant, Cohere and OpenAI, behind three consumer businesses used by millions of customers.

| Business | What it is | What the engine does there |
|:--|:--|:--|
| **Jahez** | Saudi Arabia's leading food-delivery app | Distance-ranked restaurant and grocery discovery |
| **PIK (Jahez Shops)** | The group's e-commerce marketplace | E-commerce product search |
| **Blu Store** | The official store of Al Hilal SFC, Asia's most successful football club | Global catalog search |

One codebase serves all three, and each business keeps its own indexes, quotas and geo rules.

- **Bilingual hybrid search.** Arabic and English across 30,000+ stores and millions of products, fusing 15+ relevance signals with LLM query expansion and geo-aware ranking.
- **A two-phase pipeline.** Weighted Reciprocal Rank Fusion (RRF) over Qdrant and Elasticsearch signals picks the candidate stores. Lexical, fuzzy and semantic product search follows. A quota-driven ranker with 17 result buckets and Gaussian geo-decay orders the results.
- **LLM and NLP.** Two-model OpenAI query expansion with asynchronous revision and caching through Hangfire, Cohere multilingual embeddings, and custom Elasticsearch analyzers for Arabic spelling variants.
- **Vector search and personalization.** Per-tenant Qdrant collections with HNSW and binary quantization that cuts vector memory by about 97% (32x), plus customer-affinity and past-search behavioral signals.
- **An index that stays fresh.** The Workers service I built syncs the catalog into Qdrant and Elasticsearch in under one minute, through 13 recurring Hangfire jobs, idempotent claim-token batches and self-healing recovery.
- **Relevance that can be explained.** A debug-search API explains the score of every result, and 100+ xUnit v3 tests run the real pipeline end to end over in-memory fakes.
- **Delivery.** I release and run the services through the group's existing GitLab CI/CD, Docker, Kubernetes and ArgoCD (GitOps) setup on AWS, Elastic Cloud and Qdrant Cloud.

Built with C#, .NET 10, ASP.NET Core, Clean Architecture and CQRS/MediatR.

In the group's Catalog microservice (.NET 8, EF Core, PostgreSQL) I also shipped Semantic Search V1, then hybrid search with RRF, H3 geospatial indexing and autocomplete, and built its tracker and validation APIs.

## How I work

Design review before code. Test-first fixes. Backward-compatible APIs. I wrote these conventions down for the platform, and I lead it the same way: I make the architecture decisions, review the code, manage the releases and keep the teams around it in sync.

## Before that

**Senior Full Stack Software Engineer · THIQAH, Saudi Arabia** · Oct 2023 – Mar 2025

- Founding team member of the **Saudi Halal Center (SFDA)** platform, the Saudi government platform that issues Halal certificates worldwide. We built it from scratch as a modular monolith on .NET 7 and ABP Framework, with rich Domain-Driven Design, CQRS/MediatR, EF Core, SQL Server and Redis, unit tested with xUnit and NSubstitute.
- Single-handedly designed and built the shared **Camunda 8 workflow-engine NuGet package**: a loosely coupled, extensible library that wraps gRPC and REST communication. It is reused across the company's projects, so teams integrate the workflow engine without rewriting it.
- Contributed to the company's other shared packages alongside building new ones.

**Associate Software Developer · ASSET Technology Group, Egypt** · Jul 2022 – Oct 2023

- **INUPCO**, the Saudi government platform linking hospitals with medical suppliers under the Ministry of Health: founding back-end team member. I owned the shared and integration services and introduced up-to-date .NET practices and libraries.
- Developed Catalog microservice features on an event-driven architecture (Apache Kafka) with Redis/RediSearch, Clean Architecture, rich DDD and CQRS, unit tested with xUnit and Moq.
- **Palm Hills Developments**, one of Egypt's largest real-estate developers: founding team member of its web platform. Built full-stack features with .NET 6 Web API and Angular on Onion Architecture, secured with IdentityServer and JWT.

**Associate Software Developer · National Technology, Egypt** · Jun 2021 – Jun 2022

- Material Management System for medical laboratories: built full-stack features with ASP.NET Web API, Angular and Kendo UI, and fixed production issues.
- Resolved performance issues, improved the user experience and built Telerik reports on Oracle PL/SQL.

## Toolbox

<p align="center">
  <img alt="C#" src="https://img.shields.io/badge/C%23-9B4F96?style=flat-square">
  <img alt=".NET 10" src="https://img.shields.io/badge/.NET_10-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt="ASP.NET Core" src="https://img.shields.io/badge/ASP.NET_Core-512BD4?style=flat-square&logo=dotnet&logoColor=white">
  <img alt="Elasticsearch" src="https://img.shields.io/badge/Elasticsearch-005571?style=flat-square&logo=elasticsearch&logoColor=white">
  <img alt="Qdrant" src="https://img.shields.io/badge/Qdrant-DC244C?style=flat-square&logo=qdrant&logoColor=white">
  <img alt="OpenAI" src="https://img.shields.io/badge/OpenAI-412991?style=flat-square">
  <img alt="Cohere" src="https://img.shields.io/badge/Cohere-39594D?style=flat-square">
  <img alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white">
  <img alt="Redis" src="https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white">
  <img alt="RabbitMQ" src="https://img.shields.io/badge/RabbitMQ-FF6600?style=flat-square&logo=rabbitmq&logoColor=white">
  <img alt="Apache Kafka" src="https://img.shields.io/badge/Apache_Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white">
  <img alt="Camunda 8" src="https://img.shields.io/badge/Camunda_8-FC5D0D?style=flat-square&logo=camunda&logoColor=white">
  <img alt="Docker" src="https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white">
  <img alt="Kubernetes" src="https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white">
  <img alt="Argo CD" src="https://img.shields.io/badge/Argo_CD-EF7B4D?style=flat-square&logo=argo&logoColor=white">
  <img alt="GitLab CI/CD" src="https://img.shields.io/badge/GitLab_CI%2FCD-FC6D26?style=flat-square&logo=gitlab&logoColor=white">
  <img alt="AWS" src="https://img.shields.io/badge/AWS-FF9900?style=flat-square">
  <img alt="Angular" src="https://img.shields.io/badge/Angular-DD0031?style=flat-square&logo=angular&logoColor=white">
  <img alt="TypeScript" src="https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white">
</p>

| Area | What I work with |
|:--|:--|
| **Languages** | C#, TypeScript, JavaScript, SQL, PL/SQL, Java, C++ |
| **Backend** | .NET 10/8/7/6, ASP.NET Core (Web API, Minimal APIs, MVC), Entity Framework Core, MediatR, FluentValidation, AutoMapper, Refit, SignalR, ABP Framework, ASP.NET Identity, IdentityServer, JWT, REST, gRPC, SOAP, OpenAPI (Swagger, Scalar) |
| **Architecture** | Microservices, Event-Driven Architecture, Clean Architecture, Domain-Driven Design (DDD), CQRS, Modular Monolith, Onion Architecture, Multi-Tenancy, Design Patterns, SOLID, OOP, System Design |
| **Search & AI** | Elasticsearch 8, Qdrant, Hybrid, Semantic & Vector Search, Reciprocal Rank Fusion (RRF), Relevance Tuning, Cohere Embeddings, OpenAI LLMs, Prompt Engineering, RediSearch |
| **Data & Messaging** | PostgreSQL (PostGIS, JSONB), SQL Server, Oracle, Redis, RabbitMQ, Apache Kafka, Hangfire, Camunda 8, H3, NetTopologySuite |
| **Cloud** | AWS (RDS, ECR, S3), Elastic Cloud, Qdrant Cloud, IIS |
| **DevOps (working knowledge)** | Docker, Kubernetes, ArgoCD (GitOps), GitLab CI/CD, Azure DevOps |
| **Testing & Observability** | xUnit, FluentAssertions, NSubstitute, Moq, Integration Testing, TDD, Serilog, Seq, Structured Logging |
| **Frontend** | Angular, Kendo UI, Telerik Reporting, HTML5, CSS3, Bootstrap, jQuery |
| **Tools & Practices** | Git, GitLab, GitHub, Jira, Postman, AI-Assisted Development (Claude Code, GitHub Copilot), Agile/Scrum, Code Review, Release Management |

## Education and languages

- **Bachelor of Engineering**, Helwan University, Egypt · 2013 – 2018
- **Full Stack .NET Development Diploma**, Information Technology Institute (ITI), Egypt · Dec 2020 – Apr 2021
- **Languages:** Arabic (native), English (fluent)

## Let's talk

Need search that understands your customers, in Arabic or English, at the scale of millions? I have already built it once, from an empty repository to production. I would like to hear about yours.

Based in Egypt, available worldwide: relocation to any country, or remote.

[hosamkhaled1001@gmail.com](mailto:hosamkhaled1001@gmail.com) · [linkedin.com/in/hosam-ghareeb-212133207](https://www.linkedin.com/in/hosam-ghareeb-212133207)

<sub>My production work lives in private company repositories. This page is where it shows.</sub>
