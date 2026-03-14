# Configurator Skill

The **Configurator Skill** is the entry point for the GCP Prep Framework. It conducts a discovery session with the user to customize the study plan and repository structure.

## Core Functions

1. **Discovery Phase**: Asks the user about targets, timeline, intensity, and experience.
2. **Plan Generation**:
    - Calculates a week-by-week timeline based on the target date (default: May 2026).
    - Generates a custom `planner/schedule.md`.
    - Updates `task.md` with certification-specific phases.
3. **Repository Bootstrapping**:
    - Populates `tracker/metrics.json` with initial goals.
    - Creates `planner/daily/` entries for the first week.

## Bootstrap Logic (Pseudo-code)

```python
def generate_plan(targets, duration_weeks, intensity):
    # Logic to allocate weeks per certification
    # PCA: 3-4 weeks (Foundation)
    # PDE: 3-4 weeks
    # MLE: 4-5 weeks
    # Adjust based on intensity and total duration
    pass
```

## Workflows

- **Bootstrap Framework**: `npx run configurator --init`
- **Adjust Schedule**: `npx run configurator --recalc`
