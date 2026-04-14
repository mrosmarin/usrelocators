# Tech Context

## Stack
- Vite
- React 18
- TypeScript
- Tailwind CSS + shadcn/ui + Radix
- Supabase JS client and edge functions
- React Query, React Router

## Repository Context
- Main working app: `quiet-carry-core`
- Existing docs with strongest implementation signal:
  - `quiet-carry-core/docs/PLAN-12-Stage-Journey-Update.md`
  - `quiet-carry-core/docs/FEATURES-ACTIVATION-AND-SHEETS.md`
- `quiet-carry-core/README.md` is generic scaffold guidance, low signal for product decisions.

## Tooling and Ops
- Node-based frontend scripts (`npm run dev`, `build`, `lint`, `preview`).
- Linear integration available via local MCP config in `.kilo/kilo.json`.

## Constraints
- Preserve compatibility with existing sequence-based workbook progress data during journey migration.
- Maintain role/permission safety while expanding workflows.
- Keep backlog metadata aligned to confirmed planning conventions (story points, P0-P3, unassigned).
