# finefab-shared

Shared contracts, schemas, and types used across the **Factory 4 Life
(FineFab)** monorepo — keeps `life-core`, `life-reborn`, `life-web`,
and the various MCP services aligned on a single source of truth for
data shapes.

## Status

Active scaffold. Repository contents were cleared (commit
`b3f1437 chore: clear repository contents`) and the Forgejo docs
workflow was bootstrapped on top — content is being re-introduced
on demand as cross-repo contracts solidify.

## Tech stack

- Language: Python (primary), with room for TypeScript shape
  exports as needed by `life-web` / `life-reborn`.
- Runtime: Python 3.12+, packaged via `uv`.
- CI: Forgejo workflow (`.forgejo/workflows/`) mirrored from
  GitHub Actions.

## Quickstart

```bash
# Sync env (once dependencies land)
uv sync

# Tests
uv run python -m pytest tests/
```

## Place in F4L

Sibling of `life-core`, `life-reborn`, `life-web`,
`agent-factory-cockpit`, `life-spec`, `makelife`, and the
`makelife-*` hardware tree. See
`/Users/electron/Documents/Projets/Factory 4 Life/CLAUDE.md` for
the monorepo overview and inter-repo contracts.
