# FAF — Persistent Project Context for Claude Code

`.faf` is an IANA-registered structured file (`application/vnd.faf+yaml`) that captures your project's DNA and generates/syncs your `CLAUDE.md` — so Claude starts every session already knowing the project.

This plugin bundles the [`claude-faf-mcp`](https://www.npmjs.com/package/claude-faf-mcp) server (also in the official MCP Registry).

## Install

```
/plugin install faf@claude-community
```

## What you get

- Generate + score a `.faf` for any repo
- Bi-sync `.faf` ↔ `CLAUDE.md` — deterministic, no drift
- Portable context: one source feeds `CLAUDE.md` / `AGENTS.md` / `.cursorrules`

Complementary to Claude Code's context system — `.faf` is the structured source that *generates* `CLAUDE.md`.

## Links

- Home: https://faf.one
- MCP server: https://www.npmjs.com/package/claude-faf-mcp
- Format: IANA `application/vnd.faf+yaml`
