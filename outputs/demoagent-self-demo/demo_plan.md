# Demo Plan

## Demo Goal

Show that the DemoAgent skill repository is complete, reusable, and valid.

## Opening State

The workspace contains the `demo-agent-skill/` repository folder.

## Preconditions

- PowerShell is available.
- Python is available.
- The local skill-creator validator is available.
- The DemoAgent repository files have already been generated.

## Storyboard

| Step | Action | Expected Result | Evidence To Capture |
| --- | --- | --- | --- |
| 1 | Inspect the repository tree. | Required files and folders are visible. | Command log |
| 2 | Open `SKILL.md`. | The file explains purpose, outputs, workflow, honesty rules, and philosophy. | Demo trace and file reference |
| 3 | Run the skill validator. | Validator reports that the skill is valid. | Command log |
| 4 | Compose demo artifacts. | Output package contains goal, plan, trace, verification report, and README. | Output files |

## Final State

The self-demo output package exists at `demo-agent-skill/outputs/demoagent-self-demo/`.

## Risks And Fallbacks

| Risk | Impact | Fallback |
| --- | --- | --- |
| No runnable UI exists. | No meaningful video or screenshots can be captured. | Produce written artifacts and validation evidence. |
| Validator path changes. | Validation command may fail in another environment. | Document the validator dependency and allow manual inspection. |
| Self-demo is narrower than a real project demo. | It does not prove behavior on a separate app. | Label the scope clearly and recommend a future real-project trial. |

## Rerun Notes

- Re-run the tree inspection command from the demo README.
- Re-run the validator command from the demo README.
