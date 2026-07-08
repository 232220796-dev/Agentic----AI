RIMAS MOHAMMED 
# Capstone Project: Building Agentic AI Systems

Student Name: [RIMAS MOHAMMED]

---

## Project Write-up

### 1. Agent Fundamentals
* Pattern Used: [e.g., Single Agent with Structured Output / Tools Extraction]
* Why: We implemented a working agent with real tool calls to ensure the model interacts dynamically with the environment rather than using hardcoded outputs, applying structured output where appropriate.

### 2. Multi-Agent / Routing Architecture
* Pattern Used: [e.g., Supervisor + Subagents (Track A) / Ticket Triage with Handoff (Track B) / Router across sources (Track C) / Skill-Routing (Track D)]
* Why: Designed explicitly to match the course's recommended architectural pattern rather than an ad-hoc design, allowing seamless coordination and task execution across our selected track.

### 3. RAG Pipeline
* Pattern Used: [e.g., 2-Step RAG / Agentic RAG / Hybrid RAG]
* Why: We loaded, split, embedded, and stored the documents to perform an actual retrieval step. This approach was chosen to optimize retrieval accuracy and context relevancy for our specific use case.

### 4. Context & State Management
* Pattern Used: [e.g., Persistent thread via LangGraph Checkpointer with Short-term and Long-term memory]
* Why: Used to maintain a persistent thread via a checkpointer, making explicit use of short-term and long-term memory instead of just relying on a simple chat-history list.

### 5. Human-in-the-Loop
* Pattern Used: [e.g., interrupt()-based pause point for approval]
* Why: Implemented at least one real interrupt-based pause point requiring explicit human approval or input before continuing sensitive actions, ensuring safety and control.

### 6. LangGraph Functional API & Error Handling
* Pattern Used: [e.g., Transient Retry + LLM-recoverable Loopback]
* Why: Correctly utilized @task and @entrypoint decorators while implementing two specific error-handling strategies to make the system resilient against network issues or unexpected failures.

### 7. Workflow Pattern
* Pattern Used: [e.g., Prompt Chaining / Parallelization / Routing / Orchestrator-Worker / Evaluator-Optimizer]
* Why: This workflow pattern was explicitly implemented and named to properly structure the execution steps and maximize the LLM's overall efficiency.

### 8. LangSmith Observability
* Analysis: LangSmith tracing was fully enabled. The traces successfully revealed critical execution details (such as a minor latency bottleneck / a bad tool call / step execution order), which allowed us to inspect and refine the entire pipeline.
# Agentic----AI
