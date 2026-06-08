# Runner Trial Source Matrix

Status: ready for next real runner trial — not validation-complete.

Use this before filling [[Live Runner Trial Packet]] when a runner task has multiple source docs, branches, logs, and acceptance claims. The goal is to prevent a promotion decision from relying on memory or vague screenshots.

## Trial header

- Runner under review:
- Workflow / project:
- Trial owner:
- Trial date:
- Related kickoff card:
- Related live packet:

## Source inventory

| Source type | Required? | Exact link/path | Owner | Notes |
| --- | --- | --- | --- | --- |
| Product/spec issue | Yes |  |  |  |
| Branch or workspace | Yes |  |  |  |
| Durable agent log | Yes |  |  |  |
| Diff / commit / PR | Yes |  |  |  |
| Verification output | Yes |  |  |  |
| Secret-safety check | Yes |  |  |  |
| Dependency changes | If changed |  |  |  |
| Cost/runtime record | If available |  |  |  |
| Human intervention notes | If any |  |  |  |

## Claim-to-source map

Every promotion or pilot claim needs at least one source row.

| Claim | Source row(s) | Supported? | Gap to close |
| --- | --- | --- | --- |
| Runner preserved durable logs |  |  |  |
| Runner stayed inside allowed scope |  |  |  |
| Runner produced reviewable diff |  |  |  |
| Runner passed required verification |  |  |  |
| Runner avoided secret exposure |  |  |  |
| Runner is safe to reuse for this workflow |  |  |  |

## Decision readiness checklist

- [ ] All required source rows have exact paths/URLs.
- [ ] Claims cite source rows, not memory.
- [ ] Any missing source is marked as a blocker or pilot constraint.
- [ ] [[Runner Promotion Decision Card]] uses this matrix before selecting promote / pilot-only / hold.

## Handoff prompt

```markdown
Use the Runner Trial Source Matrix to audit whether this runner trial has enough source-backed evidence for a promotion decision. Do not infer missing proof. Return: supported claims, unsupported claims, blockers, and the safest decision option.
```
