---
name: start
description: Start a two-way yakk voice conversation using local Yakk
argument-hint: [opening message]
---

# /yakk:start

Kick off an ongoing two-way voice conversation using the local Yakk MCP server.

## Implementation

1. Greet the user with the provided message (or "Hey! What's up?" if none given)
2. Use `mcp__yakk__converse` with `wait_for_response: true`
3. Listen, respond naturally, and keep the loop going
4. Continue until the user says bye / stop / ends the session

The goal is a relaxed back-and-forth — not a task runner. Just yak.
