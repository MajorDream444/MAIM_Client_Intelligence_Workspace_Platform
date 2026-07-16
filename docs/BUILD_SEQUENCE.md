# Build Sequence

Status: proposed operating sequence

This repo should grow through small pull requests, not one oversized implementation.

## PR #1 - Platform Architecture

Creates:

```txt
docs/client-intelligence-workspace.md
```

Defines:

- product vision
- multi-client architecture
- workspace lifecycle
- shared versus client-specific ownership
- client onboarding stages
- Stage A safety rules

## PR #2 - Workspace Product Specification

Defines:

- dashboard
- journey
- deliverables
- knowledge vault
- AI coach
- reports
- navigation
- UX flows
- role boundaries

## PR #3 - Client #001: Sheetal Workspace

Creates the first client workspace specification.

Possible future location:

```txt
portal/clients/sheetal/
```

Defines:

- configuration
- branding
- content map
- doctrine boundaries
- initial roadmap
- what must remain client-specific
- what can become reusable platform behavior

## PR #4 - Frontend MVP Shell

Only after PR #1 through PR #3 are accepted.

Defines or implements:

- app shell
- shared layout
- dashboard components
- navigation
- reusable client template

## PR #5 - AI & Data Layer

Only after the MVP shell is approved.

Defines:

- workspace metadata
- vault integration
- Airtable mappings
- GitHub source-of-truth synchronization
- future agent hooks
- dry-run boundaries

## Rule

Do not skip from architecture to automation.

The platform should prove the model before it connects live systems.

