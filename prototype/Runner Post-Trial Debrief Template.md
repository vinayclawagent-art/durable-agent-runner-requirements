# Runner Post-Trial Debrief Template

Use after the next real durable-runner trial. This is a blank evidence template; do not mark the package validated until the fields are filled from a real run.

## Trial identity

- Date:
- Runner / agent:
- Repository or project:
- Issue / task URL:
- Branch / PR:
- Human operator:
- Trial packet used: [[Live Runner Trial Packet]]
- Source matrix used: [[Runner Trial Source Matrix]]

## Evidence recap

| Claim | Source link / path | Evidence summary | Confidence | Gap / blocker |
|---|---|---|---|---|
| Durable log exists and is replayable |  |  |  |  |
| Environment matched the target repo |  |  |  |  |
| Secret handling was safe |  |  |  |  |
| Dependency changes were explicit |  |  |  |  |
| Verification command passed or failed clearly |  |  |  |  |
| Handoff was understandable to a human reviewer |  |  |  |  |

## What changed because of the trial

- Requirement to tighten:
- Checklist field to rename/remove/add:
- README claim to patch:
- Skill-draft step to patch:
- Prototype artifact to update:

## Decision

Choose one and cite the exact evidence row above.

- [ ] Promote: runner pattern is ready for reusable workflow guidance.
- [ ] Pilot-only: useful, but one blocker must be fixed before promotion.
- [ ] Iterate: evidence changed the requirements materially.
- [ ] Hold: evidence was insufficient or unsafe.

Decision rationale:

## Follow-up patch queue

1. 
2. 
3. 

## Copyable changelog note

> After a real runner trial, filled the post-trial debrief with exact evidence links and converted the result into a promote / pilot-only / iterate / hold decision. Validation remains pending until the fields above are complete.
