# Coding Guidelines

## General
- Use TypeScript for all code
- Follow existing code style in each package
- Add types for all function parameters and return values
- No comments unless absolutely necessary (user didn't request them)

## Testing
- Write tests for new features using Vitest
- Co-locate tests with source files: `src/index.test.ts`
- Use descriptive test names

## Packages
- Core business logic: `packages/core/`
- Authentication: `packages/auth/`
- Shared types: `packages/types/`
- UI components: `packages/ui/`
- Database schemas: `packages/schemas/`
- External integrations: `packages/integrations/`

## Apps
- Web (Next.js): `apps/web/`
- Mobile (Expo): `apps/mobile/`
- Workers: `apps/workers/`

## Imports
- Use package imports: `import { something } from '@customer-app/core'`
- Avoid relative imports across packages

## Before Committing
1. Run `pnpm typecheck`
2. Run `pnpm lint` (if available)
3. Run `pnpm test`
4. Ensure build passes: `pnpm build`
