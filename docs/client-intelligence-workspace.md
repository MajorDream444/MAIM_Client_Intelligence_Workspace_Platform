# MAIM Client Intelligence Workspace Platform Architecture

Status: canonical architecture proposal  
Stage: A — Foundation  
Owner: Major Dream Williams

## 1. Product Definition

The MAIM Client Intelligence Workspace Platform is a reusable, multi-client system that turns complex consulting and knowledge work into a clear, guided client experience.

Its purpose is to answer, at every login:

> Am I moving forward?

The platform makes progress, decisions, knowledge, deliverables, dependencies, payments, and next actions visible without exposing unnecessary internal machinery.

This repository defines the platform. It does not define any single client's doctrine, brand, content, or workspace.

## 2. Architecture Principle

```txt
Platform = reusable structure and behavior
Client instance = configuration and approved client truth
Integration = governed connection to a source system
```

A client instance may validate the platform, but no client instance becomes the platform architecture.

## 3. Platform Responsibilities

The platform owns:

- workspace shell, routing, navigation, and layout contracts
- tenant and client-instance boundaries
- reusable dashboard and progress models
- journey and milestone patterns
- deliverable status and approval patterns
- knowledge vault interfaces
- meeting and voice-note record patterns
- AI coach interaction and recommendation patterns
- reports and weekly-wins patterns
- payment-milestone presentation patterns
- role, permission, visibility, and audit contracts
- design-token and brand-framing slots
- client configuration schema
- source-of-truth mappings and integration contracts
- safety, privacy, review, and publication gates

## 4. Client-Instance Responsibilities

Each client instance supplies, through configuration or governed data:

- client identity and workspace name
- approved logo, colors, type, imagery, and voice
- mission, doctrine, offers, programs, and terminology
- journey stages, milestones, and deliverables
- approved knowledge assets and source references
- project roadmap, dependencies, owners, and payments
- client-visible messages, reports, and recommendations
- rules identifying content that must never be generalized

Client-specific truth must remain outside shared platform copy and shared component logic.

## 5. Multi-Client Model

```txt
MAIM CIW Platform
├── Platform Core
│   ├── Workspace Shell
│   ├── Navigation
│   ├── Identity and Access
│   ├── Progress Engine
│   ├── Knowledge Interfaces
│   ├── AI Guidance
│   ├── Reporting
│   └── Integration Contracts
├── Shared Modules
│   ├── Dashboard
│   ├── Journey
│   ├── Deliverables
│   ├── Knowledge Vault
│   ├── Meetings
│   ├── Roadmap
│   ├── Payments
│   ├── Reports
│   └── Messages
└── Client Instances
    ├── Configuration
    ├── Brand Theme
    ├── Content and Doctrine
    ├── Data Connections
    └── Visibility Rules
```

All modules consume platform contracts plus client configuration. They must not hard-code a client name, client doctrine, brand asset, or project-specific workflow.

## 6. Workspace Lifecycle

1. **Qualify** — confirm the client and engagement fit the workspace model.
2. **Configure** — create the client identity, roles, modules, theme, and visibility rules.
3. **Connect** — map approved systems of record without duplicating authority.
4. **Curate** — approve client-facing knowledge, milestones, and narrative.
5. **Operate** — maintain progress, decisions, actions, reports, and recommendations.
6. **Review** — verify accuracy, permissions, value communication, and client confidence.
7. **Evolve** — promote only intentionally reusable patterns into the platform.
8. **Archive or Transition** — preserve records, revoke access, and follow retention rules.

## 7. Source-of-Truth Model

The platform presents a unified experience while respecting system ownership.

| System | Intended responsibility |
|---|---|
| GitHub | product architecture, code, schemas, versioned configuration, technical decisions |
| Notion | operating manuals, approved narrative documentation, decision records |
| Airtable | structured operational records and cross-workspace tracking |
| Google Drive | approved source assets, documents, reports, and exports |
| MAIM Sites or application runtime | client-facing experience |

An integration must declare:

- authoritative source
- read/write direction
- synchronization frequency
- conflict behavior
- approval requirement
- audit trail
- failure and rollback behavior

No connector may silently become a second source of truth.

## 8. Roles and Visibility

Minimum conceptual roles:

- **Platform Owner** — controls platform architecture and global policy.
- **Workspace Operator** — manages a client instance and its approved information.
- **Contributor** — supplies or updates assigned content and deliverables.
- **Client Member** — views approved client-facing information and completes actions.
- **Reviewer** — approves sensitive content, decisions, or publication.
- **Service Agent** — performs explicitly permitted, logged, and bounded assistance.

Authorization must be tenant-scoped, least-privilege, auditable, and deny-by-default for private or unpublished material.

## 9. AI Boundary

AI may:

- summarize approved source material
- identify dependencies and stalled decisions
- propose next-best actions
- draft weekly reports and business-impact explanations
- assist search and retrieval within authorized content
- recommend reusable patterns for human review

AI may not autonomously:

- publish client doctrine
- expose private records
- approve deliverables or payments
- change source-of-truth records without an authorized workflow
- generalize a client-specific concept into platform doctrine
- send external communications without explicit permission

Every AI output shown as fact must retain source traceability and review status.

## 10. Brand and Design Framing

MAIM provides the product frame: platform identity, system chrome, trust signals, and global interaction standards.

The client provides the workspace experience: approved client logo, theme, voice, imagery, and content.

The design contract must support both without blending them:

```txt
MAIM frame + client experience
```

Global components use semantic design tokens. Client themes map into controlled token slots. Client assets never replace platform governance or leak into another tenant.

## 11. Safety and Governance

Required controls:

- explicit tenant isolation
- least-privilege access
- asset and content approval states
- provenance for client-facing claims
- audit events for material changes
- secret-free repository content
- no private-client fixtures in shared examples
- reversible migrations and integration changes
- human approval for doctrine, payments, external copy, and publication
- retention and offboarding rules before production use

## 12. Stage A Constraints

Stage A is documentation and architecture only.

Allowed:

- architecture documents
- product specifications
- schemas and non-executable examples
- reusable templates
- boundary and safety decisions

Not allowed:

- production deployment
- frontend implementation
- live integrations
- client data migration
- private client assets
- credentials or secrets
- external messages or automated writes

## 13. Stage A Exit Criteria

Stage A is complete when:

- this platform architecture is accepted
- the workspace product specification is accepted
- client configuration and isolation contracts are defined
- platform versus client ownership is unambiguous
- the frontend MVP scope is approved
- integration and AI safety boundaries are approved
- no client-specific doctrine has entered shared platform logic or copy

## 14. Decision Test

Before adding anything to the platform, ask:

1. Is this useful across multiple client instances?
2. Can it be expressed without client-specific doctrine?
3. Can it be configured rather than hard-coded?
4. Does it preserve source ownership and tenant isolation?
5. Is its client-facing effect reviewable and explainable?

If the answer is no, it belongs in a client instance or outside this repository.
