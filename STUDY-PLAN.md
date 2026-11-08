# 24-Month Backend Engineering Study Plan

Designed for a learner with basic Python/C++ familiarity, a basic math foundation, a free-first budget, and roughly 4–6 focused hours/day. Treat this as a sequence of outcomes, not a race.

## Weekly rhythm
- 3 days: concepts and small implementation exercises
- 2 days: current project and tests
- 1 day: debugging, documentation, review, and interview practice
- 1 day: rest or light catch-up

For a 6-hour day: about 90 minutes concepts, 2 hours implementation, 90 minutes project work, 30 minutes testing/debugging, and 30 minutes review. Adjust to protect consistency.

## Months 1–3: foundations and web
| Month | Focus | Deliverable |
|---|---|---|
| 1 | Python depth, Git, terminal, debugging, testing, data structures | Tested Python CLI package |
| 2 | HTML/CSS/JS essentials, browser lifecycle, HTTP, DNS, TCP/IP, TLS | HTTP experiments and tiny client |
| 3 | REST, JSON, curl, API contracts, FastAPI | Versioned CRUD API with validation and OpenAPI |

**Gate:** Explain a request end-to-end and build/test a small API without following a tutorial line-by-line.

## Months 4–6: databases and production APIs
| Month | Focus | Deliverable |
|---|---|---|
| 4 | SQL, relational modeling, PostgreSQL, constraints, joins | Schema and SQL query collection |
| 5 | Transactions, indexes, EXPLAIN, migrations, SQLAlchemy + raw SQL | PostgreSQL-backed API |
| 6 | Auth, authorization, pagination, rate limits, idempotency | Multi-user API with ownership checks |

**Gate:** Demonstrate safe transactions, explain index choices, prevent unauthorized access, and document the API.

## Months 7–9: quality and deployment
| Month | Focus | Deliverable |
|---|---|---|
| 7 | pytest, fixtures, integration/contract tests, typing, linting | CI quality gates |
| 8 | Linux, sockets, Docker, Compose, reverse proxy, HTTPS | Containerized deployed application |
| 9 | CI/CD, configuration, secrets, migrations, rollback, backups | Automated deployment and runbook |

**Gate:** A new contributor can run the stack from the README; deployment and rollback are repeatable.

## Months 10–12: async, caching, background work
| Month | Focus | Deliverable |
|---|---|---|
| 10 | asyncio, threads/processes, event loop, worker pools | Async service with concurrency measurements |
| 11 | Redis, caching, TTL, invalidation, rate limits | Cache improvement with correctness tests |
| 12 | Queues, workers, retries, dead letters, WebSockets/SSE | Durable job pipeline and real-time feature |

**Gate:** Explain behavior when a worker crashes, a message is delivered twice, or Redis is unavailable.

## Months 13–15: security and performance
| Month | Focus | Deliverable |
|---|---|---|
| 13 | OWASP, threat modeling, secure auth, SSRF/IDOR/CSRF | Security assessment and fixes |
| 14 | Profiling, SQL tuning, load testing, latency percentiles | Benchmark report with before/after results |
| 15 | Timeouts, retries, circuit breakers, bulkheads, graceful degradation | Failure-injection exercise and incident report |

**Gate:** Identify and fix a measured bottleneck; demonstrate behavior during dependency failure.

## Months 16–18: distributed systems
| Month | Focus | Deliverable |
|---|---|---|
| 16 | Availability, consistency, replication, partitioning, CAP | Design notes for replicated data service |
| 17 | Event-driven systems, outbox, sagas, broker semantics | Reliable event pipeline with idempotent consumers |
| 18 | Load balancing, object storage, CDN, search, scaling | Architecture design and implemented subsystem |

**Gate:** Produce a system design with requirements, estimates, APIs, schema, failure modes, and trade-offs.

## Months 19–21: observability and professional practice
| Month | Focus | Deliverable |
|---|---|---|
| 19 | Logs, metrics, traces, SLOs, alerts | Dashboard, tracing, SLO proposal |
| 20 | TypeScript, Node runtime, Express/Fastify | Small tested TypeScript service |
| 21 | Read open-source backend code; fix an issue or add tested feature | Merged contribution or documented PR |

**Gate:** Navigate an unfamiliar codebase and explain request flow, tests, and design choices.

## Months 22–24: capstone and hiring readiness
| Month | Focus | Deliverable |
|---|---|---|
| 22 | Design and implement capstone core, auth, schema, APIs, tests | Working deployed capstone |
| 23 | Scale, secure, instrument, load-test, document, failure drills | Production-readiness report |
| 24 | Portfolio polish, open source, CS fundamentals, interviews | Portfolio release and project walkthrough |

**Final gate:** Independently design, build, deploy, secure, measure, and operate a backend application. Explain what failed, what you measured, what changed, and why.

## Monthly review rubric
Score each category from 0–3:
- 0: cannot explain it
- 1: can explain after reading notes
- 2: can implement with documentation
- 3: can implement, debug, test, and explain trade-offs independently

Score concepts, implementation, debugging, testing, documentation, and project integration. Do not advance a critical topic below 2.

## Weekly evidence to commit
- Notes explaining key concepts
- Small exercises and experiments
- Tests and project code
- Decision log for meaningful trade-offs
- Retrospective: what worked, what broke, next week's target
