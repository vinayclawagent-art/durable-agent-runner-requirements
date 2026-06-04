# Agent Runner Readiness Checklist

Source package: [[Durable Agent Runner Requirements]]

## Minimum viable runner
- [ ] Durable process lifecycle with resumable logs
- [ ] Repo checkout and branch isolation
- [ ] Dependency install policy
- [ ] Secret-safe environment injection
- [ ] Test / build command discovery
- [ ] Artifact capture: diff, logs, screenshots, links
- [ ] Human-readable handoff summary

## Red flags
- Output disappears when browser tab closes
- Agent cannot rerun failed commands
- No commit SHA / diff evidence
- No way to separate exploratory logs from final claims

## VinClawLabs application
Use this as an acceptance gate before promoting any background coding agent into Mission Control.
