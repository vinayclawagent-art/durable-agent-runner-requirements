# Worked Example: Mission Control Background Agent Gate

Source package: [[../../Generated-Packages/Durable Agent Runner Requirements/README|Durable Agent Runner Requirements]]

## Scenario
Mission Control wants to accept a new background coding-agent runner as a durable execution option. Before it can be trusted with real VinClawLabs work, the runner must prove it can survive long jobs, preserve evidence, and hand off a verifiable result.

## Gate run

| Requirement | Pass condition | Evidence to capture |
| --- | --- | --- |
| Durable lifecycle | Runner can execute a bounded task for 30+ minutes and expose logs after completion. | Process/session ID, log URL or local log path, final exit code. |
| Branch isolation | Runner works in a dedicated branch or repo copy and never mutates `main` directly. | Branch name, `git status --short --branch`, diff summary. |
| Dependency policy | Runner records install commands and avoids global environment drift. | Lockfile diff, install log, venv/container path. |
| Secret safety | Runner can use required credentials without printing token values. | Redacted env proof and log scan result. |
| Verification | Runner discovers and executes the relevant tests/builds or records why none exist. | Command output, exit code, artifact path. |
| Handoff | Runner reports changed paths, commit SHA, remaining risks, and next action. | Final handoff note linked to commit/diff. |

## Decision rubric
- **Accept** when all pass conditions have evidence and no secret leakage appears in logs.
- **Pilot only** when lifecycle and verification pass but dependency policy or handoff needs tightening.
- **Reject** when logs disappear, branch isolation is absent, or final claims lack command output.

## Reusable command frame

```bash
git status --short --branch
# run the discovered install/test/build commands here
# capture exit code, changed paths, and final commit SHA
git diff --stat
git rev-parse HEAD
```

## Next artifact improvement
Convert this markdown gate into an interactive checklist only after one real Mission Control runner evaluation uses it end to end.
