# MAIM Client Intelligence Workspace Platform

Status: Stage A — Foundation  
Owner: Major Dream Williams

This repository defines the reusable, multi-client platform architecture for MAIM-powered Client Intelligence Workspaces.

It is not a client portal and does not contain a specific client's brand, doctrine, content, assets, or implementation.

## Core Principle

```txt
The platform is reusable.
The client instance is configurable.
Client truth remains client-specific.
```

## Repository Role

This repository owns:

- platform architecture and lifecycle
- multi-client and tenant-isolation contracts
- workspace shell and navigation specifications
- reusable module and component contracts
- client-configuration standards
- knowledge vault, AI guidance, and reporting patterns
- role, permission, visibility, and audit rules
- design-system framing and client-theme slots
- source-of-truth and integration contracts
- future shared frontend, AI, and data-layer implementation

This repository does not own:

- any individual client's doctrine, brand, copy, or assets
- MAIM Command Room implementation
- HAMAL or AMA operating doctrine
- Hanzo or Lux source code
- live client automations before approval
- private client data or unpublished source material

## Canonical Architecture

Read [docs/client-intelligence-workspace.md](docs/client-intelligence-workspace.md) first.

It defines the platform boundary, multi-client model, lifecycle, source-of-truth rules, AI boundary, brand framing, safety requirements, and Stage A exit criteria.

## Initial Build Sequence

```txt
PR #1 — Platform Architecture
PR #2 — Workspace Product Specification
PR #3 — Client Configuration Contract
PR #4 — Frontend MVP Shell
PR #5 — AI & Data Layer
PR #6+ — Governed Client Instances
```

A named client workspace is created only after the reusable configuration contract is accepted. Client-specific work belongs in an isolated client-instance area, not in platform architecture or shared copy.

## Target Structure

```txt
app/
  platform/
  workspaces/
packages/
  workspace-ui/
  client-config/
  knowledge-vault/
  ai-coach/
  reports/
docs/
  client-intelligence-workspace.md
  product-specification.md
  client-configuration-contract.md
clients/
  .gitkeep
```

The structure is directional and does not authorize implementation during Stage A.

## Stage A Safety

Stage A is documentation and architecture only.

No frontend implementation.  
No production deployment.  
No live integrations or system writes.  
No client data migration.  
No private client assets.  
No external messages.  
No secrets.
