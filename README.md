# Midmap Skills

Agent skills for Midmap.

## Install

Install the Midmap skill for Codex with:

```bash
npx skills add midmap-app/skills --skill midmap --global --agent codex
```

The repository is compatible with other agents supported by the `skills` CLI. Replace `--agent codex` with the target agent when needed.

## Prerequisites

This skill uses the Midmap MCP server. Install and configure Midmap and make sure its MCP server is connected to the selected agent before using the skill.

Installing this repository installs the agent instructions only; it does not install Midmap or configure an MCP server.

## Repository layout

Each directory under `skills/` is an independently installable skill.
