# Phase-one dry-run report

Date: 2026-11-20. Build: 0.2.0 candidate. Environment: hosted Linux/Python; not the user's VS Code installation.

## Results

- 23 automated tests passed: blank origin/resume; refusal to reinitialize; wrong home/identity; role/evidence corruption; missing inventory entries; manifest binding changes; missing parent; duplicate JSON keys; unsupported evidence links; preserved concepts; explicit briefing budget/omissions; immutable inventories/history; Markdown views; non-destructive harness wiring; open interrupted visits; publication readback; stale-head rejection; race-time non-fast-forward rejection; seeded distinct identity/provenance; invalid seed scope refusal.
- Six compatibility checks passed on a disposable copy of Dhriti's preloaded APP-004 memory: existing schema/lineage; protocol upgrade without checkpoint schema conversion; selected-record briefing fidelity/omissions; all four original checkpoint bytes unchanged; supersession preserving IDs/evolution/history; corrupted knowledge rejection.
- A fresh independent local agent recovered Fred from files alone. It identified the synthetic current panel choice (teal), rejected alternative (yellow), and draft-only restriction, attributing them to synthetic evidence rather than user product approval. It accurately reported LIMITED because no remote existed and left a local visit open instead of claiming publication.
- The fresh-agent pass found protocol metadata 0.1.0 inconsistent with the new 0.2.0 instructions. Corrected protocol.json to 0.2.0 before packaging. Checkpoint schema intentionally remains 0.1.0.

The bare-Git transport tests use disposable local remotes. A test-only logical URL adapter allows exercising the production GitHub home check without contacting GitHub. They prove the non-force publication algorithm and readback on Git, not native GitHub authentication.

## Reproduction

```text
python skills/agent-persistent-protocol-skill/scripts/test_app.py
python experiments/test_preloaded_compatibility.py skills/agent-persistent-protocol-skill PATH_TO_DHRITI_MEMORY
```

The second command copies its source, tests the copy and checks source hashes remain unchanged. It can be used on APP-005 as well; fixture assertions about original context remain relevant.

## Limits and pending gates

Native VS Code discovery and every-turn invocation, hooks, compaction handling, independent ChatGPT/Gemini round trips, remote provisioning, and semantic completeness across real tasks remain PENDING. Local synthetic recall is evidence for the tested facts only. Checksums cannot prove understanding or prevent malicious replacement of both data and inventory. No background runtime or universal MCP service is installed. Candidate status remains in effect.
