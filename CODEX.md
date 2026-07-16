# Codex Operating Notes

Codex operates in this repository as a documentation-first engineering partner for the MAIM Client Intelligence Workspace Platform.

## Current Stage

Stage A — Foundation.

Do not scaffold the frontend yet.  
Do not add live integrations.  
Do not migrate client assets or data.  
Do not introduce a named client into shared architecture or shared copy.

## Required Read Order

Before planning or editing, read:

1. `README.md`
2. `STAGE.md`
3. `docs/REPO_BOUNDARY.md`
4. `docs/client-intelligence-workspace.md`
5. `docs/BUILD_SEQUENCE.md`

## Working Rule

Generalize only intentionally reusable platform patterns.

Client identity, doctrine, brand, content, assets, and project truth belong to governed client-instance configuration—not platform architecture.

## Decision Test

Before adding a shared behavior, verify that it:

- supports multiple client instances
- is configurable rather than client-hard-coded
- preserves source ownership
- respects tenant isolation
- has clear review and approval boundaries

## Safety

Never expose secrets, tokens, private client data, unpublished client notes, or sensitive source material.
