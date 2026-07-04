# CLAUDE.md

## Overview

**Golden Shiba Dash — SHIBC Utility MVP** — Connect-wallet leaderboard mini-game ('Golden Shiba Dash') — Option A from the #4 scoping, approved by CEO (minor tier, DAO-confirmed no vote needed). Zero on-chain surface: wallet connect is read-only (no tx/gas), used only to attach an address to a submitted score. Ships inside the existing shibaclassic.io Next.js 15 app. Built as two modular pieces per CEO's hedge, so the scoring layer survives if the utility goal is later redefined toward integrating into an external partner's existing game instead of building our own.

> Scaffolded from `project-template` by AITO (#1268). This repo is **dormant**
> until its per-project Vault path + AppRole are provisioned out-of-band; until
> then `secrets:pull` has nothing to pull and the MCP servers stay unconnected.

## MCP servers

This repo ships a **least-privilege** `.mcp.json` (github + woodpecker + playwright for web). Additional MCP servers (directus, imagen, …) are added
deliberately and human-gated — never auto-expanded by an agent.

## Quality gates

Woodpecker CI (`.woodpecker/ci.yml`) runs typecheck + lint + tests.
