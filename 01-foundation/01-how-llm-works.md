# How Do LLMs Work?

Before understanding Agents, we need to understand the components that usually power them: **LLM (Large Language Model)**.

In easy word, an LLM is a model trained on a big data to learn patterns in language. Its basic job is to predict the next token based on the context it receives.

For example:

`The capital of Cyprus is` → `Nicosia`

The model predicts one token, adds it to the context, and predicts the next token. This process continues until the response is complete which you've seen this process while you are talking to GPT.

## Tokens

LLMs don't directly work with words. They work with **tokens**.

`Agent development is interesting` → `["Agent", " development", " is", " interesting"]`

The exact tokens depend on the tokenizer.

## Embeddings

Tokens are converted into numerical vectors called **embeddings**.

`Token → Embedding → Transformer`

These vectors allow the model to represent relationships and patterns between tokens.

Please attention to this subject because you will see this in RAG.

## Transformer & Attention

Modern LLMs are mainly based on the **Transformer** architecture.

One of the most important parts of the Transformer is **Attention**. Attention allows the model to understand relationships between different parts of the context.

For example:

> The developer deployed the application because it was ready.

Attention helps the model understand what `it` refers to based on the surrounding context. (this is really immpressive)

## Training vs. Inference

During **training**, the model learns its parameters from a huge amount of data.

During **inference**, we give the model context and ask it to generate tokens.

`Training: Data → Model → Learn Parameters`

`Inference: Context → Model → Next Token → Next Token → ...` (like when you use LLM to generate answer)

## Context Window

An LLM can only process a limited amount of context at once.

## Types of Context

- **System Instructions** — the identity, role, rules, and behavior of the agent.
- **User Message** — the user's request or input to the agent.
- **Conversation History** — previous messages, interactions, reflections, and other relevant history.
- **Available Tools** — external tools such as MCP tools, internal functions, and other available capabilities.
- **Tool Results** — outputs returned by tools, such as the result of a web search or an API call.
- **Retrieved Knowledge** — external knowledge retrieved for the agent, usually through a RAG pipeline.
- **Agent State** — the current state of the agent, such as actions, conditions, intermediate results, and execution status.

More context doesn't always mean a better Agent even it returns better answer in generations. This is one of trade-offs during agent development.

## Why Can LLMs Hallucinate?

An LLM is fundamentally predicting likely tokens. It isn't automatically connected to a database or a source of truth.

So it can generate something that sounds correct but is actually wrong.

This is one reason we use:

- Tools
- RAG
- External APIs
- Databases
- Validation

## LLM ≠ Agent

This is one of the most important concepts in Agent development.

An LLM by itself can generate a response:

`User → LLM → Response`

An Agent is a system built around an LLM:

`User → Agent → LLM → Tools / Memory / State / Knowledge / Execution`

The LLM is usually responsible for reasoning and generating decisions, while the surrounding system provides capabilities such as tools, memory, state, and execution.

> **An LLM is a model. An Agent is a system built around a model.**

Understanding this distinction is important because most of the interesting engineering problems in Agent development are not just about the LLM itself. They are about everything we build around it.
