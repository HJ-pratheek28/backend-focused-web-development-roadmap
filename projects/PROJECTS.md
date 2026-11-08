# Backend Portfolio Projects

Build in order. A project is not complete when the happy path works; it is complete when tested, documented, deployed, observable, and its failure modes are understood.

## 1. Task API
**Skills:** FastAPI, HTTP, Pydantic, pytest, Git.

Build CRUD, filtering, sorting, pagination, validation, consistent errors, and OpenAPI docs.

- [ ] API contract documented
- [ ] Tests cover success and failure paths
- [ ] Predictable validation errors
- [ ] Stable pagination ordering
- [ ] README includes setup, tests, and curl examples

## 2. Multi-user expense API
**Skills:** PostgreSQL, SQL, authentication, transactions, migrations.

Users manage accounts, categories, and transactions. Enforce ownership with application checks and database constraints.

- [ ] Normalized schema and ER diagram
- [ ] Password hashing using a vetted library
- [ ] Authentication and resource-level authorization
- [ ] Transaction-safe balance updates
- [ ] Migrations and seeded test data
- [ ] Tests include cross-user access attempts
- [ ] Backup and restore procedure documented

## 3. URL shortener with analytics
**Skills:** Indexes, Redis, caching, rate limiting, load testing.

Create short links, redirects, expiry, click analytics, and abuse controls.

- [ ] Collision-safe code generation and unique constraints
- [ ] Indexed lookup and cache hit/miss measurements
- [ ] Rate limits and abuse prevention
- [ ] Analytics do not excessively slow redirects
- [ ] Load report includes p50/p95/p99 latency and throughput

## 4. Background job platform
**Skills:** Queues, workers, retries, idempotency, dead-letter handling.

Build an API that accepts work, tracks state, and processes jobs asynchronously.

- [ ] Durable job records and state transitions
- [ ] Worker restart does not lose queued work
- [ ] Duplicate processing protection
- [ ] Retry policy with backoff and dead-letter handling
- [ ] Queue depth, failures, and job latency observable
- [ ] Failure-injection notes

## 5. Real-time collaboration service
**Skills:** WebSockets, pub/sub, authorization, concurrency.

Build a focused collaborative room, chat, or live-status service.

- [ ] Authenticated connections and room authorization
- [ ] Reconnect and heartbeat behavior
- [ ] Message validation and rate limits
- [ ] Persistence strategy explained
- [ ] Multi-instance scaling strategy documented

## 6. Search and ingestion backend
**Skills:** Ingestion pipelines, queues, PostgreSQL, search, object storage.

Ingest documents, extract metadata, process asynchronously, and expose search APIs.

- [ ] Upload validation and size limits
- [ ] Async processing with retry semantics
- [ ] Search relevance and pagination
- [ ] Data lifecycle and deletion behavior
- [ ] Ingestion latency and failures measured

## Capstone — Production-grade backend platform
Choose a real problem and build a multi-user service. Include:
- Problem statement, personas, requirements, and non-goals
- API specification and versioning strategy
- PostgreSQL schema, migrations, indexes, transaction boundaries
- Authentication, authorization, and threat model
- Background processing and caching where justified
- Automated unit, integration, and contract tests
- Dockerized local development and CI/CD
- HTTPS deployment, configuration, and backups
- Structured logs, metrics, traces, health checks, and alerts
- Reproducible load test and performance report
- Architecture diagram, ADRs, runbook, incident report, and cost notes

### Capstone report
1. Problem and requirements
2. Architecture and request/data flow
3. Schema and API contracts
4. Security and threat model
5. Testing strategy
6. Load-test setup and results
7. Failure modes and recovery
8. Trade-offs and future improvements

## Portfolio quality checklist
- [ ] Public repository and meaningful commit history
- [ ] Clear README and architecture diagram
- [ ] Reproducible local setup and env example without secrets
- [ ] Tests run in CI
- [ ] API docs available
- [ ] Live deployment or reproducible deployment instructions
- [ ] Performance measurements, not unsupported claims
- [ ] Security considerations documented
- [ ] Known limitations stated honestly
