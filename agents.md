# OpenCode Agents Configuration

## Explore Agent
Used for exploring the codebase structure, finding files, and understanding architecture.

**When to use:**
- Finding files by pattern or name
- Understanding project structure
- Searching for code patterns
- Finding related files

**Configuration:**
- Search patterns: ["apps/*", "packages/*"]
- Exclude: ["node_modules", "dist", ".next", "*.lock"]

## General Agent
Used for implementing features, fixing bugs, and general code changes.

**When to use:**
- Implementing new features
- Bug fixes
- Refactoring
- Writing tests

## Available Subagents

### code-reviewer
For reviewing code changes and ensuring quality.

---

## Project Structure

```
customer-app/
├── apps/
│   ├── web/          # Next.js web application
│   ├── mobile/       # React Native/Expo mobile app
│   └── workers/      # Background workers
├── packages/
│   ├── core/         # Core business logic
│   ├── auth/         # Authentication
│   ├── config/       # Configuration
│   ├── schemas/      # Database schemas
│   ├── types/        # Shared TypeScript types
│   ├── ui/           # UI components
│   └── integrations/ # External integrations
└── infra/
    └── supabase/     # Database migrations & seeds
```

## Key Technologies
- **Package Manager:** pnpm v9.15.0
- **Build Tool:** Turbo
- **Testing:** Vitest
- **Database:** Supabase
- **Frontend:** Next.js, React Native (Expo)
- **Language:** TypeScript
