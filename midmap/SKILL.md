---
name: midmap
description: Use this skill when the user wants to use Midmap to capture, organize, or discuss information; inspect or edit a board, nodes, or messages; or respond to board context. Trigger from the requested activity even if the user does not name Midmap, when the context indicates they want the information handled in their mind map. Do not trigger for unrelated information work with no Midmap context.
---

In each new session, call `midmap_usage` at least once to learn the MCP contract. If the MCP instructions are not already loaded in context, call it before other Midmap tools.

Before each Midmap tool call, call `midmap_get_current_context` to retrieve the current board state and messages. Respond to messages by default unless the user explicitly asks otherwise. Then use the smallest set of tools needed to complete the request.

If the user asks to organize information in Midmap and it has no clear connection to the current board, ask whether they want to create a new board before adding it.

If Midmap MCP is not installed or unavailable, explain that accurately and guide the user to add the MCP configuration. Do not claim to have retrieved or changed board data.

When users ask how to use Midmap or ask related questions, consult the official website before answering: [English](https://midmap.app/) and [Chinese](https://midmap.app/cn/).
