# Capability & Execution Model — Public-safe

Status: `PUBLIC_SAFE_SHOWCASE_V0.4`  
Date: 2026-10-05

This note explains one of the main V0.4 changes: Nexus separates **what a system is allowed to do** from **which model or tool performs the computation**.

## Why this separation matters

AI projects often bind a workflow to one prompt, one model or one application. Nexus instead treats execution as a replaceable resource inside a governed project system.

```text
project need
→ bounded capability
→ applicable method / extension
→ execution resource
→ human validation
→ governed result
```

The capability defines the role and constraints. The execution resource supplies computation.

## Reusable core capabilities

The reusable core covers cross-project functions such as:

- source and provenance handling;
- context qualification and routing;
- memory and lineage;
- derivation between source material and usable outputs;
- QA and human validation gates;
- action and follow-up traceability.

The public showcase describes these functions by category. Internal engine names and reconstructive contracts remain private.

## Governed extensions

A project can require knowledge or methods that should not be hard-coded into the core.

Examples include:

- a domain method;
- an occupational workflow;
- a partner-specific process;
- a project overlay;
- an adapter to an external tool or data source.

An extension should therefore retain enough metadata to answer practical questions:

```text
Where did this method come from?
Who has authority over it?
For which tasks is it valid?
Which version is active?
What inputs can it use?
What outputs or actions can it produce?
How was this result derived?
What is its validation status?
```

The current R&D objective is to make these extensions loadable, replaceable and removable without losing provenance or corrupting core memory rules.

This is an architectural direction under active validation, not a claim that Nexus already provides a finished public plug-in marketplace.

## Execution resources

A capability can potentially route to several kinds of execution resources:

### Frontier models
Useful when broad reasoning, language performance, multimodality or rapid access to current model capabilities matters.

### Local or controlled models
Useful when privacy, autonomy, cost control, offline operation or infrastructure sovereignty matters.

### Deterministic tools
Useful for operations that should be reproducible and rule-bound rather than delegated to generative inference.

### Specialised compute or external services
Useful when a task depends on a particular runtime, GPU workload, software environment or connected service.

Nexus treats these as resources with different properties rather than as competing definitions of the whole system.

## A key governance rule

```text
execution location ≠ source authority
compute distribution ≠ decision authority
model output ≠ admitted memory
```

A model can propose a result. The workflow still determines how that result is qualified, reviewed, derived, stored and allowed to influence later work.

## Example

A research-action project may use:

1. an authoritative operational folder maintained by the project;
2. a reusable Nexus capability for provenance and memory;
3. a domain method loaded as a governed extension;
4. a frontier model for one synthesis task;
5. a local model for material that requires tighter control;
6. a human review before publication;
7. a derivative stored with links back to its sources and corrections.

The value being tested is not simply model performance. It is whether the project can change tools and methods while preserving authority, continuity and reconstructibility.

## Current R&D questions

The V0.4 architecture is being tested against questions such as:

- Can a method extension be added or removed without altering core provenance rules?
- Can the same governed capability switch execution resources without changing its project authority?
- Can source, derivative and memory states remain distinguishable after repeated reuse?
- Can the workflow reduce duplicate work and reconstruction effort compared with a less governed baseline?
- Can heterogeneous project contexts reuse capabilities without falsely standardising their local rules?

These remain validation questions. Their outcomes will be documented as evidence becomes available.
