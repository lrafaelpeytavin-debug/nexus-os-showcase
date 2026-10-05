# Architecture Overview — Public-safe

Status: `PUBLIC_SAFE_SHOWCASE_V0.4`  
Date: 2026-10-05

This document exposes the architecture at a level that is useful for evaluation without publishing reconstructive implementation details.

## 1. Operating chain

```text
SOURCE / PROJECT MATERIAL
→ QUALIFICATION
→ CONTEXT
→ CAPABILITY ROUTING
→ EXECUTION RESOURCE
→ HUMAN GATE
→ QA / RESTITUTION
→ MEMORY
→ ACTION / FOLLOW-UP
```

### Source / project material
Documents, notes, conversations, structured data, workshop traces and project context enter with a known or explicitly uncertain origin.

### Qualification
The workflow records provenance, evidence status, uncertainty and the authority attached to the material.

### Context
The system identifies the project, task, applicable rules, audience and disclosure boundaries.

### Capability routing
A bounded capability is selected for the task. This may be a reusable core capability or a governed extension associated with a method, domain, partner or project.

### Execution resource
The selected capability can use a frontier model, a controlled local model, deterministic code, a specialised compute node or another tool. The execution resource performs work inside the governed workflow.

### Human gate
Sensitive interpretation, consequential action, scope changes and publication remain subject to human review.

### QA / restitution
The output is checked for coherence, traceability, audience fit and declared limits before becoming a usable derivative.

### Memory
Lineage, corrections, decisions, versions and reusable learning can be preserved so later work remains reconstructible.

### Action / follow-up
When the task requires it, the validated result can become an explicit next action or follow-up condition rather than disappearing into a static answer.

## 2. Architectural layers

```text
PROJECT AUTHORITY
  source, mandate, rules, ownership

GOVERNANCE LAYER
  provenance, epistemic status, human gates, QA

CAPABILITY LAYER
  reusable core capabilities
  governed extensions / method packs / project overlays

EXECUTION LAYER
  frontier models
  local models
  deterministic tools
  specialised compute / external services

DERIVATION LAYER
  synthesis, report, decision support, pedagogical or public derivative

MEMORY LAYER
  lineage, versioning, corrections, decisions, reusable learning
```

These layers are deliberately separated. Changing the execution model should not silently change source authority, memory policy or the rules of a project.

## 3. Stable core and governed extensions

The architecture distinguishes between capabilities that belong to the reusable operating core and extensions that enter from a specific method, profession, partner or terrain.

A public-safe extension contract can be understood through the following dimensions:

```text
source
→ scope
→ authority
→ expected inputs
→ permitted outputs / actions
→ version
→ validation status
→ provenance of derived work
```

The private implementation contains more detailed schemas and contracts. Those are outside this repository.

This separation supports interoperability without treating every method as universally valid. An extension can be added, revised or removed while the core rules for provenance, human authority and memory remain stable.

## 4. Source authority is not storage location

A recurring design problem is the accidental promotion of copied or generated material.

Nexus therefore separates several questions:

- Where is an artefact stored?
- Which artefact or location is authoritative for the project?
- Is this item a source, a derivative, a hypothesis or a research-action trace?
- Has it been admitted into reusable system memory?
- What actions is it allowed to influence?

A copied file or AI-generated synthesis does not gain authority merely because it is easier to retrieve.

## 5. Model and infrastructure strategy

Nexus is model-agnostic at the architectural level.

Frontier models can provide strong general-purpose reasoning and generation. Local or controlled execution can become preferable for privacy, autonomy, latency, cost or infrastructure reasons. Different tasks can also use different resources in the same governed workflow.

A useful distinction is:

```text
distributed compute ≠ distributed authority
model execution ≠ capability governance
```

Moving inference between machines or providers does not automatically change who is allowed to decide, publish, modify memory or act.

## 6. More than retrieval

Retrieval is one useful mechanism inside the architecture. The broader chain is:

```text
information
→ provenance
→ epistemic status
→ relations
→ authority
→ derivation
→ action
→ trace
```

The design goal is to keep those transitions visible enough for a human to reconstruct why a result exists and what it is allowed to do.

## 7. Design principles

### Provenance before confidence
A result should remain connected to the material, assumptions and transformations that produced it.

### Human authority for consequential transitions
Sensitive interpretations, publication and consequential actions remain human-gated.

### Memory as infrastructure
The objective is to preserve reconstructible project knowledge rather than accumulate disconnected outputs.

### Execution independence
A capability should not be conceptually tied to one model provider when an alternative execution resource can satisfy the same governed role.

### Reuse with bounded authority
Reusable capabilities can travel across contexts while each project preserves its own sources, rules and authority.

### Intelligibility before internal naming
Public representations explain category, function, relations and maturity before internal names.

## 8. Relationship to public KLE surfaces

- **La KLE** is the broader research-action and cooperation ecosystem.
- **Souveraineté en Action** is an experimentation and popular-education field.
- **Enquêtes du Vivant** is a public pedagogical inquiry interface.
- **Nexus OS** is the memory, provenance, derivation, QA and human/AI orchestration layer developed across these kinds of contexts.

The relationship is functional. Each surface retains its own role and authority.

## 9. Current maturity

The architecture mixes several maturity levels:

- **implemented / testable alpha** for selected private components and harnesses;
- **used in real workflows** for documentary memory, provenance, derivation, project continuity and human/AI work;
- **specified and under validation** for reusable capability packaging, heterogeneous execution and extension interoperability;
- **research hypotheses** for comparative performance advantages against simpler AI-assisted baselines.

The public showcase keeps these categories separate.

## 10. What is deliberately not published here

The private Nexus repositories contain detailed contracts, internal capability names, engine snapshots, scripts, tests, partner mappings and deployment logic. Those materials are not part of the public showcase.
