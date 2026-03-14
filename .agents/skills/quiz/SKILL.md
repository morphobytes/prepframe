---
name: quiz
description: This skill generates scenario-based multiple-choice questions aligned with specific Google Cloud certification exam domains. Activate this skill when the user asks you to "give me a quiz", "test my knowledge", "generate questions", or mentions scenario drilling.
---

# quiz

## When to use this skill

Activate this skill when:
- The user completes a study session and wants to test their knowledge.
- The user asks for a scenario question based on a specific GCP topic (e.g., VPC networks, GKE limits).
- The user requests a review of their answers from a previous quiz attempt.

## How to use it

1.  **Context Retrieval**: Use the RAG pattern or direct search to pull factual information from `content/` to formulate accurate questions. For PCA, refer back to the official case studies to flavor the scenarios.
2.  **Scenario Generation**: Formulate a question consisting of:
    *   A realistic business problem (The Scenario).
    *   A technical constraint (e.g., "cost must be minimized", "low latency is required").
    *   4 distinct options (A, B, C, D).
3.  **Explanation Generation**: For each question, internally (but do not output until the user answers) prepare an explanation detailing *why* the correct answer is right and, crucially, *why* the other 3 distractors are incorrect.
4.  **Review Mode**: If the user provides answers, compare them against the generated correct answers. Return the detailed explanations and highlight knowledge gaps.
