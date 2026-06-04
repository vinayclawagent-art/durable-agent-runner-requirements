---
name: durable-agent-runner-requirements
description: Draft skill from X Artifact Factory package: Durable Agent Runner Requirements.
status: draft
source_note: "[[Cursor Cloud Agent Lessons as Durable Execution Pattern]]"
---

# Durable Agent Runner Requirements

Use this draft to evaluate a cloud/background agent runner.

1. Verify durable logs and resumability.
2. Verify repo checkout, branch isolation, and environment setup.
3. Verify the agent can run real tests/builds.
4. Require artifact evidence: diff, logs, screenshots, URLs, and commit SHA.
5. Block promotion if the handoff summary is not inspectable.

Pitfall: a remote chat UI is not a cloud agent runner unless execution is durable and auditable.


## Verification
- Run on a real VinClawLabs task.
- Record paths changed and evidence.
- Promote only if it remains distinct from existing skills.
