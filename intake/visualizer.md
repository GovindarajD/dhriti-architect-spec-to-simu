# Dhriti intake — COP Visualizer
Status: PENDING INGESTION (not an APP checkpoint)
Date: 2026-11-26
Authority: Govi, Product Owner
Agent binding: dhriti | GovindarajD/dhriti-architect-spec-to-simu | main

## When to use
After Dhriti is first loaded and recovered in the new VS Code/Codex network, Govi may say: "Dhriti, ingest intake/visualizer.md and take up the COP Visualizer architecture assignment." Do NOT auto-activate this intake before Govi requests it. This document is a task intake, not an agent identity, system prompt, or modification to APP protocol.

## Required reading
1. First follow existing AGENTS.md, manifests/app.json and the installed agent-persistent-protocol-skill@0.2.0 to resume the existing Dhriti identity. Pin the current remote commit, validate checkpoint/integrity, and report limitations.
2. Read the comprehensive [architect blueprint](visualizer-architect-blueprint-v0.1.md), including its architecture diagrams, component boundaries, simulator tile/adapter design, interaction model, decisions, evidence categories and open questions. This is staged conceptual design, not a validated implementation baseline.\n3. Read the full source briefing: [Visualizer assignment context](../knowledge/visualizer-assignment-2026-11-26-STAGED.md). Treat its PO decisions, proposals and unverified implementation claims distinctly.
4. Load relevant prior Spec-to-Simulator concepts from the canonical checkpoint; preserve them. Do not discard or overwrite APP-001 through APP-005.
5. If the Visualizer repository is available, ask Codex for read-only code-level discovery before asserting implemented behavior. Do not begin implementation without PO authorization.

## Assignment
COP Visualizer is the immediate architecture priority. Spec-to-Simulator remains a subsequent, preserved responsibility; simulation will be one potential plugin of the horizontal Visualizer. MissionLoop is deferred from this intake. Dhriti should reconcile the conceptual baseline against real Visualizer Light code, then propose a PO-reviewable architecture and reuse strategy.

## Architecture guardrails
Visualizer is the visual access/control plane, NOT the engineering workspace. Layer 1 owns metadata and workflow visualization, native SVG selection/control, modes and agent commands. Layer 2 hosts pluggable viewers/whiteboards/engineering simulators. Layer 3 is the real VS Code/files/CLI/skills/simulator environment. Pipeline Management owns execution semantics; project files own artifact content. Reuse external viewers, do not rebuild Office or CAD. Human retains interrupt and approval authority. Proposed modes include Walk & Talk, Walk & Design, Co-Think, Co-View, Co-Design and Present. Defer gestures and deep tool-specific editing.

## APP publication boundary
This intake and the linked STAGED briefing are NOT listed in APP-005's manifest/integrity and are NOT canonical APP memory. On Govi's explicit instruction, Dhriti should use the installed APP skill to ingest with provenance and publish a validated immutable child checkpoint plus manifest and integrity inventory atomically with stale-head protection, followed by remote readback. If tools or host qualification are unavailable, report PENDING/BLOCKED and retain the source; never claim publication or perfect memory.

## First response after ingestion request
Report (a) pinned identity/home/checkpoint, (b) loaded and omitted source IDs, (c) Visualizer assignment summary and retained Spec-to-Simulator scope, (d) APP publication status, and (e) next evidence request to Codex. Do not treat successful cloning as proof of full APP host qualification.
