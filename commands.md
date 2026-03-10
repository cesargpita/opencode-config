# Custom Commands

## Development Commands

| Command | Description |
|---------|-------------|
| `pnpm dev` | Run all apps in parallel |
| `pnpm dev --filter=web` | Run web app only |
| `pnpm dev --filter=mobile` | Run mobile app only |
| `pnpm dev --filter=workers` | Run workers only |

## Build Commands

| Command | Description |
|---------|-------------|
| `pnpm build` | Build all packages and apps |
| `pnpm build --filter=@customer-app/core` | Build core package |
| `pnpm build --filter=@customer-app/ui` | Build UI package |

## Test Commands

| Command | Description |
|---------|-------------|
| `pnpm test` | Run all tests |
| `pnpm test --filter=@customer-app/core` | Run core package tests |
| `pnpm test -- --run` | Run tests once (no watch) |

## Quality Commands

| Command | Description |
|---------|-------------|
| `pnpm typecheck` | Type check all |
| `pnpm lint` | Lint all |
| `pnpm typecheck --filter=web` | Type check web app |

## Database Commands

| Command | Description |
|---------|-------------|
| Supabase CLI needed for migrations | See `infra/supabase/` |

## Notes
- All commands run from root using pnpm
- Use `--filter` to target specific packages/apps
- Turbo handles caching and parallelization
