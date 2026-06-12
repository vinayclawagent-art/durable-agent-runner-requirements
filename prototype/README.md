# Durable Agent Runner Requirements Prototype

Use `runner-readiness-checklist.md` before trusting a background/cloud agent runner with real work. For a clickable pass/fail gate, open `runner-readiness-checklist.html` in a browser.

## Worked examples

- [[Worked Example - Mission Control Background Agent Gate]] — turns the checklist into a concrete acceptance gate for adding a new background coding-agent runner to Mission Control.
- [[Handoff Summary - Mission Control Background Agent Gate]] — archives a copied HTML-checklist handoff summary with pilot-only decision, requirement scores, blockers, and promotion criteria.
- [[Runner Trial Evidence Attachment Template]] — adds the missing proof packet for the next live runner trial: branch proof, durable log, secret-safety scan, dependency changes, verification, and promotion decision.
- [[Runner Promotion Decision Card]] — converts the next filled evidence attachment into a source-backed promote / pilot-only / hold decision with explicit gates.
- [[Live Runner Trial Packet]] — orders the readiness checklist, evidence attachment, promotion card, and handoff summary into one fillable proof packet for the next real runner trial.
- [[Runner Trial Source Matrix]] — maps every promotion claim to exact issues, branches, logs, diffs, and verification outputs before the decision card is filled.
- [[Runner Post-Trial Debrief Template]] — turns the future source-backed trial output into a promote / pilot-only / iterate / hold decision plus README/prototype/skill patch queue.

## Next iteration

Run [[Live Runner Trial Packet]] with [[Runner Trial Source Matrix]] during the next real runner trial, then fill [[Runner Post-Trial Debrief Template]] so checklist score, branch/log proof, verification output, decision gates, and handoff text become concrete patch decisions.

## What it demonstrates
A requirements checklist for evaluating or building any cloud agent runner before trusting it with real code or ops work.

## How to use
Open `runner-readiness-checklist.html` for an interactive score, or `runner-readiness-checklist.md` for the plain markdown version, and fill it against one concrete project/workflow.

## Next iteration ideas
- Fill [[Runner Trial Evidence Attachment Template]] during the next live runner trial, then attach it to [[Handoff Summary - Mission Control Background Agent Gate]].
- Fill [[Runner Promotion Decision Card]] immediately after the evidence attachment so the trial produces a decision, not just raw notes.
- Fill [[Live Runner Trial Packet]] as the canonical proof packet before updating the package with completed validation evidence.
- Fill [[Runner Trial Source Matrix]] before the promotion decision so every claim has an exact source path or is marked as a blocker.
- Fill [[Runner Post-Trial Debrief Template]] after the real trial before patching README, prototype, or skill wording.
- Add export-to-markdown download after a real use proves the fields are stable.
- Link one accepted runner trial back into the package note.
