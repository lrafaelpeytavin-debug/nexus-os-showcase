# Nexus OS — Public Showcase

Status: `PUBLIC_SAFE_SHOWCASE_V0.4`  
Date: 2026-10-05  
Purpose: recruiter / partner / funder discovery

> **Public showcase ≠ open-source release.**

This repository is a **sanitized public showcase** of Nexus OS. It is designed for recruiters, partners and funders who need to understand the architecture, the current evidence and the R&D trajectory without access to the private runtime or deployment packages.

## Author and CV — versions du 9 octobre 2026

**Lucas Rafael Benavenuto** — concepteur de systèmes socio-techniques et de dispositifs de coopération, fondateur de La KLE et cofondateur de Souveraineté en Action. Parcours à l'interface de la recherche-action, de l'éducation populaire, de la pédagogie, de l'ingénierie de l'information et des systèmes IA.

**Choisir le CV adapté au besoin du recruteur :**

- **[Général — architecture socio-technique](assets/Lucas_Benavenuto_CV.pdf)** — Profil transversal : gouvernance de l'information, IA, recherche-action, coordination et coopération.
- **[IA / LLMOps et systèmes agents](assets/Lucas_Benavenuto_CV_IA_LLMOps_2026-10-09.pdf)** — Architecture d'agents et de workflows LLM, QA, traçabilité, critères d'acceptation et gouvernance.
- **[Facilitation et capitalisation](assets/Lucas_Benavenuto_CV_Facilitation_2026-10-09.pdf)** — Accompagnement de collectifs, éducation populaire, formation et mémoire des décisions.
- **[Recherche-action et évaluation](assets/Lucas_Benavenuto_CV_RechercheAction_Evaluation_2026-10-09.pdf)** — Enquête participative, analyse des changements, capitalisation et transmission.
- **[Territoires et transition écologique](assets/Lucas_Benavenuto_CV_Territoires_2026-10-09.pdf)** — Animation territoriale, agroécologie, partenariats et conduite de projets.
- **[Habitat participatif et projets coopératifs](assets/Lucas_Benavenuto_CV_HabitatParticipatif_2026-10-09.pdf)** — CV V0.4 sur la DA de référence (photo, bleu marine et vert, deux pages) : facilitation, AJMF, cartographie territoriale, chantiers participatifs et ingénierie documentaire/IA.

