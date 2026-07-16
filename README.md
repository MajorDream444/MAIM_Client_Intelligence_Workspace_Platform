# MAIM Client Intelligence Workspace Platform

Status: Stage A - Foundation
Owner: Major Dream Williams

This repository defines the reusable client workspace platform for MAIM-powered client intelligence systems.

It is not a one-off client portal.

It is the product foundation for repeatable client workspaces where strategy, journey, deliverables, knowledge vaults, reports, and AI-assisted coaching can compound across Client #001, Client #002, Client #003, and beyond.

## Core Principle

```txt
The platform is reusable.
The client workspace is configurable.
The client doctrine is preserved.
```

Sheetal / Shakti may become Client #001, but Sheetal is not the architecture.

## Repository Role

This repo owns:

- client intelligence workspace architecture
- reusable workspace lifecycle
- dashboard and navigation specifications
- client configuration standards
- knowledge vault patterns
- AI coach patterns
- reporting patterns
- future shared frontend shell
- future AI and data layer contracts

This repo does not own:

- MAIM Command Room landing page
- HAMAL doctrine
- AMA agent operating doctrine
- Hanzo source code
- Lux sovereignty implementation
- Shakti-specific doctrine as generic platform copy
- live client automations before approval

## Initial Build Sequence

```txt
PR #1 - Platform Architecture
PR #2 - Workspace Product Specification
PR #3 - Client #001: Sheetal Workspace
PR #4 - Frontend MVP Shell
PR #5 - AI & Data Layer
```

No frontend or live integrations should be added before the architecture and workspace specification are accepted.

## Target Structure

Future structure:

```txt
portal/
  app/
  clients/
    sheetal/
    bali-arena/
    hanzo/
  packages/
    workspace-ui/
    knowledge-vault/
    ai-coach/
    reports/
  docs/
```

This structure is a target, not permission to scaffold everything at once.

## Stage A Safety

Stage A is documentation and architecture only.

No live integrations.
No client data migration.
No Airtable writes.
No Notion writes.
No emails.
No CRM writes.
No secrets.
No frontend implementation yet.

