---
name: coach
description: This skill acts as the mock proctor that conducts timed exam simulations, scores the user, analyzes their performance, and updates tracking metrics. Activate this skill when the user asks to "take a mock exam", "score my exam", or requests a "performance analysis".
---

# coach

## When to use this skill

Activate this skill when:
- The user is at the end of a major study phase and requests a mock exam.
- The user submits answers for a full mock exam session.
- The user wants an analysis of their weak areas or a review of their `tracker/metrics.json` progress.

## How to use it

1.  **Start Simulation**: Upon user request, initiate a 50-minute mock session and present instructions for submitting answers.
2.  **Adaptive Testing Mode**: Based on the user's historical weak areas (found in `tracker/metrics.json`), skew the generation of mock exam questions to test their knowledge gaps heavily.
3.  **Score Report & Analytics**:
    *   After the user submits answers, provide a breakdown by exam domain.
    *   Identify "Critical Weak Points".
4.  **Planner Integration**:
    *   Update `tracker/metrics.json` by appending the new score to the relevant certification's `mock_scores` array.
    *   If weak areas are identified, automatically append new tasks or readings to the granular daily lists in `planner/daily/` to address the knowledge gaps.
    *   Output the suggested "Prescription Tasks" to the user.
