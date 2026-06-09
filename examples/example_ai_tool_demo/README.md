# Example: AI Tool Demo

This example describes how DemoAgent might structure a demo for an AI-assisted tool, model wrapper, prompt utility, or agentic workflow.

## Example Goal

Show that the tool accepts a realistic input, performs the intended AI-assisted operation, and returns an understandable output.

## Example Storyboard

| Step | Action | Expected Result | Evidence |
| --- | --- | --- | --- |
| 1 | Prepare a small, non-sensitive input. | Input is visible and reproducible. | Fixture file or prompt text |
| 2 | Run the tool. | The tool completes without hidden manual intervention. | Terminal log or UI trace |
| 3 | Inspect the output. | Output is relevant to the input and clearly displayed. | Output file or screenshot |
| 4 | Verify limitations. | Model assumptions, errors, or uncertainty are documented. | Verification report |

## Example Verification Notes

- Do not expose secrets, private prompts, or sensitive training data.
- Label mocked model responses or offline simulations clearly.
- Distinguish between deterministic tool behavior and model-generated content.
