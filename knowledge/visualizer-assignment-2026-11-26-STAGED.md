# COP Visualizer — Architect assignment context (staged for APP ingestion)
Date: 2026-11-26
Authority: Govi, Product Owner
Recipient: Dhriti (existing identity dhriti)
Status: PO-directed assignment; STAGED CONTEXT ONLY, not an APP checkpoint or proof of completed APP resume.
Source: Visualizer concept discussion with Master Architect, November 2026. This is an attributed synthesis, not verified implementation evidence.

## Assignment and precedence
Dhriti's first active engineering architecture assignment on the receiving VS Code/Codex network is COP Visualizer. Preserve her existing Spec-to-Simulator mission, identity, lineage, concepts, and all prior APP checkpoints; Spec-to-Simulator is subsequent work, not cancelled. Simulation is expected to be a reusable Visualizer plugin/integration. Dhruv may coordinate, Codex investigates and implements only when authorized; Govi retains approval authority. MissionLoop is out of immediate scope. This file is project-specific context, not a replacement identity/system prompt.

## Vision and architectural baseline
COP Visualizer is a metadata-first, skill-controlled, multimodal visual access and control plane over an existing engineering workspace, NOT the workspace or authoritative owner of deliverable content. It is a horizontal COP capability usable by Spec-to-Simulator, SDLC, Co-Think, and other projects.

Three layers:
1. Native control plane: pipeline metadata visualization, stage hierarchy and relationships, browser dashboard, navigation, native SVG rendering and deterministic element selection, agent-accessible visual actions, context, modes, control authority, persistent visual state. Existing Visualizer Light functionality must be preserved.
2. Pluggable viewers/engines: whiteboards (Excalidraw/tldraw etc.), Markdown/PDF/Office viewers, circuit/CAD viewers, simulators. Use existing viewers instead of reimplementing document editors. Declare actual plugin capabilities; no fictitious deep editing. Native SVG belongs to layer 1; advanced third-party whiteboard engine belongs to layer 2.
3. Existing workspace/execution: VS Code, project folders, Git, CLI, agent harnesses, skills, document generation, simulation tools and storage. Artifacts are created/modified here, not in Visualizer metadata.

Pipeline Management is an already existing separate skill with JSON manifests and dynamic orchestration; pipeline owns execution semantics, stages, prerequisites and approval gates, NOT artifact content. Visualizer projects its state, does not become a second pipeline authority. Stage nodes initially may be blank and can reference multiple files/folders. Folders organize artifacts; explicit metadata defines sequencing/branches/approvals rather than relying on folder names. Deterministic top-level pipeline can contain adaptive/pattern-driven exploratory subloops. A typical example: requirements intake → analysis/review → design → test scripts/data → test execution/reporting, with RTM and defect feedback loops.

SQLite is the candidate persistent visual/metadata store, with JSON definitions/import/export possible. Existing Visualizer Light is reported to have SQLite persistence, journal/revisions/checkpoints/replay, SVG element identity/selection, browser tabs/tiles, skill/API, and element-level LLM editing. These are discussion-reported features requiring code-level confirmation, not acceptance evidence. Files remain in project directories. Do not claim SQLite is automatically an encrypted security vault.

Brainstorm/Co-Think is a common ongoing tool, not only a one-time setup wizard. Setup can discuss project objectives, pipeline type, folder structure, roles, approvals, then instantiate empty stage references. Co-Think, Co-Design and Co-View can operate in any stage. Temporary exploratory visual thinking need not become a formal deliverable, but can be persisted and later promoted.

## Interaction and control model
Skills invoke behaviors dynamically; do not force manual mode selection. Distinguish skill capability, active session mode and control authority. Human can interrupt and reclaim control. Proposed modes:
- Present: largely noninteractive prepared playback.
- Walk & Talk: agent/human navigates, highlights, explains and answers questions; no design modifications.
- Walk & Design: pause walkthrough, propose/authorize design changes, modify using available tools, resume.
- Co-View: inspect/discuss without editing.
- Co-Think: exploratory collaboration.
- Co-Design: shared authorized editing.
Selection of one deterministic SVG element is sufficient for phase one; gestures and complex multi-element interpretation deferred. Prefer structured visualizer APIs for control; computer use is fallback/visual verification, not primary deterministic actuation. Voice skill is reported already working with coding agents; verify actual integration. Show & Tell may animate a circuit, but engineering-accurate behavior requires simulator/model evidence; illustration is not simulation. Recording/replay of visual walkthrough is a proposal.

## Open-source reuse shortlist (not approved)
React Flow/xyflow for pipeline graph; Excalidraw for whiteboarding; tldraw for advanced agent canvas subject to production license; Freero for collaborative/agent-capable board. These are investigation candidates, not verified compatibility or approved dependencies. Avoid UI reinvention and do not replace Visualizer Light without evidence.

## Initial assignment to Codex (read-only)
Inventory actual Visualizer repository, commit/branch, tests, frontend/backend, SQLite schema, SVG selection API, Visualizer skill, pipeline-management manifests, voice/computer use, browser/VS Code integration, and missing capabilities. Classify Implemented/Partial/Absent/Unverified with file/line evidence. Inspect viewer integration and licensing. No code edits, dependency installation, database migration, release, or field-environment changes. Produce evidence-based capability matrix and architecture reconciliation.

## Dhriti bootstrap and APP safety
Existing authoritative home: GovindarajD/dhriti-architect-spec-to-simu, agent ID dhriti, branch main. Follow AGENTS.md, manifests/app.json, installed agent-persistent-protocol-skill@0.2.0, and current checkpoint/integrity. The protocol source repository is NOT a normal runtime dependency and MUST NOT be modified. Native host invocation/cross-host recovery remain unqualified as of the inspected APP-005 evidence. A new network should RESUME the existing Dhriti identity, not seed or recreate it. The receiving agent must validate identity, pin remote commit, load relevant concepts/evidence, and honestly report gaps.

IMPORTANT: This staged briefing is not referenced by the APP-005 manifest/integrity and does not alter canonical APP state. Before claiming APP persistence or active-focus change, an authorized, skill-equipped Dhriti host must ingest this source with attribution and publish a validated immutable child checkpoint + manifest + integrity in one stale-head-protected commit, verify remote readback, and preserve previous checkpoints. Do not manually edit APP-005 or pretend this file alone completes that lifecycle.

## Decisions and unknowns
PO direction: prioritize Visualizer architecture first; retain Spec-to-Simulator knowledge and later mission. No implementation authorization. Existing code reality, APP host qualification, LiveLoop availability on the new network, plugin API fidelity, remote multi-human collaboration, and exact POC choice remain to be established. Do not conflate architecture proposal with implementation.
