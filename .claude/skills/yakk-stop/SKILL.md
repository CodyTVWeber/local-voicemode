---
name: stop
description: End the current yakk voice conversation
---

# /yakk:stop

Gracefully end the current yakk voice conversation.

## Implementation

Say a brief goodbye using `mcp__yakk__converse` with `wait_for_response: false`, then stop the conversation loop.
