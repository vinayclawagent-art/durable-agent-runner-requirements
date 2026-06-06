# Runner Trial Evidence Attachment Template

Source package: [[../../Generated-Packages/Durable Agent Runner Requirements/README|Durable Agent Runner Requirements]]
Use with: [[Handoff Summary - Mission Control Background Agent Gate]]
Date created: 2026-06-05

## Purpose

This template converts the next live runner trial into attachable proof instead of a narrative-only handoff. Paste it under the handoff summary once a Mission Control background-agent trial finishes.

## Required evidence packet

| Evidence | Required format | Accept threshold | Notes |
| --- | --- | --- | --- |
| Runner identity | Candidate name, runtime, session/process ID | Concrete runner and session are named | Avoid vague labels like “the agent”. |
| Branch proof | `git status --short --branch` plus `git rev-parse HEAD` | Run starts off `main` or explicitly explains why not | Include before and after when possible. |
| Durable log | URL, artifact path, or persisted local path | Still accessible after process exit | Must include final exit code. |
| Secret-safety scan | Token-pattern scan command and exit code, or documented equivalent | Pass or explicit redaction remediation | Do not paste secrets into this note. |
| Dependency changes | Package manager output, lockfile diff, or “none” | All installs scoped to repo/venv/container | Global installs need a risk note. |
| Verification | Commands, exit codes, changed paths | At least one task-specific verification command | If not applicable, state why. |

## Copyable attachment block

```markdown
### Runner trial evidence — <date>
- Candidate:
- Session/process ID:
- Branch proof:
- Commit SHA:
- Durable log URL/path:
- Final exit code:
- Secret-safety scan:
- Dependency changes:
- Verification commands:
- Decision delta: keep Pilot / promote to Accept / reject
- Remaining risk:
```

## Promotion rule

The runner may only move from **Pilot only** to **Accept** when every row in the evidence packet has concrete proof, not just an assertion.
