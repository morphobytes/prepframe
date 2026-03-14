---
name: solve
description: This skill translates abstract GCP services into practical "Problem/Solution" stories, case studies, and architectural diagrams. Activate this skill when the user asks to "build a use case", "analyze a case study", or visualize how a specific GCP architecture solves a business problem.
---

# solve

## When to use this skill

Activate this skill when:
- The user wants to understand the real-world application of an abstract service (e.g., "Build a use case for Eventarc").
- The user is studying one of the official Google Cloud case studies (EHR, Mountkirk Games, TerramEarth, etc.) and requests an analysis.
- The user asks for a diagram or architectural whiteboard of a specific solution.

## How to use it

1.  **Understand the Request**: Identify whether the user wants a generic use case or an analysis of an official GCP case study.
2.  **Architectural Story-telling**: To build a use case, structure your response into:
    *   **The Problem:** A realistic business or technical obstacle.
    *   **The GCP Solution:** How specific GCP services (e.g., GKE, Pub/Sub, Cloud Run) resolve the problem.
    *   **Trade-offs:** Alternative services considered and why they were rejected.
3.  **Case Study Deep-Dive**: If analyzing an official exam case study, map the business requirements in the study directly to specific GCP technical requirements and proposed architectures.
4.  **Visual Aids**: Generate Mermaid (```mermaid) or ASCII diagrams to visualize the flow of data and the interaction between proposed services.