[Guide de choix des CV et règles d'actualisation](CV_PORTFOLIO.md) · [La KLE](https://lakle.fr) · [Souveraineté en Action](https://sa.lakle.fr) · [Newsletter Résilience & Synergie](https://www.linkedin.com/newsletters/la-kle-r%C3%A9silience-synergie-7266945786234519552)

**Repères de terrain communiqués par le porteur au 09/10/2026 :** 427 personnes dans la communauté SA ; plus de 160 ayant accepté le règlement et le Contrat blanc pédagogique (rôle-seuil « Travail Souverain ») ; environ 20 rencontres et 180 participations comptées hors répétitions selon un bilan provisoire dont les unités restent à consolider ; newsletter *Résilience & Synergie* à 292 abonnés. Le bilan antérieur du 16/07/2026 (16 ateliers / 169 participations cumulées) demeure une photographie historique et n'est pas directement comparable. Ces chiffres décrivent le dispositif collectif ; ils ne constituent pas des résultats individuels ou des impacts causaux.

Le **CV général** reste le point d'entrée stable du dépôt (`assets/Lucas_Benavenuto_CV.pdf`). Les autres CV sont des représentations ciblées du même parcours, avec des priorités de lecture différentes. Ils n'ajoutent pas de qualifications formelles, de missions accomplies ou de preuves d'industrialisation au-delà des sources.

## What Nexus OS is

Nexus OS is a **human-gated, model-agnostic architecture** for turning heterogeneous project material into structured, traceable and reusable work.

Its role is to govern the transitions between sources, context, capabilities, AI execution, human validation, deliverables, memory and follow-up.

```text
sources and project material
→ qualification, provenance and authority
→ context and routing
→ core capability or governed extension
→ AI / tool execution
→ human gate and QA
→ usable derivative
→ governed memory
→ action or follow-up
```

A language model is therefore an execution resource inside the architecture. It does not become the source of truth, the project authority or the memory policy.

## What changed in V0.4

V0.4 makes several architectural distinctions explicit.

### Stable capabilities and governed extensions

Nexus separates reusable core capabilities from methods or project-specific extensions.

The core covers functions such as provenance, context routing, memory, derivation, QA and human validation. Domain methods, partner workflows or occupational practices can be attached as governed extensions with an explicit scope, version, source, authority and validation status.

This allows reuse across projects while preserving the rules of each terrain.

### Frontier models and local execution

Nexus can use frontier models when their capabilities are useful and controlled local execution when privacy, autonomy, cost or infrastructure constraints justify it.

The architecture is not defined by a particular model provider or deployment mode. Governance, provenance and human authority remain stable when the execution resource changes.

### Source, storage and system memory are different things

A document can be stored in one place while another location remains authoritative for the project. A research-action derivative can inform Nexus without automatically becoming canonical project knowledge.

This separation helps prevent a copied document, a generated synthesis or an imported method from silently acquiring more authority than its source supports.

### Capability routing instead of universal automation

The system selects a bounded capability for a task rather than treating every available method, model or tool as universally applicable.

That routing can include native capabilities, governed method packs, project overlays, adapters and external tools. Their internal contracts remain private; the public principle is documented in [CAPABILITY_AND_EXECUTION_MODEL.md](CAPABILITY_AND_EXECUTION_MODEL.md).

## A concrete public-safe workflow

```text
raw workshop, document or project material
→ identify source, context and authority
→ separate observation, interpretation and hypothesis
→ select the relevant capability or governed extension
→ execute with an appropriate model or tool
→ produce a candidate synthesis or deliverable
→ human review and correction
→ publish or circulate the appropriate derivative
→ preserve lineage, decision and reusable learning
→ trigger the next action when relevant
```

The objective is to make these transitions inspectable, revisable and reconstructible over time.

## More than retrieval

Retrieval is useful, but Nexus is designed around a longer chain:

```text
information
→ provenance
→ epistemic status
→ relationships
→ authority
→ derivation
→ action
→ trace
```

The R&D question is whether governing that chain improves continuity, correction, reconstruction and accountability compared with less structured AI-assisted work.

## Who this showcase is for

### Recruiters
A compact view of concrete capabilities in human/AI system design, structured workflows, provenance, QA, project memory, model routing and prototyping.

### Partners
A high-level view of how Nexus can support a bounded project workflow while keeping source authority, methods, validation and deployment constraints explicit.

### Funders
A reviewable R&D trajectory combining alpha components, instrumented tests, proof-by-use signals, architectural contracts, explicit limitations and comparative validation gates.

## How Nexus connects to public KLE surfaces

These projects are related through their functions:

- **La KLE** — https://lakle.fr — the broader research-action ecosystem and frame in which cooperation, pedagogy and project methods are developed.
- **Souveraineté en Action (SA)** — https://sa.lakle.fr — a field of experimentation and popular education where collective practices, governance and situated learning are tested.
- **Enquêtes du Vivant** — https://enquetesduvivant.lakle.fr — a public pedagogical inquiry interface for exploring collective situations and structuring learning.

Nexus OS is the **memory, provenance, derivation, QA and human/AI orchestration layer** developed across these kinds of contexts. Each public project retains its own function and authority.

## Selected proof-of-use signals

Public-safe snapshot from 2026:

- 31/31 CTX-1A.1 tests validated in one instrumented Nexus sequence;
- 34/34 harness controls validated in another evaluation sequence;
- 14,542 files / 15.37 GB structured as a heterogeneous documentary corpus used for retrieval, provenance, versioning, lineage and capitalisation workflows;
- repeated use across pedagogy, collective intelligence, project structuring, applications and research-action;
- Enquêtes du Vivant beta launched on 20 May 2026 as a practical research-action interface.

The corpus size is not presented as a storage performance metric. The relevant challenge is keeping evolving material retrievable, attributable and reconstructible across projects, formats and derivatives.

These are **implementation and usage signals**, not claims of market superiority or causal business impact.

See [PROOF_OF_USE.md](PROOF_OF_USE.md).

## Current maturity

Nexus is an evolving R&D / product architecture.

Some components have executable alpha implementations and test harnesses in private repositories. Provenance, routing, memory, human gates and documentary workflows have been exercised in real work. The packaging of reusable capabilities and external method packs is an active R&D area rather than a finished plug-in marketplace.

The public showcase intentionally avoids exposing code, schemas and contracts that would materially ease reconstruction of the private system.

See [ARCHITECTURE_OVERVIEW.md](ARCHITECTURE_OVERVIEW.md) and [CAPABILITY_AND_EXECUTION_MODEL.md](CAPABILITY_AND_EXECUTION_MODEL.md).

## Next validation gates

Current public-safe priorities:

1. compare a governed Nexus workflow with a credible baseline such as a frontier model working from a less structured project folder;
2. measure human correction effort, cycle time, duplicate work, provenance loss and reconstruction effort where possible;
3. test the loading, replacement and removal of governed method or project extensions without corrupting core provenance and memory rules;
4. document an additional heterogeneous workflow with explicit before/after and human-correction traces;
5. test whether a zero-context reader can explain what Nexus does, where human authority sits and what remains unproven;
6. add anonymised visual examples only after disclosure review.

## Public projects

- La KLE: https://lakle.fr
- Souveraineté en Action: https://sa.lakle.fr
- Enquêtes du Vivant: https://enquetesduvivant.lakle.fr
- GitHub profile: https://github.com/lrafaelpeytavin-debug

## Boundaries

This repository excludes runtime internals, engine snapshots, reconstructive capability contracts, partner packages, private mappings, sensitive traces, private corpora, credentials and operational deployment know-how.

See [SECURITY_AND_BOUNDARIES.md](SECURITY_AND_BOUNDARIES.md).

## License and reuse

This repository is intentionally published **without an open-source license**.

**Copyright © 2026 Lucas Benavenuto / La KLE. All rights reserved.**

It is available for viewing and evaluation only. Public visibility does not grant permission to copy, modify, redistribute, commercialize or incorporate the contents into another product.

See [NOTICE.md](NOTICE.md) and [COPYRIGHT.md](COPYRIGHT.md).

## Contact

Lucas Benavenuto  
La KLE  
https://lakle.fr
