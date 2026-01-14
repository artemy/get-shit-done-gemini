# Coding Conventions

**Analysis Date:** 2026-01-14

## Naming Patterns

**Files:**
- `kebab-case` for all files (e.g., `new-project.md`, `install.js`)
- `UPPERCASE.md` for project root files

**Functions:**
- `camelCase` for JavaScript functions in `bin/install.js`

**Variables:**
- `camelCase` for JavaScript variables
- `CAPS_UNDERSCORES` for environment variables and bash-like parameters in workflows

**Commands:**
- `gsd:kebab-case` (e.g., `/gsd:map-codebase`)

## Code Style

**Formatting:**
- 2 space indentation
- Single quotes for JavaScript strings
- Semicolons required in JavaScript
- XML-like tags for prompt structure (`<objective>`, `<process>`)

**Tone:**
- Professional, direct, and imperative
- No conversational filler
- Focus on clarity and safety

## Import Organization

**JavaScript:**
- Node.js built-ins first
- Alphabetical order preferred

**Markdown/Prompts:**
- References listed in `<execution_context>` using `@path` notation

## Error Handling

**Patterns:**
- Synchronous `try/catch` or check-and-exit in `bin/install.js`
- Defensive checks in bash scripts (e.g., `[ -f file ] || exit 1`)
- Validation gates in workflows

## Logging

**Patterns:**
- `console.log` for user feedback in installer
- Markdown-based state logging in `.planning/` files
- Git commit messages for history tracking

## Comments

**When to Comment:**
- Explain the "why" in complex workflow steps
- Comment on regex patterns in `bin/install.js`

## Function Design

**JavaScript:**
- Synchronous utility functions preferred for installer simplicity
- Single-purpose functions (e.g., `copyWithPathReplacement`, `install`)

## Module Design

**Prompts:**
- Encapsulated in semantic tags
- Modular workflows that can be referenced across multiple commands

---

*Convention analysis: 2026-01-14*
*Update when patterns change*
