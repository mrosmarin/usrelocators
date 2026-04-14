# System Patterns

## Architecture Snapshot
- Frontend: React + TypeScript app (Vite).
- Data/backend patterns: Supabase-backed flows, including edge functions for selected operations.
- Planning/execution ops: Linear backlog with project/epic/story hierarchy.

## Key Domain Pattern: Journey as Shared Constant Model
A single source of truth is expected for journey phases and sequence mappings, consumed by:
- Consumer journey views
- Dashboard/AgentHub phase calculations
- CRM phase displays/cards/filters
- Vault/workbook phase grouping

## Current Journey Pattern (Target)
- Migrate from legacy 7-phase assumptions to 12-stage model.
- Preserve progress derivation from existing workbook section sequence values (1-18, 100, 101).
- Use mapping layer rather than immediate DB schema expansion where possible.

## Operational Pattern: Activation Code Flow
- `profiles.activation_code` supports agent activation links.
- Edge functions:
  - `ensure-agent-activation-code` (JWT required)
  - `resolve-activation-code` (public for sign-up link resolution)

## Delivery Management Pattern
- Linear structure: Projects -> Epics -> Stories/Tasks.
- Issue template sections: Context, Scope, Acceptance Criteria, Dependencies, Out of Scope.
- Priority model: P0/P1/P2/P3.
