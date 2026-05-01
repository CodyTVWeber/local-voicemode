---
description: Check the status of Yakk services
---

# /yakk:status

Check the status of Yakk services.

## Usage

```
/yakk:status
```

## Description

Shows the current status of Yakk services including Whisper (STT), Kokoro (TTS), and LiveKit (if used).

## Implementation

Use the `mcp__yakk__service` tool:

```json
{
  "service_name": "whisper",
  "action": "status"
}
```

Check all services:

```bash
# Check Whisper (STT)
mcp__yakk__service service_name=whisper action=status

# Check Kokoro (TTS)
mcp__yakk__service service_name=kokoro action=status

# Check LiveKit (optional)
mcp__yakk__service service_name=livekit action=status
```

## Output

Shows for each service:
- Running status
- Resource usage
- Endpoint availability
