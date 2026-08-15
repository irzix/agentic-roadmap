# What Is an Agent?

An Agent is a system that uses an LLM to make decisions and take actions to achieve a goal.

An Agent adds things around the LLM:

`User → Agent → LLM → Action → Observation → LLM → ...`

Imagine an automated workflow, Agent is really look like a flow with a big different thing: Agents have a non-deterministic flow but automations have a deterministic flow which is why Agents useful when we don't have a predfined path.

## What Makes a System an Agent?

**There is no single universal definition**, but an Agent usually has these characteristics:

- **Goal** — something the Agent is trying to achieve, such as creating a landing page.
- **Decision Making** — it can decide what action to take. This is really important because some decisions must be deterministic, while others can be LLM-based.
- **Tools** — capabilities the Agent can invoke, such as external systems, internal functions, APIs, or MCP tools.
- **State** — it can keep track of what is happening. This is not the history of actions; it represents the **current state** of the Agent.
- **Observation** — the information or result the Agent receives after taking an action and uses to decide what to do next.
- **Iteration** — it can perform multiple steps instead of generating a single response. This introduces several trade-offs around latency, cost, reliability, and complexity.


For example, consider a simple customer support Agent.

The user says:

`"Where is my order?"`

The Agent might:

`User Request`
→ `Understand the goal`
→ `Call order API`
→ `Observe the result`
→ `Decide what information is relevant`
→ `Respond to the user`

The important part is that the Agent is not simply generating an answer. It is **deciding and acting based on the current state and available information**.
