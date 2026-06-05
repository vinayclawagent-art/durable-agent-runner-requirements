# Handoff Summary: Mission Control Background Agent Gate

Source package: [[../../Generated-Packages/Durable Agent Runner Requirements/README|Durable Agent Runner Requirements]]
Generated from: `runner-readiness-checklist.html`
Date: 2026-06-05

## Runner evaluated
**Candidate:** Mission Control background coding-agent runner

**Scope of simulated gate:** Accepting a long-running agent lane that can modify code, preserve proof, and hand off safely without human babysitting.

## Gate result
**Decision:** Pilot only

The candidate is promising enough for bounded non-production tasks, but should not receive unattended production-changing work until secret-safety log scanning and post-run evidence retention are automated.

## Requirement scores
| Requirement | Status | Evidence captured | Follow-up |
| --- | --- | --- | --- |
| Durable lifecycle | Pass | Runner must expose process/session ID, final exit code, and durable log path after a 30+ minute bounded task. | Run the next trial with a persisted log URL or artifact path. |
| Branch isolation | Pass | Gate requires dedicated branch/repo copy and `git status --short --branch` before handoff. | Reject any run that starts on `main`. |
| Dependency policy | Partial | Installs must be recorded, but global environment drift is still manually reviewed. | Add a dependency-change section to every handoff. |
| Secret safety | Partial | Redaction is required, but no automated token-pattern scan is attached yet. | Add a log scan step before pilot graduates to accept. |
| Verification | Pass | Handoff must include commands, exit codes, and artifact paths or an explicit “not applicable” reason. | Keep as hard gate. |
| Handoff | Pass | Final report requires changed paths, commit SHA, risks, and next action. | Mirror this summary into runner docs if reused. |

## Copied handoff summary
```markdown
Runner: Mission Control background coding-agent runner
Decision: Pilot only
Commit / branch proof: required before acceptance
Durable logs: required before acceptance
Verification: commands + exit codes required
Primary blocker: automated secret-safety log scan is not yet attached
Next action: run a bounded pilot on a non-production task and archive the durable log URL plus `git status --short --branch`
```

## Promotion criteria
Move from **Pilot only** to **Accept** only when:

1. The runner completes one bounded 30+ minute task with durable logs still accessible after completion.
2. The handoff includes `git status --short --branch`, diff summary, verification output, and commit SHA.
3. A token-pattern scan or equivalent redaction check is attached to the run evidence.
4. Dependency/install changes are isolated to the repo, venv, or container and are documented.

## Next artifact improvement
If another runner trial uses this gate, add an export/download control to `runner-readiness-checklist.html` so copied handoffs become less manual.
