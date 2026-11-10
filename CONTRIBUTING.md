# Contributing to Ingenious AI open-source tools

Thanks for helping improve a defensive security tool.

## Ground rules

- **Dependency-light.** The tools are Python standard library only unless a
  change is discussed first. Small tools must stay easy to audit.
- **Tests prove detections.** Every detection change needs a fixture proving
  it fires — and one proving it does not fire on a benign input.
- **Honesty standard.** Verdicts must say exactly what a check establishes.
  "Not detected" never means "safe". Never strengthen a claim beyond the
  evidence the check produces.
- **No real secrets in fixtures.** Never commit real credentials, tokens, or
  third-party data.

## Workflow

1. Fork the repository and branch from its default branch.
2. Run the test suite before opening a pull request (`python -m pytest`).
3. In the PR, describe what your change detects or fixes, with sample output.

## Reporting bugs

Use the bug report template: tool version, OS and Python version, the exact
command, and the output you saw vs. what you expected.
