# Backend Engineering Roadmap

Follow the stages in order. Revisit earlier layers when projects expose gaps.

## 0. Developer foundations
- [ ] Git: commits, branches, merges, pull requests, conflict resolution
- [ ] Terminal and shell: pipes, grep, find, permissions, processes
- [ ] Python: modules, exceptions, iterators, generators, decorators, typing, packaging
- [ ] Data structures: arrays, hash maps, stacks, queues, trees, heaps, graphs
- [ ] Complexity analysis and common algorithmic patterns
- [ ] Debugging, stack traces, logging, minimal reproductions
- [ ] Unit testing and test organization

**Exit test:** Build a Python CLI package with tests, type hints, logging, configuration, and clean Git history.

## 1. Web and networking fundamentals
- [ ] IP, TCP, UDP, DNS, ports, routing, TLS
- [ ] HTTP request/response lifecycle; HTTP/1.1, HTTP/2, HTTP/3 concepts
- [ ] Methods, status codes, headers, cookies, caching headers
- [ ] URLs, query parameters, encoding, MIME types, JSON
- [ ] Browser basics: DOM, forms, fetch, CORS, same-origin policy
- [ ] HTML, CSS, and JavaScript essentials
- [ ] REST constraints and resource-oriented API design

**Exit test:** Explain a browser request from DNS lookup to response; inspect traffic with browser devtools and curl.

## 2. Backend fundamentals with Python
- [ ] Virtual environments, dependency pinning, project structure
- [ ] FastAPI routing, parameters, request bodies, response models
- [ ] Pydantic validation and settings
- [ ] Dependency injection and application lifecycle
- [ ] Error handling and consistent error contracts
- [ ] OpenAPI documentation
- [ ] Middleware, request IDs, structured logging
- [ ] Environment-based configuration
- [ ] File uploads, downloads, and streaming basics
- [ ] Background task limitations

**Exit test:** Build a versioned REST API with validation, pagination, filtering, errors, OpenAPI docs, and tests.

## 3. Databases and data modeling
- [ ] Entities, relationships, constraints, normalization
- [ ] SQL: joins, grouping, subqueries, CTEs, window functions
- [ ] PostgreSQL schemas, data types, constraints, indexes
- [ ] ACID, transactions, isolation levels, concurrency anomalies
- [ ] Query plans with EXPLAIN and EXPLAIN ANALYZE
- [ ] B-tree, composite, partial, and covering indexes
- [ ] Migrations and schema evolution
- [ ] Connection pooling
- [ ] SQLAlchemy plus raw SQL
- [ ] Backups, restore drills, data integrity
- [ ] NoSQL concepts and appropriate use cases

**Exit test:** Design a normalized schema, write non-trivial SQL, explain query plans, and demonstrate safe transactions.

## 4. Production API engineering
- [ ] Authentication vs authorization
- [ ] Password hashing, sessions, access and refresh tokens
- [ ] OAuth 2.0 and OpenID Connect concepts
- [ ] Role-based and resource-based access control
- [ ] Rate limiting, quotas, abuse prevention
- [ ] Idempotency keys and safe retries
- [ ] Offset vs cursor pagination
- [ ] API versioning and backwards compatibility
- [ ] Webhooks: signatures, retries, replay protection
- [ ] CORS, CSRF, secure cookies
- [ ] API contracts and schema evolution

**Exit test:** Secure a multi-user API with ownership checks, token/session lifecycle, rate limits, idempotent writes, and integration tests.

## 5. Testing and software quality
- [ ] Unit, integration, contract, and end-to-end tests
- [ ] pytest fixtures, parametrization, mocking boundaries
- [ ] Test database isolation and migration tests in CI
- [ ] Property-based testing concepts
- [ ] Load and stress testing; latency percentiles
- [ ] Disposable service dependencies / Testcontainers
- [ ] Static analysis, formatting, linting, type checking
- [ ] Code review and design documentation

**Exit test:** CI runs lint, type checks, unit/integration tests, migration checks, and a small load test.

