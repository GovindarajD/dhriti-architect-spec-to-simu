# COP Visualizer — Dhriti reverse-briefing and self-check
Date: 2026-11-26 | Status: STAGED, PO-triggered only | Owner: Govi
This is an architect comprehension/coverage check, NOT an APP protocol change, APP validation substitute, automatic activation, or permission to implement.

## Trigger and prerequisites
Only after Govi requests Visualizer ingestion: resume existing Dhriti identity using installed APP skill; pin current remote head and validate manifest/checkpoint/integrity; read intake/visualizer.md, intake/visualizer-architect-blueprint-v0.1.md, and knowledge/visualizer-assignment-2026-11-26-STAGED.md. Load task-relevant prior Spec-to-Simulator concepts from canonical APP memory. Record actual loaded and omitted source paths/IDs. If any source cannot be read, explicitly mark incomplete; do not improvise missing content. APP lifecycle and visit/publishing requirements continue to apply.

## Reverse briefing: demonstrate understanding before architecture work
Dhriti must explain IN HER OWN WORDS to Govi, without copying the blueprint verbatim:
1. What COP Visualizer is, why it is horizontal across COP, and what it is not.
2. The three layers; which layer owns native SVG selection, third-party viewers, project artifacts, pipeline execution truth, simulator execution and traces.
3. What is reportedly implemented in Visualizer Light vs only conceptual or unverified. Explicitly state she has not yet inspected code unless she actually has.
4. The pipeline stage ↔ artifact references model, blank stages, folder-vs-dependency distinction, and how adaptive subloops coexist with deterministic top-level stages.
5. Why Co-Think is persistent collaboration, not merely a setup wizard; distinguish Co-Think, Co-View, Co-Design, Present, Walk & Talk, Walk & Design.
6. Skill vs session mode vs control authority; human interruption, editing approval, and safe resume of presentations.
7. How a simulator tile could render SVG while QEMU or another simulator runs separately; mapping commands/events/state/evidence through a typed adapter; distinguish illustrative animation from validated simulation.
8. Why SQLite visual state, pipeline truth, workspace files, simulator traces and APP memory have different authoritative owners.
9. Open-source reuse candidates and license/compatibility uncertainty.
10. Dhriti's immediate Visualizer assignment, preserved Spec-to-Simulator responsibility, deferred MissionLoop, Codex as engineering collaborator, Dhruv as optional coordinator, Govi as PO.
11. Exactly what she must ask Codex to inspect read-only before proposing changes.
12. What APP has and has not verified, what was ingested, what was omitted, whether a new canonical checkpoint was actually published and remotely read back.

## Coverage ledger (mandatory in Dhriti's response)
For each of the 12 items, report one of:
- GROUNDED: correctly restated and linked to exact source section(s);
- PARTIAL: incomplete or ambiguous; specify missing detail;
- GAP: not present/loaded or contradictory; ask Govi;
- UNVERIFIED IMPLEMENTATION: concept understood but current code/runtime not inspected.
A concept may be GROUNDED while implementation is UNVERIFIED. Do not collapse these statuses into a single "I know everything" claim.
Provide an overall readiness verdict:
- READY FOR ARCHITECTURE DISCOVERY: core concept covered, open implementation evidence clearly identified;
- NEEDS PO CLARIFICATION: material concept/authority disagreement or missing decision;
- BLOCKED: required intake, APP validation, or identity binding unavailable.
Do not claim READY FOR IMPLEMENTATION from intake alone.

## Reverse-check questions to Govi
Ask only material gaps, grouped and prioritized (max 5 at first pass). Explain the consequence of each ambiguity and present the best current interpretation. Govi may confirm/correct/supersede. Capture responses with authority/provenance and feed them into the next APP checkpoint through the installed skill. Never treat silence as approval.

## Codex collaboration awareness
Codex is available in the intended VS Code environment as a coding/discovery agent, not as a verified connected runtime in this chat. Dhriti should first ask Govi which Codex workspace/repository and actual access exist; then issue the read-only discovery brief from the blueprint. Codex must report repository/branch/commit, source path/line evidence, tests and actual host checks, and distinguish Implemented/Partial/Absent/Unverified. Dhriti owns architecture reconciliation, not unapproved code changes. Do not assume LiveLoop is connected until verified.

## Demonstration probes (ask Dhriti to answer, then compare with blueprint)
A. A user clicks a resistor in a circuit SVG and asks an agent to explain it. Identify selection authority, voice, plugin/backend, and evidence limits.
B. A stage shows a PDF, an SVG, and a simulator trace. Identify where bytes live, who owns status, and what Visualizer stores.
C. QEMU stops responding during Walk & Talk. What must the UI and agent do? Do not fabricate state or trace.
D. Govi says "change this diagram" during a presentation. What mode/authority transition is needed before any edit?
E. A second host updates Dhriti's APP checkpoint first. What happens to the stale draft? No force-push, reconcile.
F. A coder reports SVG selection works in Windows unit tests but has never been exercised in browser. How should Dhriti classify it?

## First response format (not an inert form)
1. Identity / pinned commit / loaded checkpoint / actual APP validation status.
2. 2–4 paragraph architectural teach-back with key distinctions.
3. 12-item compact coverage ledger with source references and qualification.
4. Demonstration probe answers and any corrections.
5. Up to five focused PO questions if material gaps remain.
6. Codex discovery handoff proposal; no implementation.
7. Publication status: staged vs validated child checkpoint, exact commit/readback if actually completed.

## Safety / non-destructive scope
No changes to APP protocol repository, identity, existing checkpoint bytes, role, manifest or integrity files by manually editing this intake. Do not self-certify memory quality or protocol compliance. Any official new checkpoint must be created through the installed APP skill with schema/lineage validation, stale-head protection, single-commit publication and remote readback. Preserve original source and any unsaved draft if validation/publishing fails.
