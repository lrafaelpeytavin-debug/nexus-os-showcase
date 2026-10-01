# Architecture Overview — Public-safe

This is intentionally a high-level view.

```text
1. INPUT
   Documents, notes, conversations, project context

2. QUALIFICATION
   Source, provenance, uncertainty, evidence status

3. CONTEXT
   What project is this?
   What is the task?
   What rules and boundaries apply?

4. ROUTING
   Select the appropriate workflow, skill or bounded capability

5. HUMAN GATE
   Review sensitive assumptions, scope and consequential actions

6. QA / RESTITUTION
   Check coherence, limits and traceability
   Produce a usable deliverable

7. MEMORY
   Preserve lineage, decisions, versioning and reusable learning
```

## Design principles

### Provenance before confidence
A result should remain connected to the material and assumptions that produced it.

### Human authority
Consequential actions and sensitive interpretations remain human-gated.

### Memory as infrastructure
The objective is not only to produce an answer, but to keep project knowledge reconstructible over time.

### Local-first where useful
The architecture explores local and controlled runtimes when privacy, autonomy or cost justify them.

### Reuse without pretending universality
Capabilities are reused across contexts, but each terrain keeps its own authority and constraints.

## What is deliberately not published here

The private Nexus repositories contain more detailed contracts, engine snapshots, scripts, tests and deployment logic. Those materials are not part of the public showcase.
