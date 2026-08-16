# What Is an Agent?

An Agent is a system that uses an LLM to make decisions and take actions to achieve a goal.

An Agent adds things around the LLM:

`User → Agent → LLM → Action → Observation → LLM → ...`

Imagine an automated workflow, Agent is really look like a flow with a big different thing: Agents have a non-deterministic flow but automations have a deterministic flow which is why Agents useful when we don't have a predfined path.

## What Makes a System an Agent?

There is no single universal definition, but an Agent usually has these characteristics:

- **Goal** — something the Agent is trying to achieve, such as creating a landing page.
- **Decision Making** — it can decide what action to take. Some decisions can be deterministic, while others can be LLM-based.
- **Tools** — capabilities the Agent can invoke, such as external systems, internal functions, APIs, or MCP tools.
- **State** — the current state of the Agent during execution. This is not simply the history of actions.
- **Observation** — the information or result the Agent receives after taking an action.
- **Evaluation** — it can evaluate whether the current outcome is good enough to achieve the goal.
- **Iteration** — it can continue taking actions when the goal has not yet been achieved.

For example, consider a simple customer support Agent.

The user says:

`"Where is my order?"`

The Agent might:

`User Request` → `Understand Goal` → `Decide Action` → `Call Order API` → `Observe Result` → `Evaluate`

If the result is sufficient, the Agent can finish:

`Evaluate` → `Goal Achieved` → `Respond`

If it is not sufficient, it can continue:

`Evaluate` → `Not Enough` → `Decide Again` → `Take Action` → `Observe` → `Evaluate` → `...`

The important part is that the Agent is not simply generating an answer. It is **deciding, acting, observing, and evaluating based on the current state and available information**.
