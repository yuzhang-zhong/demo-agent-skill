# DemoAgent Skill

DemoAgent is an agent skill for turning software projects into clear, reproducible, human-facing demo artifacts.

Instead of treating a demo as a single screen recording, DemoAgent guides an agent through project understanding, demo planning, execution, evidence capture, verification, and honest artifact composition — producing a demo package that future developers can inspect, trust, and rerun.

<!-- TODO: add screenshot -->

## Features

- **SKILL.md entry point** — a single skill definition with YAML frontmatter (`name`, `description`) that tells an agent when and how to use DemoAgent.
- **Five-step workflow** — guided stages for project understanding, demo planning, demo execution, demo verification, and artifact composition (`workflow/`).
- **Reusable templates** — demo goal, demo plan/storyboard, demo trace, verification report, and README demo section templates (`templates/`).
- **Worked examples** — example demo structures for three project types: a React app, an AI tool, and a game (`examples/`).
- **Honesty-first rules** — the skill requires clearly distinguishing verified, failed, assumed, untested, and blocked steps; it never claims that unverified behavior was actually demonstrated.
- **Validator-friendly** — includes a self-demo output package (`outputs/demoagent-self-demo/`) showing the repository structure and a passing skill validation result.
- **Documentation-only** — no runtime code and no dependencies, so it works with any agent or skill runtime that supports Markdown-based skills.

## Quick Start

1. Read `SKILL.md` — it is the primary entry point and describes when to use DemoAgent, what it produces, and how to run the workflow.
2. Follow the `workflow/` guides in order (01 → 05).
3. Fill in the `templates/` to capture your demo goal, plan, trace, and verification report.
4. Compose the final demo package under `outputs/<project-demo-name>/`.

## Installation

This skill is documentation-only and has no dependencies.

Clone it for reference:

```bash
git clone https://github.com/yuzhang-zhong/demo-agent-skill.git
```

To make it available to an agent, copy it into that agent's skill directory (the exact path varies by agent, e.g. a `skills/` folder under the agent's config directory):

```bash
cp -r demo-agent-skill <agent-config-dir>/skills/demoagent
```

## Usage

Use DemoAgent when a user asks for a project demo, walkthrough, product showcase, GitHub demo video, research prototype demo, or reproducible demo artifact.

The workflow defined in `SKILL.md`:

1. **Project understanding** (`workflow/01_project_understanding.md`) — inspect what the software does, how it runs, and which features are most worth demonstrating.
2. **Demo planning** (`workflow/02_demo_planning.md`) — write a demo goal and storyboard using the templates.
3. **Demo execution** (`workflow/03_demo_execution.md`) — run the flow and capture screenshots, recordings, or logs.
4. **Demo verification** (`workflow/04_demo_verification.md`) — verify what actually worked; record failures, assumptions, and blocked steps honestly.
5. **Artifact composition** (`workflow/05_artifact_composition.md`) — assemble the demo package under `outputs/`.

For contributor guidance on writing, editing, and quality expectations, see `AGENTS.md`.

## Project Structure

```text
demo-agent-skill/
├── SKILL.md                  # Skill definition (entry point)
├── AGENTS.md                 # Contributor/agent guidance
├── LICENSE                   # MIT license
├── README.md                 # This file
├── workflow/                 # Step-by-step demo workflow guides
│   ├── 01_project_understanding.md
│   ├── 02_demo_planning.md
│   ├── 03_demo_execution.md
│   ├── 04_demo_verification.md
│   └── 05_artifact_composition.md
├── templates/                # Reusable demo artifact templates
│   ├── demo_goal_template.md
│   ├── demo_plan_template.md
│   ├── demo_trace_template.md
│   ├── verification_report_template.md
│   └── readme_demo_template.md
├── examples/                 # Example demo structures
│   ├── example_react_app_demo/
│   ├── example_ai_tool_demo/
│   └── example_game_demo/
└── outputs/                  # Demo output packages
    ├── README.md
    └── demoagent-self-demo/  # Self-demo: structure + validation evidence
```

## Tech Stack

- **Markdown documentation** — the entire skill is plain Markdown files.
- **Agent skill convention** — `SKILL.md` with YAML frontmatter (`name`, `description`) for skill discovery.
- **No runtime code or dependencies** — nothing to build or install; works with any agent or skill runtime that supports Markdown-based skills.
- Validation shown in the self-demo was performed with an external skill validator (`quick_validate.py`); see `outputs/demoagent-self-demo/`.

## License

MIT — see [LICENSE](LICENSE).
