# OpenCode Skills Configuration

## Available Skills

No custom skills currently configured. 

---

## Project Commands

The following commands are available via npm/pnpm:

```bash
# Development
pnpm dev              # Run all apps in parallel
pnpm dev --filter=web # Run only web app

# Build
pnpm build            # Build all packages/apps
pnpm build --filter=@customer-app/core  # Build specific package

# Testing
pnpm test             # Run all tests
pnpm test --filter=@customer-app/core   # Test specific package

# Type checking
pnpm typecheck        # Type check all

# Linting
pnpm lint             # Lint all

# Individual apps
cd apps/web && pnpm dev    # Next.js web
cd apps/mobile && pnpm dev # Expo mobile
cd apps/workers && pnpm dev # Workers
```

## Testing Framework
- **Framework:** Vitest
- **Location:** Tests typically co-located with source files (*.test.ts)

## Package Structure
- Apps: `apps/web`, `apps/mobile`, `apps/workers`
- Packages: `packages/core`, `packages/auth`, `packages/config`, `packages/schemas`, `packages/types`, `packages/ui`, `packages/integrations`
