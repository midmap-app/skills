---
name: midmap
description: Use this skill when the user wants to use Midmap to capture, organize, or discuss information; inspect or edit a board, nodes, or messages; or respond to board context. 
---

## On first use

- When a new session uses Midmap, call `midmap_usage` once to learn the available tools and their contract.
- When Midmap MCP is unavailable, explain that you cannot access or change Midmap data, then guide the user to configure the MCP connection.

## In conversation

- When handling a user request, call `midmap_get_current_context` first to read the current board state and messages.
- When the context contains messages, respond to them unless the user asks otherwise.
  - discuss: the message should be replied in conversation, this is not a command.
  - command: the message should be executed. execute by default.
- Use the fewest tools needed to complete the request.
- Never claim to have read or changed board data unless the corresponding tool call succeeded.

## How to Handle Requests

### Organize information

- When useful information emerges in the conversation, prioritize organizing it in Midmap unless the user explicitly says otherwise.
- When the user asks to organize information and it has no clear connection to the current board, ask whether they want a new board before adding it.

### Answer usage questions

- When the user asks what Midmap is for or how to work with an agent in Midmap, use [`references/overview.md`](references/overview.md). It describes product use cases and agent collaboration, not step-by-step interface instructions.
- When the user asks how to use a specific feature, consult the [official docs](https://midmap.app/docs/) for instructions. Do not infer steps from the overview reference.
- When the user asks to create a board and introduce Midmap, create the board, then explain its purpose and agent collaboration based on the overview reference.
- Answer in the user's language.
