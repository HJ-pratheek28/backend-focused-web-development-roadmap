# System Design Case Studies

Write assumptions and requirements before drawing an architecture.

## Beginner

### URL shortener
Create and resolve short codes. Handle collisions, custom aliases, expiry, analytics. Discuss redirect latency, cache behavior, abuse prevention, and global reads.

### Pastebin
Store text snippets with expiry and optional access control. Discuss storage choice, IDs, retention, large payloads, and deletion.

### Rate limiter
Support per-user and per-IP limits. Compare fixed window, sliding window, token bucket, and leaky bucket. Discuss distributed counters.

## Intermediate

### Notification service
Accept requests and deliver email, push, or webhook jobs. Design queues, retries, deduplication, preferences, delivery status, and provider failure handling.

### File upload service
Support large uploads, metadata, permissions, and download links. Discuss multipart/resumable uploads, object storage, scanning, lifecycle, and CDN.

### Chat service
Support direct and group messaging, online status, and history. Discuss WebSockets, ordering, persistence, fan-out, reconnect, and multi-instance deployment.

### Ticket booking
Prevent double booking under concurrency. Discuss transactions, locks, inventory reservation, expiry, idempotency, and payment/confirmation failure.

## Advanced

### News feed
Compare fan-out-on-write and fan-out-on-read. Discuss hot users, ranking, caching, and eventual consistency.

### Metrics ingestion platform
Accept high-volume time-series events. Discuss batching, buffering, partitioning, retention, aggregation, and query patterns.

### E-commerce checkout
Design cart, inventory, payment, order state, and refunds. Discuss sagas, outbox, idempotency, reconciliation, and auditability.

## Review checklist
- [ ] Requirements and explicit assumptions
- [ ] API endpoints and example payloads
- [ ] Data model and key indexes
- [ ] High-level architecture and capacity estimate
- [ ] Read/write flow
- [ ] Consistency and concurrency strategy
- [ ] Failure modes and recovery
- [ ] Security and abuse cases
- [ ] Observability and SLO
- [ ] Cost and complexity trade-offs
