# FAF — Persistent Project Context for Claude Code

> **Retired (2026-10-03).** FAF is one plugin now: **[FAF Skills](https://github.com/Wolfe-Jam/faf-skills)**. This plugin's MCP toolbox (`claude-faf-mcp`) joins it in FAF Skills v2.
>
> ```
> /plugin marketplace add Wolfe-Jam/faf-skills
> /plugin install faf@faf-skills
> ```
>
> Until v2 ships, add the MCP server on its own: `claude mcp add faf -- npx -y claude-faf-mcp@7.0.1`. This repo is archived (read-only).

`.faf` is an IANA-registered structured file (`application/vnd.faf+yaml`) that captures your project's DNA and generates/syncs your `CLAUDE.md` — so Claude starts every session already knowing the project.

This plugin bundles the [`claude-faf-mcp`](https://www.npmjs.com/package/claude-faf-mcp) server (also listed in the MCP Registry).

## Install

Not in Anthropic's directory yet (review pending). Until then, install from the FAF marketplace:

```
/plugin marketplace add Wolfe-Jam/faf-plugins
/plugin install faf@faf-plugins
```

## What it runs

The plugin starts one local MCP server, `claude-faf-mcp@7.0.1`, through `npx` (downloaded from npm on first run). It reads and writes `.faf`, `CLAUDE.md` and related files in your project. It contacts GitHub only when you ask it to read a GitHub repo, and collects no data. Support: team@faf.one.

## What you get

- Generate + score a `.faf` for any repo
- Bi-sync `.faf` ↔ `CLAUDE.md` — deterministic, no drift
- Portable context: one source feeds `CLAUDE.md` / `AGENTS.md` / `.cursorrules`

Complementary to Claude Code's context system — `.faf` is the structured source that *generates* `CLAUDE.md`.

## Links

- Home: https://faf.one
- MCP server: https://www.npmjs.com/package/claude-faf-mcp
- Format: IANA `application/vnd.faf+yaml`

## Citation

> Wolfe, J. (2025). *Format-Driven AI Context Architecture: The .faf Standard for Persistent Project Understanding*. Zenodo. https://doi.org/10.5281/zenodo.18251362

> Wolfe, J. (2026). *Why Agents Need a Passport: .fafa — Portable Identity for the Agentic Era*. Zenodo. https://doi.org/10.5281/zenodo.21951641
