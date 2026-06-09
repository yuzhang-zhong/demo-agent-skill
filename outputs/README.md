# Outputs

This directory is reserved for generated or example demo output packages.

Keep committed outputs small and intentional. For real project demos, prefer storing large recordings outside the repository or under a release artifact system, then link to them from the generated demo README.

Suggested output package:

```text
outputs/
  <project-demo-name>/
    README.md
    demo_goal.md
    demo_plan.md
    demo_trace.md
    verification_report.md
    screenshots/
    recordings/
    logs/
```

Generated demo artifacts should clearly distinguish successful, failed, assumed, untested, and blocked steps.
