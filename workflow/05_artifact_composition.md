# Artifact Composition Guide

Compose the final demo package from the plan, evidence, trace, and verification report.

## Recommended Output Package

```text
demo/
  README.md
  demo_goal.md
  demo_plan.md
  demo_trace.md
  verification_report.md
  screenshots/
  recordings/
  logs/
```

Adjust this structure to match the target project, but keep files easy to locate and rerun.

## Composition Checklist

- Include the demo goal.
- Include the demo plan.
- Include the trace of what happened.
- Include screenshots, keyframes, or recording instructions.
- Include logs when they are important for verification.
- Include a verification report.
- Include a short README-ready demo section.
- Include rerun instructions.
- Include honest limitations.

## README Demo Section

The README section should be concise and useful. It should answer:

- What does this demo show?
- How can someone run or watch it?
- What artifacts are included?
- What worked?
- What did not work or was not verified?

## Artifact Naming

Prefer predictable names:

- `demo_goal.md`
- `demo_plan.md`
- `demo_trace.md`
- `verification_report.md`
- `screenshots/01_opening_state.png`
- `screenshots/02_key_interaction.png`
- `recordings/demo.mp4`
- `logs/demo_run.log`

Use project-specific names only when they make the artifact clearer.
