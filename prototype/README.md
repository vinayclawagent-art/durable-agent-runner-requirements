# Durable Agent Runner Requirements Prototype

Use `runner-readiness-checklist.md` before trusting a background/cloud agent runner with real work. For a clickable pass/fail gate, open `runner-readiness-checklist.html` in a browser.

## Worked examples

- [[Worked Example - Mission Control Background Agent Gate]] — turns the checklist into a concrete acceptance gate for adding a new background coding-agent runner to Mission Control.
- [[Handoff Summary - Mission Control Background Agent Gate]] — archives a copied HTML-checklist handoff summary with pilot-only decision, requirement scores, blockers, and promotion criteria.
- [[Runner Trial Evidence Attachment Template]] — adds the missing proof packet for the next live runner trial: branch proof, durable log, secret-safety scan, dependency changes, verification, and promotion decision.

## Next iteration

Run the HTML gate against the next real runner trial and compare its copied handoff against [[Handoff Summary - Mission Control Background Agent Gate]].

## What it demonstrates
A requirements checklist for evaluating or building any cloud agent runner before trusting it with real code or ops work.

## How to use
Open `runner-readiness-checklist.html` for an interactive score, or `runner-readiness-checklist.md` for the plain markdown version, and fill it against one concrete project/workflow.

## Next iteration ideas
- Fill [[Runner Trial Evidence Attachment Template]] during the next live runner trial, then attach it to [[Handoff Summary - Mission Control Background Agent Gate]].
- Add export-to-markdown download after a real use proves the fields are stable.
- Link one accepted runner trial back into the package note.
