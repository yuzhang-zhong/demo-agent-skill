# Project Understanding Guide

Before planning a demo, inspect the project enough to explain it accurately.

## Goals

- Identify what the project does.
- Identify the application type.
- Identify the primary user journey.
- Identify setup and runtime requirements.
- Identify features worth demonstrating.
- Identify risks, missing pieces, credentials, or blocked paths.

## Suggested Inspection Order

1. Read the main README and project documentation.
2. Inspect package manifests, dependency files, build files, and scripts.
3. Inspect app entry points, routes, commands, or public APIs.
4. Inspect tests, fixtures, seed data, examples, screenshots, and sample outputs.
5. Run lightweight setup or discovery commands when safe.
6. Summarize what is known, unknown, assumed, and blocked.

## Project Summary Format

```markdown
# Project Understanding

## Project Type

Describe the kind of software: web app, CLI, API, library, game, notebook, model demo, research prototype, or other.

## Core Purpose

Summarize what the software helps users do.

## Primary Users

Describe who the demo viewer or user likely is.

## Main Interaction Model

Describe how a user interacts with the project.

## Features Worth Demonstrating

- Feature 1
- Feature 2
- Feature 3

## Setup And Runtime Notes

List commands, ports, dependencies, environment variables, seed data, and credentials requirements.

## Risks Or Unknowns

Separate verified facts from assumptions.
```

## Guidance

Do not overfit the demo to implementation details. The project understanding step should explain the product experience and the technical constraints that matter for reproducing the demo.
