---
name: distill
description: This skill processes raw reading notes, documentation snippets, or lab results into clean architectural summaries and separates rote "flashcards" from deep concepts. Activate this skill when the user provides raw study text or explicitly asks you to "distill", "summarize", or "take notes" on a specific GCP topic.
---

# distill

## When to use this skill

Activate this skill when:
- The user finishes reading a GCP topic and wants to organize their raw notes.
- The user pastes raw documentation or lab outputs and asks for a summary.
- The user asks you to extract "flashcards" or memorization targets from a block of text.

## How to use it

1.  **Information Diet**: Ingest the raw lab notes or documentation snippets provided by the user.
2.  **Separation of Concerns**:
    *   Extract rote facts (e.g., limits, quotas, port numbers, predefined IAM roles) into a "Flashcards" section.
    *   Extract conceptual information and architectural patterns into a "Deep Concept" section.
3.  **Markdown Generation**: Create a well-structured markdown file containing both sections.
4.  **Save Output**: Save the resulting markdown file to the appropriate certification folder in `content/` (e.g., `content/pca/vpc_networking.md`).
5.  **Cross-Linking**: If the topic overlaps multiple certifications (e.g., BigQuery is in PDE and MLE), explicitly note the cross-certification relevance at the top of the file.
