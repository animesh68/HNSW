# Filtered Semantic Search on AG News
### A Baseline Reproduction Study of Filtered Approximate Nearest Neighbor Search

> **Research project on semantic search, vector databases, and filtered approximate nearest neighbor (ANN) retrieval.**

---

## Abstract

Semantic search retrieves documents according to their semantic similarity to a query rather than relying only on exact keyword matches.

Modern semantic search systems commonly represent documents as dense vector embeddings and use Approximate Nearest Neighbor (ANN) indexes to make retrieval efficient at scale.

However, real-world search queries often contain **both a semantic requirement and a structured filtering requirement**.

For example:

> Find the most relevant news articles about artificial intelligence, but only from the `Sci/Tech` category.

This creates a **filtered vector search** problem.

The vector component answers:

> Which documents are most semantically similar to the query?

The filtering component answers:

> Which documents are allowed to appear in the result?

The two operations can be performed in different orders or integrated directly into the search process. Different strategies can therefore produce substantially different trade-offs between **retrieval recall, query latency, indexing cost, and memory usage**.

This project investigates these trade-offs by implementing and evaluating several filtered ANN search strategies under a common experimental protocol using the AG News dataset.

The current stage of the project is focused on **baseline reproduction and controlled experimentation**. No new algorithm is proposed at this stage.
