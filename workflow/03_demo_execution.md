# Demo Execution And Evidence Capture Guide

Execute the planned flow in a way that is technically reproducible and understandable to a human viewer.

## Execution Modes

Use the mode that fits the project and environment:

- **Direct execution:** Run the app, drive the UI, call the API, or execute the CLI.
- **Instrumented execution:** Capture screenshots, logs, traces, or state snapshots while running.
- **Guided recording:** Provide precise recording instructions when the current environment cannot record directly.
- **Simulation:** Use only when direct execution is blocked, and clearly label simulated steps.

## Execution Notes To Capture

Record:

- Commands used.
- Working directory.
- Required environment variables, without exposing secrets.
- Runtime URLs and ports.
- Input data and fixture data.
- User interactions.
- Observed outputs.
- Errors, warnings, retries, or deviations from the plan.

## Viewer Experience

The demo should be readable as a story:

1. Show the starting state.
2. Perform visible, intentional actions.
3. Pause long enough for important results to be understood.
4. Show the final state clearly.
5. Avoid claiming that invisible setup is part of the demonstrated user experience.

## Failure Handling

If execution fails, preserve the evidence. Record what failed, where it failed, what was already demonstrated, and what would be required to finish the demo.
