# CI POSTROOMMAL DEMO

Sandbox repository for the Thursday onboarding CI postmortem demo.

## Workflow

This repo contains a GitHub Actions workflow at `.github/workflows/demo-fail.yml`
that intentionally fails (`exit 1`) so we can walk through a real failed-run
postmortem on stage.

## Running the demo

1. This workflow runs on every `push` and can be triggered manually via
   `workflow_dispatch`.
2. Check the **Actions** tab for the latest run; it should end with a failure.
3. The failing job is `explode`, and its log contains the verbatim error line
   captured for the postmortem issue.
