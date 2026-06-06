# Runner Promotion Decision Card

Use this after filling [[Runner Trial Evidence Attachment Template]] so the trial can move from raw proof to an explicit ship/hold decision without inventing evidence.

## Decision summary

| Field | Value |
| --- | --- |
| Runner / provider | _TBD during live trial_ |
| Repo + branch | _TBD_ |
| Durable log URL/path | _TBD_ |
| Checklist score | _TBD_ |
| Trial decision | ☐ promote ☐ pilot-only ☐ hold |
| Decision owner | _TBD_ |

## Promotion gates

| Gate | Pass evidence required | Status |
| --- | --- | --- |
| Durable execution | Link to replayable run log, transcript, or job URL | ☐ pass ☐ fail ☐ n/a |
| Branch isolation | Branch name plus clean diff summary before merge | ☐ pass ☐ fail ☐ n/a |
| Secret safety | Note confirming no credentials in diff/logs | ☐ pass ☐ fail ☐ n/a |
| Dependency control | List of installs/config changes or explicit none | ☐ pass ☐ fail ☐ n/a |
| Verification | Test/build/check command output with exit status | ☐ pass ☐ fail ☐ n/a |
| Recovery path | Resume/retry note if the runner stalls or disconnects | ☐ pass ☐ fail ☐ n/a |

## Decision rubric

- **Promote** only when every required gate has source-backed evidence and the copied handoff is inspectable without the original chat UI.
- **Pilot-only** when the runner produces useful work but one non-critical proof item is missing or manual recovery was required.
- **Hold** when durable logs, branch isolation, secret safety, or verification evidence is missing.

## Handoff block to copy

```markdown
### Runner promotion decision
- Runner / provider:
- Repo + branch:
- Durable log URL/path:
- Checklist score:
- Gate failures:
- Decision: promote | pilot-only | hold
- Required follow-up before next trial:
```

## Next attachment step

When a real Mission Control runner trial happens, fill this card immediately after the evidence attachment and paste the handoff block into [[Handoff Summary - Mission Control Background Agent Gate]].
