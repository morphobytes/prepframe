# setup

The **setup** skill is the bootstrap skill that initializes the 12-week schedule and repository structure.

## Core Functions

1. **Discovery Phase**: Asks the user about targets, timeline, intensity, and experience.
2. **Plan Generation**:
    - Calculates a week-by-week timeline based on the target date.
    - Generates a custom `planner/schedule.md`.
    - Updates `task.md` with certification-specific phases.
3. **Repository Bootstrapping**:
    - Populates `tracker/metrics.json` with initial goals.
    - Creates `planner/daily/` entries for the first week.

## Usage Guide

- **Bootstrap Framework**: Run this skill to initialize the environment.
- **Adjust Schedule**: Run to recalculate your timeline.
