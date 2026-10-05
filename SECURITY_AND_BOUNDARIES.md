# Security, IP and disclosure boundaries

Status: `PUBLIC_SAFE_SHOWCASE_V0.4`  
Date: 2026-10-05

This repository is designed for broad external viewing while preserving the private implementation, partner material and research-action boundaries of Nexus OS.

## What can be public

The showcase may expose:

- high-level architectural layers and operating chains;
- public-safe diagrams and synthetic examples;
- capability categories without reconstructive internals;
- execution strategy at the level of frontier, local, deterministic and specialised resources;
- selected proof-by-use summaries;
- public project links;
- maturity statements, validation questions and epistemic limits.

## What remains controlled

The following stay private or controlled when disclosure would expose people, partner material or materially ease reconstruction of the system:

- engine source snapshots and executable runtime internals;
- detailed capability and execution schemas;
- private internal engine names and mappings;
- method-pack contracts when they contain protected or reconstructive implementation logic;
- private skills, prompts and operational policies;
- partner deployment packages and partner-specific overlays;
- private project traces and corpora;
- research-action material that could identify people or expose sensitive situations;
- credentials, tokens and operational secrets;
- deployment know-how not intended for public release.

## Source authority and disclosure

Public availability does not make an artefact authoritative for a private project.

The architecture distinguishes:

```text
storage location
≠ project authority
≠ research-action derivative
≠ reusable system memory
```

A public derivative may describe a project without replacing its operational source of truth.

## Public abstraction rule

A public document should expose enough structure to make the work understandable and evaluable while withholding implementation detail that would materially lower the effort required to reconstruct the private system.

For V0.4 this means the showcase can explain the distinction between core capabilities, governed extensions and execution resources. It does not publish the complete contracts that implement those distinctions.

## Repository family

The public showcase is intentionally separate from:

- the private controlled technical kit;
- private partner deployment packages;
- local/runtime workspaces;
- research-action memory and operational project sources.

Public visibility of this showcase does not grant rights to the private Nexus codebase, private methods or private project material.
