Yash Trivedi
AI-Native Backend Engineer | LinkedIn | GitHub | Email

I am a backend engineer specializing in Go, distributed systems, and AI orchestration. I thrive on building highly concurrent, verifiable infrastructure and maintain a skeptical, practical approach to production AI.


🏗️ Architecture & Deep Dives
1. High-Throughput AI Inference Pipeline
The Problem: Processing massive product feeds using LLMs caused severe memory exhaustion (OOM crashes), synchronous blocking, and constant API rate-limiting, leading to 16+ hour processing times.
The Architecture: I completely re-architected the pipeline in Go. I decoupled operations into separate pods, streamed the data through an SQS async queue with KEDA autoscaling, and built a custom multi-provider token bucket to load-balance across AI models based on real-time capacity.
The Impact: Eliminated blocking, stabilized memory, and dropped processing time for massive feeds from 16 hours down to under 3 hours.
2. Multi-Tenant Agentic Commerce Platform (MCP Server)
The Problem: LLMs cannot natively render rich UI widgets, and they hallucinate when given raw database access to massive product catalogs.
The Architecture: I built a multi-tenant conversational commerce platform using the Model Context Protocol (MCP). The server safely bridges non-deterministic LLMs with deterministic catalogs by forcing the LLM to output standardized, strictly curated tool calls.
The Impact: Clients can now embed an AI shopping assistant on their sites that safely searches live catalogs and returns interactive UI widgets natively into the chat, backed by a 3-layer cross-device session memory system to retain user context without context-window bloat.


💻 Technical Proficiencies
Languages: Go, Python, Java
Systems & Infrastructure: Distributed Systems, Microservices, Async Queues (SQS, Kafka), Event-Driven Architecture, Caching (Redis), KEDA Autoscaling, Docker, AWS (EC2, ECS).
AI Integration: LLM Orchestration, Model Context Protocol (MCP), Agentic Tool Calling, Prompt Engineering, Memory Graphs, Multi-Provider Routing.
Design Patterns: Strategy, Observer (Pub-Sub), Factory, Interface Segregation.


🚀 Professional Experience
Senior Software Engineer | DaVinci Commerce | Jan 2024 - Present

Architect backend infrastructure powering B2B multi-tenant AI shopping assistants.
Design and implement high-throughput Go pipelines and MCP servers for enterprise-grade catalog integration.

Software Engineering Intern | DaVinci Commerce

Assisted in early backend development and infrastructure scaling.


🎓 Education
BITS Pilani

Bachelor's Degree — Electronics and Mathematics



Built with GSD Spirit.
