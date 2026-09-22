# Midmap Skills

Agent skills for Midmap.

## Install

Install the Midmap skill for your coding agent with:

```bash
npx skills add midmap-app/skills --skill midmap --global
```

The `skills` CLI supports multiple coding agents. Add `--agent <agent>` when you want to target a specific agent, or let the CLI detect available agents.

## Prerequisites

This skill uses the Midmap MCP server. Install and configure Midmap and make sure its MCP server is connected to the selected agent before using the skill.

Installing this repository installs the agent instructions only; it does not install Midmap or configure an MCP server.

## Repository layout

Each directory under `skills/` is an independently installable skill.
