# Phase-one installation and validation plan

Status: 0.2.0 candidate for host qualification. Date: 2026-11-20.

## Deliverables and boundaries

The protocol repository is the development/release source. Install the versioned skill distribution once into the chosen harness. Normal operation uses only the agent's authoritative memory repository plus its installed package. The memory repository records required protocol/schema versions and a recovery entry, not a runtime dependency on the protocol source repository. Markdown vault views are derived; SQLite remains an optional rebuildable index.

The skill is the lifecycle entry point. Small harness instruction files activate it; this is instruction wiring, not proof of universal hooks or every-turn enforcement. Actual host invocation remains a release gate. Independent security/trust/signatures are later work; SHA-256 does not authenticate a malicious replacement of data and hashes.

## Installation

1. Download `releases/agent-persistent-protocol-skill-0.2.0-candidate.zip` from this repository and verify the adjacent SHA256SUMS.txt. Extract it. Install Python and jsonschema in the intended environment.
2. Use a blank VS Code workspace initially. Choose Codex, Claude Code or Copilot; do not install three copies unnecessarily. Run the extracted `scripts/app.py wire` command from the included references/vscode.md. It installs the folder in the chosen discovery location and merges an APP instruction section without discarding existing instructions.
3. Authenticate Git/GitHub using the host's supported flow. Verify read/write scope for the chosen memory repository. Never put credentials in memory files or prompts. The skill cannot manufacture repository-creation permissions.
4. For Dhriti, use the existing authoritative home GovindarajD/dhriti-architect-spec-to-simu, agent ID dhriti, branch main. Clone into a dedicated memory checkout or use a capable GitHub connector. Do not create a replacement identity or point two divergent remotes at the same identity silently.
5. Read the startup prompt and qualification checklist inside references/vscode.md. Require a pinned commit, checkpoint, source-linked recovery answers and accurate LIMITED/BLOCKED status for unavailable checks.

## Three starting modes

Blank: use init to create a new local identity/mission skeleton, then provision and publish an authorized remote. Seeded: use seed to create a new identity with explicit selected concepts and evidence from a qualified source snapshot; confirm delegated execution authority separately. Resume: load an existing identity from its current remote checkpoint. Moving Dhriti across hosts is resume, not another seeded creation.

Dhriti's APP-001 through APP-004 are retained unchanged. APP-005 records the phase-one requirements and implementation scope. Protocol version 0.2.0 continues to use checkpoint schema 0.1.0. An explicit integrity inventory covers current role/checkpoint, all parent checkpoints and referenced local evidence.

## VS Code acceptance matrix

| Test | Blank Fred | Seeded independent agent | Preloaded Dhriti |
| --- | --- | --- | --- |
| Correct identity/home/owner | Required | Required; distinct from source | Required; retained identity |
| Initial context | Mission/role gaps explicit | Selected scope and provenance | Prior decisions and open questions |
| A saves, B recovers, B saves, A refreshes | Required | Required | Required |
| Concurrent save rejection and retained draft | Required | Required | Required |
| Compaction/old-thread resume | Required | Required | Required |
| Superseded decision and insufficient-context probe | Required | Required | Required |
| Failed network/save and interrupted visit | Required | Required | Required |

Use separate clones/workspaces for A and B. Record actual extension/version, tool capabilities, commits, loaded IDs, probe answers and publication/readback. Run corruption tests only on disposable copies. Do not deliberately corrupt the real Dhriti home. Re-run in ChatGPT and Gemini when actual read/write/validation tools are available; an attachment-only trial proves reconstruction only.

## Release decision

Automated package tests and local recovery may pass while native host tests remain pending. Label the build candidate until chosen hosts demonstrate discovery, per-turn invocation, read/write/readback, source-linked recall, conflict handling and recovery. The agent must not claim perfect memory or checksum its internal understanding. A compact briefing is a declared projection, not silent deletion of canonical knowledge.

## Sources checked

- https://learn.chatgpt.com/docs/build-skills — Codex project discovery under .agents/skills.
- https://code.claude.com/docs/en/skills — Claude Code project discovery under .claude/skills.
- https://code.visualstudio.com/docs/agent-customization/agent-skills — Copilot project discovery under .github/skills; harness distinctions.
- https://github.com/henrydaum/second-brain/blob/main/agent/system_prompt_static.md — inspected application architecture and focused memory injection guidance. No Second Brain code copied or executed. Full memory package behavior is not yet qualified.
