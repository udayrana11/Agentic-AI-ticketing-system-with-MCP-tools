# Agentic AI Ticketing System
## Raw Thoughts:

<img width="1307" height="860" alt="Untitled-2025-08-20-1644" src="https://github.com/user-attachments/assets/265d6827-e457-46cb-89e1-656270ba59f3" />

## Production ready with small tweaks:

<img width="446" height="280" alt="Screenshot 2025-08-20 180216" src="https://github.com/user-attachments/assets/573648d9-b7a7-4ffe-8e73-403bae1bf108" />

## Project Overview
Designed and implemented an **AI-powered ticketing system** for IT support, automating ticket triaging, escalation, and human oversight while integrating with enterprise tools.

## Key Features
- **LLM Orchestrator:** Routes user queries to specialized nodes based on priority and task type.
- **RAG Node:** Provides instant answers to frequently asked questions using a vector database and retrieval chain.
- **Notification Node:** Sends updates via email, Slack, and SMS using webhooks and polling mechanisms.
- **Human-in-the-Loop Node:** Escalates high-priority tickets for manual intervention when thresholds are exceeded.
- **MCP Tool Integration:** Connects seamlessly to ServiceNow API and communication tools for read/write operations.
- **Memory Management:** Session caching for cost efficiency and global memory for auditability.

## Technical Highlights
- Node-based architecture with clearly defined input/output JSON schemas.
- React loops for RAG nodes to ensure higher confidence in responses.
- Polling and webhook mechanisms for event-driven and periodic ticket monitoring.
- SLA compliance tracking and automated escalation.

## Summary

**Use case:** IT team struggled with high ticket volumes, delayed responses, and SLA compliance issues.  

**Solution:** Design an AI system to automate ticket triaging, provide instant FAQ responses, escalate high-priority tickets, and include human oversight.  

**Action:** Built an agentic AI ticketing system with an LLM orchestrator routing queries to multiple nodes:
- Classifier for ticket priority
- RAG-powered FAQ responder
- Notification node (webhooks, polling, Slack/email/SMS)
- Human-in-the-loop escalation node  
Integrated MCP tools for ServiceNow API and other communication channels. Implemented session caching for cost efficiency.

**outcome:** Reduced manual ticket handling by **60%**, ensured SLA compliance, and provided full auditability via global memory logging.

## Tech Stack
- **LLM:** OpenAI GPT-4 / Groq MiniLLM  
- **Vector Database:** Pinecone / FAISS  
- **Workflow Orchestration:** LangGraph agentic nodes  
- **Integration:** ServiceNow API, Slack API, Email, SMS  
- **Memory Management:** Global and session memory  
- **Deployment:** AWS EC2 / Lambda, Webhooks, Polling
