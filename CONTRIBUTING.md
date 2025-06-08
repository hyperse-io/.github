# Contributing to Hyperse

Thank you for your interest in contributing to Hyperse! This document provides guidelines and instructions to help you contribute effectively.

## Table of Contents
- [Getting Started](#getting-started)
- [Branch Strategy](#branch-strategy)
- [Making Contributions](#making-contributions)
- [Commit Guidelines](#commit-guidelines)
- [Development Setup](#development-setup)
- [Legal Requirements](#legal-requirements)

## Getting Started

Before you begin:
1. Create an issue to discuss your proposed changes
2. Ensure your contribution aligns with Hyperse's goals
3. Review these guidelines thoroughly

## Branch Strategy

We maintain three main branches:

| Branch | Purpose | When to Use |
|--------|---------|-------------|
| `master` | Production-ready code | Bug fixes and minor improvements |
| `minor` | New features | Non-breaking feature additions |
| `major` | Breaking changes | Backwards-incompatible changes |

### Branch Selection Guide
- **Bug fixes**: Submit to `master`
- **New features**: Submit to `minor`
- **Breaking changes**: Submit to `major`

## Making Contributions

### Bug Fixes
1. Create an issue describing the bug
2. Indicate your intention to fix it
3. Submit your fix to the `master` branch
4. Follow the commit message format below

### New Features
1. Create a feature request issue
2. State your intention to implement
3. Submit to the `minor` branch
4. Document new APIs with `@since` tags

Example of API documentation:
```typescript
/**
 * @description
 * Sets the value of the new API thing.
 *
 * @since 1.2.0
 */
myNewApi: number;
```

## Commit Guidelines

We follow the [Conventional Commits](https://www.conventionalcommits.org) specification.


### Commit Types
- `feat`: New feature
- `fix`: Bug fix
- `docs`: Documentation changes
- `style`: Code style changes
- `refactor`: Code refactoring
- `perf`: Performance improvements
- `test`: Test-related changes
- `chore`: Maintenance tasks

### Scope
- Use package names (e.g., `core`, `common`, `website`)
- For multiple packages: `fix(core,common): Fix the thing`
- Omit scope for root-level changes

### Breaking Changes
Include a `BREAKING CHANGE` section in your commit message:

```text
feat(core): Add new field to Customer
Relates to #123. This commit adds the "foo" field to the Custom entity.
BREAKING CHANGE: A DB migration will be required to add the new "foo" field to the customer table.
```

> 💡 **Tip**: Use `yarn g:cz` for interactive commit message creation

## Development Setup

Follow the [Development guide](./README.md#development) in the README for local setup instructions.

## Legal Requirements

All contributors must agree to the [Contributor License Agreement](./license/CLA.md) before their contributions can be merged. This is handled automatically via a bot when you open a pull request.

---

Thank you for contributing to Hyperse! Your efforts help make this project better for everyone. 🌿💚