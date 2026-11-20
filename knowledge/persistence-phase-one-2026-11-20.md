# Persistence phase-one direction — 20 November 2026

This is a concept-level record of the available conversation, not a verbatim transcript. Author: current ChatGPT assistant preparing memory on behalf of Dhriti; the author remains distinct from Dhriti. Govi authorized building the starter skill, updating this home and providing a VS Code plan. No VS Code test had previously been established.

## User decisions

1. Treat GovindarajD/agent-persistent-memory as protocol source/release development. Distribute a versioned, self-contained skill. Normal agent operation must not depend on that source repository being accessible.
2. Install the skill in the chosen harness with explicit entry wiring. The agent's own Git memory home remains authoritative; local harness context/indexes are working caches. Remember protocol version/schema in the home. Copying a repository to another network requires an explicit authoritative-home decision.
3. Support both blank creation and seeded/delegated creation of a distinct agent from selected knowledge/work. These differ from resuming Dhriti's existing identity. Preserve provenance and explicit scope; do not silently clone identity/authority.
4. Make memory quality central to phase one: capture decisions, reasons, requirements, pending actions, proposals and contradictions; preserve source attribution and superseded history; retrieve enough task context and report omissions. Use bounded briefings, not unbounded transcript loading.
5. Keep structured files in Git; retain canonical JSON checkpoints and derived Markdown views for later Obsidian inspection. SQLite can be an optional local index later. ZIP was an analogy for checksum checks; no ZIP-only memory requirement was made. A downloadable skill archive is a distribution convenience.
6. Qualify live working context against persisted context at resume and publication. Verify identity/home, lineage, expected hashes, freshness, supplied/omitted concept IDs and task-specific meaning probes. Checksums do not prove model understanding. Report LIMITED/BLOCKED gaps, recover from sources and ask the human when necessary.
7. Phase one assumes protected Git access. Stronger privacy, trust roots/signatures and deliberate-tamper resistance are later phases. Password protection alone does not prevent prompt injection; hashes do not authenticate a maliciously replaced inventory.
8. Checkpoint meaningful work during activity and at exit, publish atomically with stale-head protection, verify readback and preserve unsaved drafts. No automatic background work after host termination is promised.
9. Test a disposable Fred agent, Dhriti's preloaded memory compatibility, new seeded identities and two-instance continuity. Native VS Code/ChatGPT/Gemini invocation remains a qualification requirement, not a claim established by local tests.

## Current implementation evidence

See experiments/PHASE_ONE_QUALIFICATION.md and procedures/VS_CODE_PHASE_ONE_PLAN.md. Candidate protocol 0.2.0 deliberately retains checkpoint schema 0.1.0. APP-001 through APP-004 are unchanged. A generated briefing declares selected and omitted records; it does not rewrite or silently compact canonical knowledge. No Second Brain code was copied; its application architecture and focused-memory pattern were inspected, with full memory-package behavior still unqualified.