## 6. Linux, containers, and deployment
- [ ] Linux processes, signals, file descriptors, permissions
- [ ] Environment variables, secrets, filesystem layout
- [ ] TCP sockets and tools such as ss, lsof, curl
- [ ] Docker images, layers, volumes, networks, multi-stage builds
- [ ] Docker Compose for local multi-service environments
- [ ] Reverse proxies and TLS termination
- [ ] Nginx basics; Uvicorn/Gunicorn workers
- [ ] CI/CD with GitHub Actions
- [ ] Deploy to a Linux VM or free-tier platform; understand costs
- [ ] DNS, HTTPS certificates, health checks
- [ ] Release strategies, rollback, migration safety

**Exit test:** Deploy a containerized API and PostgreSQL, automate tests and deployment, configure HTTPS, and document rollback.

## 7. Performance and asynchronous systems
- [ ] Python concurrency: threads, processes, asyncio
- [ ] Async I/O vs CPU-bound work; event loop behavior
- [ ] Worker pools and bounded concurrency
- [ ] Redis data structures, TTL, eviction, persistence
- [ ] Cache-aside, write-through, invalidation, stampede protection
- [ ] Queues and brokers: delivery semantics, acknowledgements
- [ ] Background workers such as Celery or RQ
- [ ] Retries, exponential backoff, dead-letter queues
- [ ] WebSockets and server-sent events
- [ ] Streaming and large-file handling
- [ ] Profiling, flame graphs, database bottlenecks
- [ ] Timeouts, load shedding, bulkheads, circuit breakers

**Exit test:** Add caching and durable background jobs; demonstrate behavior during worker, broker, and cache failures.

## 8. Security engineering
- [ ] OWASP Top 10 and API Security Top 10
- [ ] Injection, XSS, CSRF, SSRF, path traversal, insecure deserialization
- [ ] Broken access control and IDOR
- [ ] Secure password storage and account recovery
- [ ] Secrets management and key rotation
- [ ] TLS, encryption at rest, data minimization
- [ ] Dependency and container vulnerability scanning
- [ ] Audit logs, privacy, retention, threat modeling
- [ ] Security headers and secure deployment configuration

**Exit test:** Threat-model a project, run security checks, fix issues, and write a security review.

## 9. Distributed systems and system design
- [ ] Latency, throughput, availability, reliability, durability
- [ ] Replication, partitioning, sharding, consistency
- [ ] CAP theorem and practical consistency models
- [ ] Leader election and coordination concepts
- [ ] Distributed transactions, sagas, transactional outbox
- [ ] Event-driven architecture and event sourcing trade-offs
- [ ] Service discovery and load balancing
- [ ] Horizontal scaling and stateless services
- [ ] Monolith, modular monolith, microservices trade-offs
- [ ] Object storage, CDN, search indexing
- [ ] Multi-region concepts, disaster recovery, RPO/RTO
- [ ] Capacity estimation and bottleneck analysis

**Exit test:** Design a system from requirements, estimate scale, identify bottlenecks, explain trade-offs, and plan failure recovery.

## 10. Secondary ecosystem: TypeScript and Node.js
Only after building and deploying a substantial Python service.
- [ ] TypeScript types, generics, narrowing, modules
- [ ] Node runtime, event loop, streams, buffers
- [ ] Express or Fastify; middleware and error handling
- [ ] PostgreSQL integration and validation
- [ ] Auth, testing, observability, Docker
- [ ] Compare Python async and Node event-loop approaches

**Exit test:** Rebuild a smaller service in TypeScript and compare maintainability, performance, and trade-offs.

## 11. Professional engineering
- [ ] Read unfamiliar codebases and trace requests end-to-end
- [ ] Write RFCs, ADRs, incident reports, and runbooks
- [ ] On-call fundamentals and incident response
- [ ] SLOs, SLIs, error budgets
- [ ] Metrics, logs, traces, dashboards, alert design
- [ ] Profiling and optimization based on measurements
- [ ] Open-source contribution: reproduce, test, fix, document
- [ ] Interview preparation: coding, SQL, networking, OS, databases, system design

**Final standard:** Three deployed, documented projects; one substantial backend capstone; meaningful tests; measured performance; security review; operational runbooks; and the ability to defend architectural decisions.
