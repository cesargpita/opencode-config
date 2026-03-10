# Project Context

## Overview
Customer-app is a monorepo containing a web application (Next.js), mobile app (React Native/Expo), and background workers.

## Tech Stack
- **Language:** TypeScript
- **Package Manager:** pnpm
- **Build System:** Turbo
- **Testing:** Vitest
- **Database:** Supabase (PostgreSQL)
- **Auth:** Custom auth package
- **UI:** React + React Native

## Package Manager Notes
- Uses pnpm v9.15.0
- pnpm workspace configuration in `pnpm-workspace.yaml`
- All apps and packages are in workspace

## Testing Notes
- Tests use Vitest
- Test files are co-located: `src/*.test.ts`
- Run tests with `pnpm test`

## Type Checking
- Base config: `tsconfig.base.json`
- Each package/app has its own tsconfig.json
- Run typecheck with `pnpm typecheck`

## Build Notes
- Turbo manages build orchestration
- Build output goes to `dist/` for packages, `.next/` for web app

## Database
- Supabase used for database
- Migrations in `infra/supabase/migrations/`
- Seeds in `infra/supabase/seeds/`
- RLS policies in `infra/supabase/policies/`

## Key Conventions
- Packages use scoped names: `@customer-app/*`
- Follow existing code style in each package
- Write tests for new features
- Run typecheck before committing
