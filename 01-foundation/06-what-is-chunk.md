# What is a Chunk?

A **chunk** is a small piece of a larger document or data source.

In RAG, large documents are split into smaller chunks so we can retrieve only the relevant parts instead of sending the entire document to the LLM.

For example:

Document → Chunk 1, Chunk 2, Chunk 3...

## How are Documents Chunked?

The simplest approach is to split a document by fixed size or by paragraphs.

However, newer approaches try to split text based on **meaning**, not just structure.

For example, instead of:

Paragraph 1 → Chunk 1
Paragraph 2 → Chunk 2
Paragraph 3 → Chunk 3

a semantic chunking approach asks:

> "Does this text still belong to the same concept?"

When the topic or meaning significantly changes, a new chunk is created.

This is called **Semantic Chunking**.

The advantage is that related information stays together even if the boundaries don't match paragraphs.

For example, a section might contain several short paragraphs that all explain the same concept. A semantic chunker can keep them together as one chunk.

The key idea:

> **Chunk boundaries should ideally follow meaning, not arbitrary text boundaries.**

## Why does chunking matter?

Chunking directly affects **retrieval quality**.

If chunks are too small, they may lose important context.

If chunks are too large, retrieval becomes less precise and we send more unnecessary information to the LLM.

So the goal is not simply:

> "Split the document every 500 tokens."

The goal is to create a **meaningful unit of information that can be retrieved independently**.
