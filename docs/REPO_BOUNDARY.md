# Repository Boundary

Status: canonical

This repository exists to build the MAIM Client Intelligence Workspace Platform as a reusable, multi-client product.

## Product Boundary

The platform provides reusable structure and behavior. Governed client instances provide client-specific truth.

```txt
Platform owns:
shared workspace model
workspace shell and navigation
tenant isolation
client configuration contract
knowledge vault interfaces
AI guidance patterns
reports and milestones
design-system framing
routing and metadata
roles, approvals, and audit rules

Client instance supplies:
identity and brand theme
content and doctrine
journey and deliverables
roadmap and payments
approved assets and source references
client-specific visibility rules
```

No named client is part of the platform architecture.

A client instance may validate a shared pattern, but the pattern becomes part of the platform only after deliberate review confirms that it is reusable, configurable, tenant-safe, and free of client-specific doctrine.

## Ecosystem Boundary

```txt
MAIM teaches.
HAMAL orchestrates.
AMA agents operate.
Hanzo provides AI infrastructure.
Lux provides sovereignty.
This repository provides the reusable Client Intelligence Workspace Platform.
```

The platform may integrate with these systems through explicit contracts. It does not absorb or redefine their doctrine or source code.

## Repository Exclusions

This repository does not contain:

- named-client doctrine, copy, or brand assets as platform defaults
- private client records or unpublished source material
- live credentials or secrets
- unapproved automations
- unrelated MAIM product implementations
- infrastructure owned by another system

## Implementation Boundary

The accepted order is:

1. Platform architecture.
2. Workspace product specification.
3. Reusable client-configuration contract.
4. Frontend MVP shell using client-neutral fixtures.
5. AI and data layer.
6. Governed client instances.

Do not begin with a named-client dashboard or back-fit a client prototype into shared architecture.

## Human Approval Boundary

Human review is required before:

- publishing externally visible copy
- introducing or changing client doctrine
- connecting a live source system
- migrating client data or assets
- enabling payment-related behavior
- promoting a client-specific pattern into the platform
