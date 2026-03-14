# quiz

The **quiz** skill is the generator for scenario-based multiple-choice questions aligned with specific exam domains.

## Core Functions

1. **Scenario Generation**: Uses the RAG pattern to pull from `content/` and official GCP documentation to create complex real-world scenarios.
2. **Multiple-Choice Generation**: Creates 4-choice questions with detailed explanations for why each option is correct or incorrect.
3. **Case Study Alignment**: Aligns questions with specific PCA case studies (EHR, Mountkirk, etc.).

## Usage Guide

- **Generate Set**: Request a 10-question set for a specific domain (e.g., "Networking in PCA").
- **Review Mode**: Review answers and explanations for a previous set.
