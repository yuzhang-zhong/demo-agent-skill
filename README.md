# DemoAgent Skill

DemoAgent is an agent skill for turning software projects into clear, reproducible demo artifacts.

It helps an agent understand a project, choose a useful demo goal, plan a human-readable walkthrough, execute or simulate the flow, capture evidence, verify what actually worked, and compose reusable demo notes.

## What DemoAgent Produces

DemoAgent is designed to produce:

- A demo goal.
- A demo plan or storyboard.
- A recorded demo video, or recording instructions.
- Key screenshots or keyframes.
- A demo trace.
- A verification report.
- A README-ready demo section.
- Honest notes about failures, limitations, and incomplete parts.

## Repository Structure

```text
demo-agent-skill/
  SKILL.md
  AGENTS.md
  README.md
  workflow/
    01_project_understanding.md
    02_demo_planning.md
    03_demo_execution.md
    04_demo_verification.md
    05_artifact_composition.md
  templates/
    demo_goal_template.md
    demo_plan_template.md
    demo_trace_template.md
    verification_report_template.md
    readme_demo_template.md
  examples/
    example_react_app_demo/
    example_ai_tool_demo/
    example_game_demo/
  outputs/
    README.md
```

## How To Use

Use DemoAgent when a developer asks for a project demo, walkthrough, product showcase, GitHub demo video, research prototype demo, or reproducible demo artifact.

Start with `SKILL.md`. It contains the core skill behavior and points to the workflow files and templates only when more detail is needed.

## Philosophy

Software demos should be reproducible, inspectable, and honest. DemoAgent treats demos as durable engineering artifacts, not just polished recordings.

A good demo should help viewers understand what the software does and help future developers rerun the same story with enough context to verify the result.
