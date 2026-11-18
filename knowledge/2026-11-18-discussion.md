# Design discussion checkpoint

## C07

Status accepted.

Govi clarified that a sandbox is an instantiated breadboard-like environment with identity, typed ports, attached tools, retained experiment state and lifecycle controls. Multiple named instances preserve their own state and connect through declared interfaces. A shared harness was proposed.

Next action Confirm lifecycle and port contract before coding.

## C08

Status accepted.

Specification work is an exploratory sandbox assembling use cases, architecture knowledge, research evidence and assumptions into a cohesive, testable specification. Entry and exit criteria qualify outputs; the agent chooses actions within the active focus.

Next action Define spec qualification checks and the smallest experiment.

## C09

Status accepted.

Model an ecosystem through product, environment/behavior and communication roles. Select replay, synthetic signals, mathematical models, emulation or real hardware per component and purpose. Candidate tools such as QEMU, SPICE, OpenModelica, Simulink and Gazebo require capability checks for the exact target. No i.MX board support has been established.

Next action Declare fidelity, signal ownership, timing and valid test conclusions for each assembly.

## C10

Status accepted.

Provide a common visual sandbox view with inputs left, outputs right, human/library references above and sources below. Show declared wiring and observed probe state, provenance and mismatch. Preserve native tool UIs for detailed inspection. Begin with one spec sandbox and then compose its qualified output with assembly.

Next action Specify a small SVG-based view driven by actual state and probes.

## C11

Status proposed.

A local Python service and browser dashboard were proposed. Govi questioned web services at the pause point. Transport choice remains unresolved. A Windows-native lightweight wrapper between folders and heavyweight deployment is the goal.

Next action Resume Govi's web-interface concern before selecting REST, CLI, in-process or IPC.

## C12

Status accepted.

Govi requested reusable agent-persistent-protocol-skill and repository entry/exit updates for Dhriti. Use canonical versioned JSON with schema and validator, concept-level notes, parent lineage and attributed evidence. Keep client, harness and execution environment distinct. Runtime SIP/background awareness remains future work.

Next action Run independent recovery on another harness using the saved repository.

## C13

Status proposed.

Second Brain was reviewed as a possible self-hosted memory/runtime component. APP's cross-host checkpoint contract remains the chosen development direction. Second Brain integration and native app automated handoffs have not been qualified.

Next action Evaluate only when a concrete APP host integration is needed.

REA requires a compatible authorized artifact for a scoped reverse-engineering question. Research Loop gathers sources. Craft Anything is a candidate build aid. Their integration remains unverified. Knowledge Hub and pattern library are planned connectors. The earlier dialysis fault timing experiment remains a candidate with unresolved baseline criteria. New spec-sandbox experiments have been discussed, with no final component selection.
