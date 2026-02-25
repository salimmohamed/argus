# Contributing to Argus

Thanks for your interest in contributing to Argus. This guide covers how to get set up and the conventions we follow.

## Development Setup

### Prerequisites

- [Bun](https://bun.sh/) (package manager and runtime)
- [Convex](https://convex.dev/) account
- AWS account with [Bedrock](https://aws.amazon.com/bedrock/) access (Claude model enabled)

### Getting Started

```bash
git clone https://github.com/salimmohamed/argus.git
cd argus
bun install
cp .env.example .env.local
```

Fill in your credentials in `.env.local`, then start the development servers:

```bash
npx convex dev   # Convex backend (terminal 1)
bun dev          # Next.js frontend (terminal 2)
```

## Code Style

This project uses [Biome](https://biomejs.dev/) for linting and formatting.

```bash
bun run lint        # Check for issues
bun run lint:fix    # Auto-fix issues
```

## Commit Conventions

We use [Conventional Commits](https://www.conventionalcommits.org/):

```
<type>(<scope>): <short description>
```

**Types:** `feat`, `fix`, `docs`, `style`, `refactor`, `test`, `chore`

**Examples:**
```
feat(agent): add network analysis tool
fix(detection): handle null API responses
docs: update setup instructions
```

Keep commit messages short with no body text.

## Pull Requests

1. Fork the repo and create a branch from `main`
2. Make your changes
3. Run `bun run lint` to check code style
4. Open a PR with a clear title and description
5. Link any related issues

## Reporting Bugs

Use the [bug report template](https://github.com/salimmohamed/argus/issues/new?template=bug_report.md) and include:

- Steps to reproduce
- Expected vs actual behavior
- Environment details (OS, Bun version, browser)

## Feature Requests

Use the [feature request template](https://github.com/salimmohamed/argus/issues/new?template=feature_request.md) and describe:

- The problem you're trying to solve
- Your proposed solution
- Any alternatives you've considered
