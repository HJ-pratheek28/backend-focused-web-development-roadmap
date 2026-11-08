# Backend System Design Syllabus

System design is applied engineering, not memorizing diagrams. Clarify requirements, estimate scale, define interfaces and data, identify bottlenecks, then discuss failure and trade-offs.

## 1. Requirements and estimation
- Functional and non-functional requirements
- Traffic patterns, read/write ratio, requests per second
- Storage growth, bandwidth, latency targets, tail latency
- Availability, durability, consistency, SLOs and error budgets

Practice estimates for a URL shortener, chat service, and file upload platform.

## 2. API and data design
- Resource modeling, API boundaries, pagination, idempotency, versioning
- Relational schema, indexes, constraints, transactions, isolation
- Read/write paths, query patterns, retention, archival, deletion

## 3. Scaling a service
- Vertical vs horizontal scaling; stateless application instances
- Load balancing, health checks, connection pooling, backpressure
- Caching and invalidation; CDN and object storage
- Database replicas, partitioning, and sharding

## 4. Distributed systems
- Partial failure and network partitions
- Timeouts, retries, jitter, idempotency
- At-most-once, at-least-once, and effectively-once processing
- Replication lag, consistency, leader/follower models
- Partitioning, rebalancing, coordination, distributed locks
- Sagas and transactional outbox

## 5. Messaging and event-driven architecture
- Queue vs pub/sub vs event log
- Ordering, delivery, acknowledgements, consumer groups, replay
- Poison messages and dead-letter queues
- Schema evolution and compatibility
- Event sourcing: use cases and costs

## 6. Reliability and operations
- Health/readiness/liveness checks
- Metrics, logs, distributed traces
- SLI/SLO, alert fatigue, graceful degradation, load shedding
- Backups, restore drills, disaster recovery, RPO/RTO
- Incident response, capacity planning, cost optimization

## 7. Architecture choices
- Modular monolith vs microservices
- Service boundaries and ownership
- Synchronous vs asynchronous communication
- Database-per-service trade-offs
- API gateway and service discovery
- Avoiding premature complexity

## Design interview framework
1. Restate the problem and clarify scope.
2. List functional and non-functional requirements.
3. Estimate users, traffic, storage, and bandwidth.
4. Define APIs and the core data model.
5. Draw the simplest architecture that meets requirements.
6. Walk through read and write flows.
7. Identify bottlenecks and scale incrementally.
8. Discuss consistency, failure modes, and recovery.
9. Cover security, observability, and deployment.
10. Summarize trade-offs and open questions.

For every design, produce a requirements brief, API sketch, schema, architecture diagram, capacity estimate, failure table, and decision log. Revisit the design after implementing a slice.
