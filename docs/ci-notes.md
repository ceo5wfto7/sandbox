# CI Pipeline Notes

Collected 2026-08-25.

## Current sandbox experiments

- Testing GitHub Actions matrix builds for multiple Python versions.
- Evaluating `act` for local workflow runs.
- Trying out reusable workflows across repos.

## Useful commands

```bash
# Validate workflow syntax
act --dry-run

# Run a specific job locally
act -j build

# Check YAML formatting
yamllint .github/workflows/*.yml
```

## Reminders

- Keep sandbox branches short-lived; delete after merge.
- Use `workflow_dispatch` for manual testing.
- Cache dependencies between jobs to speed up runs.
