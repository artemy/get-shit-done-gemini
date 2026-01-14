# Testing Patterns

**Analysis Date:** 2026-01-14

## Test Framework

**Runner:**
- None for the meta-prompting system itself
- Vitest prescribed for managed projects

**Run Commands:**
```bash
# For managed projects:
npm test
npm run lint
```

## Test File Organization

**Managed Projects:**
- `*.test.ts` alongside source files
- `__tests__/` for integration tests

## Test Structure

**Managed Projects:**
- Arrange/Act/Assert pattern
- Describe/It structure

## Mocking

**Managed Projects:**
- Vitest `vi` for module and function mocking
- Mocking of external boundaries (FS, API) required

## Fixtures and Factories

**System Templates:**
- `get-shit-done/templates/` serve as fixtures for project initialization

## Coverage

**Managed Projects:**
- No strict enforcement, but coverage tracking is recommended for critical services

## Test Types

**Unit Tests:**
- Logic in services and utilities

**Integration Tests:**
- API and database interactions

**UAT (User Acceptance Testing):**
- Managed via `/gsd:verify-work` command
- Issues tracked in `ISSUES.md` within phases

---

*Testing analysis: 2026-01-14*
*Update when test patterns change*
