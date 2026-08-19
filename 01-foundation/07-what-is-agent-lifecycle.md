# What is the Agent Lifecycle?

The **Agent Lifecycle** describes what happens from the moment an agent receives a task until the task is completed.

A typical agent goes through several stages:

1. **Input** — The agent receives a goal or request.
2. **Context Building** — The agent gathers the relevant state, memory, knowledge, and other context.
3. **Reasoning** — The model decides what to do next.
4. **Action** — The agent may call a tool, execute code, retrieve information, or interact with another system.
5. **Observation** — The result of the action is added back to the agent's context.
6. **Iteration** — The agent reasons again and decides whether another action is needed.
7. **Completion** — The agent produces a final result when the task is complete.

The important part is that an agent is usually **a loop, not a single LLM call**.

For example:

User Request
→ Context
→ Reasoning
→ Action
→ Observation
→ Reasoning
→ Action
→ ...
→ Final Result

## Why is this important?

The lifecycle is where many agent capabilities come together.

> An agent is not just an LLM that answers a question. It is a system that repeatedly reasons, acts, observes, and updates its context until it reaches a stopping condition.
