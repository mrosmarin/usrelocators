# Nobody Move Workspace

This repository workspace contains the active development environment and project context for the Nobody Move CRM platform.

## What We Are Developing

The primary application is in `quiet-carry-core/`.

Current product focus is an MVP relocation CRM and consumer experience platform with:
- A shared **12-stage transition journey** across consumer and professional views
- Consumer onboarding and guided dashboard flows
- Professional CRM tools (client tracking, alerts, touchpoints)
- Document/tip-sheet delivery and decision-support tools
- Stress-score and threshold alert behaviors
- Vendor/care package operations
- Integration track for Stripe, Google OAuth, email, Calendly, and Claude
- Pilot readiness workflows (QA, launch gates, blocker tracking)

Planning and backlog execution are aligned in Linear under team `Nobodymove`.

## Development Environment

This workspace runs in a containerized dev environment.

- Root workspace: `usrelocators`
- Main app path: `quiet-carry-core/`
- Frontend stack: Vite + React + TypeScript + Tailwind + shadcn/ui
- Data/backend integration: Supabase client + edge functions (project-specific)
- Task/backlog tooling: Linear integration configured via `.kilo/kilo.json`

## Local Development (App)

From `quiet-carry-core/`:

```bash
npm install
npm run dev
```

Useful scripts:

```bash
npm run build
npm run lint
npm run preview
```

## Key Project Docs

Use these as implementation source-of-truth over scaffold README content:
- `quiet-carry-core/docs/PLAN-12-Stage-Journey-Update.md`
- `quiet-carry-core/docs/FEATURES-ACTIVATION-AND-SHEETS.md`

## Notes

- Prioritization model: `P0 / P1 / P2 / P3`
- Estimation model: story points
- New Linear issues default to unassigned at creation
- Memory Bank is initialized under `memory-bank/` for ongoing project continuity
