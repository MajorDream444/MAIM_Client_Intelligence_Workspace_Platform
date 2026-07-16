# Build Sequence

Status: canonical operating sequence

This repository grows through focused pull requests. Platform contracts are accepted before client instances or integrations are implemented.

## PR #1 — Platform Architecture

Creates:

```txt
docs/client-intelligence-workspace.md
```

Defines:

- product boundary and vision
- multi-client architecture
- platform versus client-instance ownership
- workspace lifecycle
- source-of-truth model
- roles and visibility
- AI and design-system boundaries
- Stage A safety and exit criteria

## PR #2 — Workspace Product Specification

Defines:

- dashboard
- journey
- deliverables
- knowledge vault
- meetings
- roadmap
- AI coach
- payments
- reports
- messages
- navigation and UX flows
- component and role boundaries

## PR #3 — Client Configuration Contract

Defines the reusable schema required to create any governed client instance:

- identity and workspace metadata
- brand-theme token mapping
- module enablement
- navigation configuration
- client-content references
- doctrine and terminology boundaries
- roles and visibility
- source mappings
- approval states
- isolation and validation rules

No named client is part of the platform architecture.

## PR #4 — Frontend MVP Shell

Begins only after PR #1 through PR #3 are accepted.

Defines or implements:

- platform app shell
- shared layout and navigation
- reusable workspace components
- configuration-driven theming
- tenant-safe routing
- approved sample fixtures containing no private client data

## PR #5 — AI & Data Layer

Begins only after the MVP shell and governance contracts are approved.

Defines:

- workspace metadata
- vault interfaces
- connector mappings
- GitHub source-of-truth synchronization
- agent hooks and permissions
- provenance and audit events
- dry-run, approval, and rollback boundaries

## PR #6+ — Governed Client Instances

A named client workspace may be introduced only through the accepted configuration contract and in an isolated client-instance area.

Client doctrine, content, brand assets, and private data must never be committed as shared platform defaults.

## Rule

Do not skip from architecture to automation.

The platform proves its reusable model, safety boundaries, and configuration contract before connecting live systems or introducing named clients.
