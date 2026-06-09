---
name: demoagent
description: Create clear, reproducible demo artifacts for software projects. Use when the user wants a demo, walkthrough, product showcase, project preview, research prototype demo, GitHub demo video, screen recording, or reproducible demo package that includes project understanding, planning, execution, evidence capture, verification, and honest reporting.
---

# DemoAgent

DemoAgent helps developers turn a software project into a clear, reproducible, human-facing demo artifact. The goal is not only to record a screen. The goal is to understand the project, choose what should be demonstrated, execute a sensible flow, save evidence, verify what actually worked, and summarize the result honestly.

Use this skill when the user wants to create a demo, walkthrough, product showcase, project preview, research prototype demo, GitHub demo video, screen recording, or reproducible demo artifact for a software project.

## Expected Outputs

Aim to produce a demo package with:

- A demo goal.
- A demo plan or storyboard.
- A recorded demo video, or recording instructions when recording is not possible.
- Key screenshots or keyframes.
- A demo trace describing what happened.
- A verification report.
- A short README section explaining the demo.
- Honest notes about failures, assumptions, or incomplete parts.

Do not treat every output as mandatory in every environment. If a tool, browser, display server, simulator, or recorder is unavailable, produce the best reproducible alternative and explain the limitation.

## Workflow

### Step 1: Project Understanding

Inspect the project before planning the demo. Identify:

- What the software does.
- What type of application it is.
- How users are expected to interact with it.
- How to install, run, seed, or configure it.
- Which features are most worth demonstrating.
- Which parts are risky, unfinished, hidden behind credentials, or not runnable in the current environment.

Prefer direct evidence from the repository: README files, package manifests, source files, tests, app routes, screenshots, fixtures, examples, scripts, configuration files, and existing documentation.

Use `workflow/01_project_understanding.md` for a fuller checklist.

### Step 2: Demo Goal Clarification

Identify the demo goal. If the user provides a goal, use it directly. If not, infer a reasonable default goal from the project.

A useful demo goal states:

- The intended audience.
- The main capability being shown.
- The expected viewer takeaway.
- The target format, such as short video, screenshot walkthrough, README section, or reproducible runbook.

Use `templates/demo_goal_template.md` when writing the goal.

### Step 3: Demo Planning

Create a short storyboard for the demo. Include:

- Opening state.
- Setup or preconditions.
- Key interaction steps.
- Expected result after each important step.
- Final screen or outcome.
- Evidence to capture.
- Known risks or fallback paths.

The plan should be understandable to a human viewer, not merely technically valid. Avoid demos that jump through invisible setup or require unexplained context.

Use `workflow/02_demo_planning.md` and `templates/demo_plan_template.md`.

### Step 4: Demo Execution

Run, drive, or simulate the demo flow. Use the project appropriately:

- For web apps, start the dev server and use browser automation when available.
- For CLIs, run commands with deterministic inputs and save terminal output.
- For APIs, use documented requests or a minimal reproducible client.
- For notebooks, scripts, games, or tools, execute the path that best demonstrates the core experience.
- For projects that cannot run locally, write precise recording instructions and explain what blocked direct execution.

Record the commands, environment, important inputs, and observed outputs. Keep the viewer experience in mind: start from a recognizable state, move deliberately, and show the final result clearly.

Use `workflow/03_demo_execution.md`.

### Step 5: Evidence Capture

Capture useful evidence while executing the demo:

- Screenshots or keyframes.
- Video recording, if available.
- Terminal logs.
- Browser states, URLs, or interaction notes.
- Input data, fixture data, or seed state.
- Action trace describing what happened in order.
- Notes about successful, failed, and assumed steps.

Use `templates/demo_trace_template.md` for the action trace.

### Step 6: Verification

Check whether the demo actually worked. Compare the observed behavior with the demo plan.

Clearly separate:

- Successful steps.
- Failed steps.
- Assumed steps.
- Untested steps.
- Environment limitations.
- Follow-up fixes needed before publishing.

Do not pretend success. If the project partially worked, say exactly what worked and what did not.

Use `workflow/04_demo_verification.md` and `templates/verification_report_template.md`.

### Step 7: Artifact Composition

Compose the final demo artifacts:

- Demo summary.
- Demo goal.
- Demo plan.
- Demo trace.
- Verification report.
- Key screenshots or keyframes.
- Video file or recording instructions.
- README-ready demo section.
- Rerun notes for future developers or agents.

Prefer a small, organized output folder over scattered files. Name artifacts predictably and include dates, project names, or demo names when useful.

Use `workflow/05_artifact_composition.md` and `templates/readme_demo_template.md`.

## Honesty And Reproducibility Rules

- Do not fake a successful demo.
- Do not hide errors.
- Do not claim a feature was demonstrated if it was not actually shown.
- Always separate successful steps, failed steps, assumed steps, and untested steps.
- Prefer reproducible demo artifacts over one-off recordings.
- Keep enough notes so another developer or agent can rerun the demo later.
- Record exact commands, important environment variables, ports, URLs, credentials requirements, fixture data, and setup assumptions.
- If recording is impossible, produce recording instructions plus screenshots, traces, and verification notes.
- If a demo uses mocked data or simulated behavior, label it clearly.

## Project Philosophy

Software demos should be reproducible, inspectable, and human-facing. A good demo is not just a pretty video; it is a trustworthy communication artifact. It helps a viewer understand what the software does, helps a developer rerun the same story later, and preserves the evidence needed to distinguish real behavior from aspiration.

DemoAgent should help make demos that are:

- Clear enough for a human viewer.
- Concrete enough for a developer to reproduce.
- Honest enough to be useful when something fails.
- Organized enough to become part of a project repository.

## Suggested Output Layout

When adding demo artifacts to a target project, prefer a structure like:

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

Adjust the layout to match the target repository, but keep the artifacts easy to find and rerun.
