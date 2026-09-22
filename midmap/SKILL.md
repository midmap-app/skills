---
name: midmap
description: Use Midmap MCP tools to inspect and edit the user's boards when the user asks to work with Midmap boards, nodes, messages, or board context.
---

Use the `midmap_get_current_context` tool first, then use the smallest set of Midmap MCP tools needed to answer or complete the request.

If the Midmap MCP tools are unavailable, report that the Midmap MCP server is not configured or connected. Do not pretend that board state was retrieved.

When new discuss or command messages are found while retrieving information, respond to their contents by default.
