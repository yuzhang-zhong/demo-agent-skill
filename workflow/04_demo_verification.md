# Demo Verification Guide

Verify the demo against the plan before composing final artifacts.

## Verification Questions

- Did the project start or run as expected?
- Were the planned interactions actually performed?
- Were the expected results visible?
- Were screenshots, video, logs, or traces captured?
- Were there errors or warnings?
- Did any step require assumptions, mocks, manual intervention, credentials, or skipped setup?
- Could another developer or agent rerun the demo from the notes?

## Result Categories

Use these categories consistently:

- **Successful:** Actually demonstrated and supported by evidence.
- **Failed:** Attempted but did not work as planned.
- **Assumed:** Treated as true without direct verification.
- **Untested:** Not attempted.
- **Blocked:** Could not be attempted because of environment, credentials, missing dependencies, or other constraints.

## Verification Output

Write a concise report that includes:

- Overall status.
- Evidence reviewed.
- Successful steps.
- Failed or blocked steps.
- Assumptions.
- Reproducibility notes.
- Recommended fixes or follow-up work.

Do not soften or hide failures. A partial demo with accurate verification is more useful than a polished but misleading artifact.
