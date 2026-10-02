A containerized workflow automation pipeline that ingests RSS feeds, summarizes headlines with an LLM, and dispatches daily tech digests using n8n and Docker.

Containerized Deployment: Packaged entirely in Docker Compose with persistent volumes to ensure setup, node definitions, and credentials survive container updates.

Visual Multi-Step Orchestration: Node-based workflow (Trigger → RSS Ingestion → Transformation → LLM Summarization → Output Formatting) demonstrating visual agentic design.

Secure Credential Management: Enforces API authentication using n8n's encrypted secret store instead of inline plain-text keys.

Custom Data Transformation: Custom JavaScript Code nodes aggregate multi-feed RSS outputs into unified LLM prompt structures and format responses for final delivery.
