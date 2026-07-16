# Realtime Architecture

Realtime use cases include messaging presence, notifications, live-stream chat, event updates, wallet status, and operator queues. Transport is an authenticated gateway with channel-level authorization, back-pressure, rate limiting, replay/ordering semantics, and observability.

WebRTC/media sessions are isolated from control-plane data. LiveKit/SFU, OBS/RTMP ingestion, recording, captions, and moderation are provider/service boundaries with explicit failure modes. A realtime event never substitutes for a durable command result.
