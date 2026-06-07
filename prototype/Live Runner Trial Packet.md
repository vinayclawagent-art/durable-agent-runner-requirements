# Live Runner Trial Packet

Use this packet during the next real Mission Control background/cloud runner trial. It ties the readiness checklist, evidence attachment, promotion decision card, and handoff summary into one ordered proof packet.

Source package: [[../../Generated-Packages/Durable Agent Runner Requirements/README|Durable Agent Runner Requirements]]  
Loop: [[../../Improvement-Loops/Durable Agent Runner Requirements Loop|Durable Agent Runner Requirements Loop]]

## When to use

- A background/cloud runner is about to work on a real repo branch or Mission Control workflow.
- The operator can capture durable logs, branch details, dependency/config changes, and verification output.
- The goal is to decide whether the runner should be promoted, kept pilot-only, or held.

## Packet steps

| Step | Artifact | Fill during trial | Done |
| --- | --- | --- | --- |
| 1 | `runner-readiness-checklist.html` or [[runner-readiness-checklist]] | Score environment realism, branch isolation, logs, secrets, verification, and recovery path before trusting the run. | ☐ |
| 2 | [[Runner Trial Evidence Attachment Template]] | Attach branch proof, durable log URL/path, secret-safety scan, dependency changes, verification output, and decision delta. | ☐ |
| 3 | [[Runner Promotion Decision Card]] | Convert proof into promote / pilot-only / hold with explicit gate failures. | ☐ |
| 4 | [[Handoff Summary - Mission Control Background Agent Gate]] | Paste the completed packet block and link the proof artifacts. | ☐ |

## Trial fields

| Field | Value |
| --- | --- |
| Runner / provider | _TBD during live trial_ |
| Repo + branch | _TBD_ |
| Task attempted | _TBD_ |
| Durable log URL/path | _TBD_ |
| Checklist score | _TBD_ |
| Evidence attachment link | _TBD_ |
| Promotion card link | _TBD_ |
| Final decision | ☐ promote ☐ pilot-only ☐ hold |

## Minimum evidence checklist

- [ ] Branch name and before/after diff summary are recorded.
- [ ] Durable log, transcript, or job URL/path is linked and inspectable after the run.
- [ ] Secret-safety result confirms no credentials were committed or exposed in logs.
- [ ] Dependency/config changes are listed, or explicitly marked none.
- [ ] Verification command output includes command, exit status, and summary.
- [ ] Recovery/resume behavior is noted if the runner stalls, disconnects, or needs manual intervention.

## Copyable trial handoff block

```markdown
### Durable Runner Trial Packet
- Runner / provider:
- Repo + branch:
- Task attempted:
- Checklist score:
- Evidence attachment: [[Runner Trial Evidence Attachment Template]]
- Promotion decision: [[Runner Promotion Decision Card]]
- Gate failures:
- Final decision: promote | pilot-only | hold
- Required follow-up before next run:
```

## Changelog line to paste after the real run

```markdown
- YYYY-MM-DD: Filled [[Durable Agent Runner Requirements/Live Runner Trial Packet]] for `<runner + repo>` and attached durable log, branch proof, verification output, and decision.
```

## Next action

During the next live runner trial, fill this packet before editing the package status. This artifact is ready for the next trial; no runner proof or validation outcome has been invented.
