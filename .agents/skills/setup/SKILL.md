---
name: setup
description: This is the bootstrap skill that initializes the 12-week schedule and repository structure for the GCP Prep Framework. Activate this skill when the user explicitly requests to "setup", "bootstrap", or "initialize" their GCP study plan, or when they want to recalculate their timeline.
---

# setup

## When to use this skill

Activate this skill when:
- The user is starting the GCP Prep Framework for the first time.
- The user asks to "bootstrap the repository", "configure the schedule", or "setup the plan".
- The user wants to adjust their existing schedule or certification targets.

## How to use it

1.  **Discovery Phase**: Ask the user the following questions if the information is not already provided:
    *   **Targets**: Which certifications are you aiming for? (PCA, PDE, MLE).
    *   **Timeline**: What is your target exam date or available duration?
    *   **Intensity**: How many hours per day can you commit?
    *   **Experience**: What is your current level for each domain (Beginner, Intermediate, Expert)?
2.  **Plan Generation**:
    *   Calculate a week-by-week timeline based on the target date.
    *   Generate a custom `planner/schedule.md` file outlining the weekly topics.
    *   Update `task.md` with the newly generated certification-specific phases.
3.  **Repository Bootstrapping**:
    *   Populate `tracker/metrics.json` with initial goals and dates.
    *   Create granular daily task entries in `planner/daily/` for the first week of study.
