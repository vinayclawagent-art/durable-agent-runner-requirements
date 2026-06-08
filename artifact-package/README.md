---
type: artifact-package
status: active
source_note: "[[Cursor Cloud Agent Lessons as Durable Execution Pattern]]"
source_url: "https://x.com/cursor_ai/status/2061878340265656620"
github_repo: "https://github.com/vinayclawagent-art/durable-agent-runner-requirements"
score: 8
artifact_tracks: [prototype, infographic, skill]
improvement_cadence: nightly
last_improved: 2026-06-07
tags: [artifact-package, x-intel, agent-workflows]
---

# Artifact Package: Durable Agent Runner Requirements

Source: [[Cursor Cloud Agent Lessons as Durable Execution Pattern]]

## Why this matters
Cursor’s cloud-agent lessons map directly to Hermes/Mission Control: durable logs, realistic environments, harnesses, and verification are table stakes for trustworthy long-running agents.

## Artifact score
**8/10** — high because it is repeatable, agent-building relevant, and can become visible workflow infrastructure for VinClawLabs.

## Generated artifacts
- Prototype: [[Durable Agent Runner Requirements/runner-readiness-checklist]]
- Interactive prototype: [[Durable Agent Runner Requirements/runner-readiness-checklist.html|runner-readiness-checklist.html]]
- Worked example: [[Durable Agent Runner Requirements/Worked Example - Mission Control Background Agent Gate]]
- Handoff summary: [[Durable Agent Runner Requirements/Handoff Summary - Mission Control Background Agent Gate]]
- Evidence template: [[Durable Agent Runner Requirements/Runner Trial Evidence Attachment Template]]
- Decision card: [[Durable Agent Runner Requirements/Runner Promotion Decision Card]]
- Trial packet: [[Durable Agent Runner Requirements/Live Runner Trial Packet]]
- Source matrix: [[Durable Agent Runner Requirements/Runner Trial Source Matrix]]
- Infographic: [[Durable Agent Runner Requirements Workflow]]
- Skill draft: [[durable-agent-runner-requirements/SKILL]]
- Improvement loop: [[Durable Agent Runner Requirements Loop]]

- Kickoff card: [[Durable Agent Runner Requirements/Live Runner Trial Kickoff Card]]

## Prototype brief
A requirements checklist for evaluating or building any cloud agent runner before trusting it with real code or ops work.

## Infographic brief
Show the workflow from source signal to repeatable agent/product artifact.

## Skill candidate
Drafted as `durable-agent-runner-requirements`. Not promoted yet because it overlaps with existing Hermes planning/product/artifact skills and needs one more real-world reuse pass.

## GitHub repo
https://github.com/vinayclawagent-art/durable-agent-runner-requirements

## Improvement backlog
- Add one worked example from an active VinClawLabs project. ✅ Done with [[Durable Agent Runner Requirements/Worked Example - Mission Control Background Agent Gate]].
- Convert the markdown prototype into a small interactive HTML checklist if usage repeats. ✅ Done with `runner-readiness-checklist.html`.
- Run `runner-readiness-checklist.html` against one Mission Control runner and archive the copied handoff summary. ✅ Done with [[Durable Agent Runner Requirements/Handoff Summary - Mission Control Background Agent Gate]].
- Create an attachable proof packet for the next live runner trial. ✅ Done with [[Durable Agent Runner Requirements/Runner Trial Evidence Attachment Template]].
- Add a promotion decision card so live runner proof turns into an auditable promote / pilot-only / hold call. ✅ Done with [[Durable Agent Runner Requirements/Runner Promotion Decision Card]].
- Add a single live-trial packet that sequences readiness scoring, evidence attachment, promotion decision, and copied handoff. ✅ Done with [[Durable Agent Runner Requirements/Live Runner Trial Packet]].
- Add a source matrix so promotion claims cite exact issues, branches, logs, diffs, and verification outputs before a decision. ✅ Done with [[Durable Agent Runner Requirements/Runner Trial Source Matrix]].
- Decide whether to merge the skill draft into an existing skill or promote it after a live runner trial attaches durable logs.

## Change log
- 2026-06-04: Created nightly package, prototype, skill draft, loop, and GitHub repo sync.
- 2026-06-04: Added the Mission Control background-agent gate worked example and moved the first backlog item to done.
- 2026-06-04: Added a browser-based readiness checklist with scoring, saved state, and copyable handoff summary.
- 2026-06-05: Archived [[Durable Agent Runner Requirements/Handoff Summary - Mission Control Background Agent Gate]] with a pilot-only decision, requirement scores, and promotion criteria.
- 2026-06-05: Added [[Durable Agent Runner Requirements/Runner Trial Evidence Attachment Template]] so the next live runner trial can attach branch proof, durable logs, secret-safety scan, dependency changes, and verification evidence.
- 2026-06-06: Added [[Durable Agent Runner Requirements/Runner Promotion Decision Card]] to convert the next live-trial proof packet into an explicit promote / pilot-only / hold decision.
- 2026-06-06: Added [[Durable Agent Runner Requirements/Live Runner Trial Packet]] to bundle readiness score, evidence attachment, promotion decision, and handoff fields for the next real runner trial without inventing proof.
- 2026-06-07: Added [[Durable Agent Runner Requirements/Live Runner Trial Kickoff Card]] as the pre-trial scope/guardrail card for the next real-world run.
- 2026-06-08: Added [[Durable Agent Runner Requirements/Runner Trial Source Matrix]] so the next live runner trial can map every promotion claim to exact source evidence before a decision.
