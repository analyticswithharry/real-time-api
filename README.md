# Real-Time API Lab

Build low-latency update pipelines for dashboards, activity feeds, and collaborative UX.

## Why this lab matters

Real-time APIs are not just transport protocols — they are systems design problems involving fanout, consistency, auth, and reconnection behavior.

## Core concepts

- Event fanout architecture
- Channel/topic authorization
- Connection lifecycle management
- Reconnect and state resync
- Latency/throughput instrumentation

## Suggested Stack

- WebSocket or SSE layer
- Redis pub/sub or broker for multi-node fanout

## Practical API plan

- `GET /realtime/channels`
- `POST /realtime/publish`
- `GET /realtime/metrics`
- Starter routes: `GET /api/health`, `GET /api/lesson`, `POST /api/demo`

## Learning Tasks

- Build channel-based live update feed
- Add token-based channel auth
- Implement heartbeat + reconnect strategy
- Add message sequence IDs for state sync
- Measure p95 delivery latency

## Validation checklist

- [ ] Channel auth is enforced
- [ ] Reconnect restores consistent state
- [ ] Delivery latency is measured and reported
- [ ] Multi-client fanout behaves correctly
