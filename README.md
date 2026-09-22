# Midmap Skills

Supporting agent skills for the [Midmap](https://midmap.app) application.
Midmap provides MCP capabilities that these skills use to work with Midmap boards.

## Install

Install the skills for your coding agent with:

```bash
npx skills add midmap-app/skills
```

The `skills` CLI supports multiple coding agents and installs the skills to the current project by default. Add `--agent <agent>` when you want to target a specific agent.

## Prerequisites

Install and configure the Midmap application, then make sure its MCP capabilities are connected to the selected agent before using these skills.

Installing this repository installs the agent instructions only; it does not install Midmap or configure its MCP capabilities.

## Repository layout

Each directory under `skills/` is an independently installable skill.
