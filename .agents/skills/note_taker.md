# Note-Taker Skill

The **Note-Taker Skill** is designed to capture, organize, and distill knowledge gathered during study sessions.

## Core Functions

1. **Draft Summarization**: Converts raw lab notes or documentation snippets into structured markdown in the `content/` folders.
2. **Standardization**: Ensures all notes follow the "Concepts, Commands, Use Cases" format.
3. **Cross-Linking**: Identifies common services across certifications (e.g., BigQuery) and links relevant notes.
4. **Flashcard Extraction (New)**: Automatically parses fact-based definitions, quotas, default ports, and IAM roles into a separate "Flashcard Output" section (Q&A format). This strictly separates rote memorization facts from the deeper architectural summaries.

## Usage Guide

- **New Note**: Provide the agent with a topic and raw text. The agent will output the architectural summary and the separate Flashcard definitions.
- **Review**: Request a summary of a specific service across PCA/PDE/MLE.
- **Flashcard Export**: Request all flashcards generated for a specific week or module to review in a spaced-repetition tool like Anki.
