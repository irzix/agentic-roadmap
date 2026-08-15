# Agent Development Roadmap

In this repository, I'm going to explain the fundamentals of agent development using general-purpose programming languages and real-world examples based on my own projects.
My goal is to create easy-to-follow learning content and videos based on practical examples, covering a complete series on agent development. The goal is to help programmers understand how to build agentic systems and make the right engineering trade-offs.
Agentic development is still a relatively new field, but many useful articles and resources have already been published. Throughout this repository, I'll try to reference relevant resources and research as I build and explain each topic.

## 1. Foundations

- [How do LLMs work?](./01-foundation/01-how-llm-works.md)
- [What is an Agent?](./01-foundation/02-what-is-agent.md)
- What is State?
- What is Memory?
- What types of Memory exist?
- What is Knowledge?
- What is a Chunk?
- What is the Agent Lifecycle?

## 2. Tools & Actions

- How does Tool Calling work?
- What is MCP and how does it work?
- Tool Calling vs. MCP
- Deterministic Conditions
- Structured Output

## 3. Agent Architecture

- What is an Agent Flow?
- What is Agent Orchestration?
- Agent Flow vs. Orchestration
- Nodes and Edges
- What are Subagents?
- Types of Subagents
- Agent Delegation
- Trade-offs of different Nodes and Subagents

## 4. Context Engineering

- What is Context Engineering?
- Context Window
- Context Selection
- Context Compression
- Context Isolation
- Context Management
- Managing Tool Context
- Context vs. Memory vs. Knowledge
- Context Growth and Optimization

## 5. Knowledge & RAG

- How does RAG work?
- RAG Strategies
- Chunking Strategies
- Retrieval Strategies
- Reranking
- RAG Trade-offs
- RAG Optimization

## 6. Memory & Experience

- Short-term Memory
- Long-term Memory
- Semantic Memory
- Episodic Memory
- Procedural Memory
- Experience
- Reflection
- Human Feedback

## 7. Reliability

- Agent Failure Modes
- Retry
- Idempotency
- Timeout
- Caching
- Agent Failure Recovery
- Deterministic vs. Probabilistic Behavior
- Human-in-the-Loop (HITL)

## 8. Multi-Agent Systems

- Why Multiple Agents?
- Agent Delegation
- Agent Communication
- Supervisor Pattern
- Specialist Agents
- Parallel Agents
- Multi-Agent Workflows
- Trade-offs of Multi-Agent Systems

## 9. Evaluation

- Why is Agent Evaluation Different?
- Step-level Evaluation
- Final Evaluation
- Tool-call Evaluation
- Trajectory Evaluation
- LLM-as-a-Judge
- Evaluation Datasets
- Human Evaluation
- Regression Testing

## 10. Observability

- Agent Observability
- Tracing
- Logging
- Metrics
- Token Monitoring
- Cost Monitoring
- Agent Performance Monitoring

## 11. Security & Guardrails

- Prompt Injection
- Tool Permissions
- Agent Authorization
- Data Leakage
- Untrusted Tool Output
- Guardrails
- Input Validation
- Output Validation

## 12. Governance

- Agent Governance
- Permissions
- Policies
- Auditability
- Human Oversight
- Compliance
- Safe Agent Execution

## 13. Performance & Optimization

- Token Optimization
- Context Optimization
- Model Selection
- Caching Strategies
- Parallel Tool Calling
- Concurrency
- Latency Optimization
- Cost vs. Quality Trade-offs

## 14. Production Agent Systems

- Designing Production-ready Agents
- Agent Architecture Trade-offs
- Failure Recovery
- Scalability
- Reliability
- Observability
- Security
- Evaluation
- Cost Optimization
- Continuous Improvement
