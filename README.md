# Backend-Focused Web Development Roadmap

A backend-first, 24-month path from programming foundations to production services, distributed systems, and system design.

**Primary stack:** Python, FastAPI, PostgreSQL, Redis, Docker, Linux, GitHub Actions.  
**Supporting skills:** HTML/CSS/JavaScript/TypeScript, HTTP, networking, cloud, testing, security, observability.  
**Budget:** Free-first. **Pace:** Adapt the plan to 4–6 focused hours/day.

## Purpose

This is not a frontend roadmap with a backend chapter. Its center is API engineering, data modeling, transactions, reliability, security, performance, distributed systems, and operating software in production.

Learn one primary stack deeply first. Start with Python and FastAPI; add TypeScript and Node.js later as a complementary ecosystem, not as a second simultaneous beginner track.

## Start here

1. Read [ROADMAP.md](ROADMAP.md) for the skill sequence and exit tests.
2. Follow [STUDY-PLAN.md](STUDY-PLAN.md) for the 24-month execution schedule.
3. Use [RESOURCES.md](RESOURCES.md) for topic-by-topic free resources.
4. Build the projects in [projects/PROJECTS.md](projects/PROJECTS.md).
5. Study [system design](system-design/SYSTEM-DESIGN.md) and [case studies](system-design/CASE-STUDIES.md).

## Engineering rules

- Build every week and ship a working milestone every month.
- Learn SQL directly; an ORM does not replace database knowledge.
- Test failure paths, authorization boundaries, and concurrency—not only happy paths.
- Deploy projects. A localhost demo is not a production project.
- Measure performance before optimizing.
- Document architecture decisions, trade-offs, known limitations, and recovery procedures.
- Never commit secrets. Use environment variables and appropriate secret management.

## Definition of job-ready

You can independently design, implement, test, document, deploy, secure, debug, and improve a backend service. You can explain API contracts, schema design, indexes, transactions, caching, concurrency, queues, failure handling, observability, and scaling trade-offs.

## Repository map

| File | Purpose |
|---|---|
| [ROADMAP.md](ROADMAP.md) | Prerequisite-ordered skill tree |
| [STUDY-PLAN.md](STUDY-PLAN.md) | 24-month plan and checkpoints |
| [RESOURCES.md](RESOURCES.md) | Curated resources for every topic |
| [projects/PROJECTS.md](projects/PROJECTS.md) | Portfolio projects and acceptance criteria |
| [system-design/SYSTEM-DESIGN.md](system-design/SYSTEM-DESIGN.md) | Architecture and design syllabus |
| [system-design/CASE-STUDIES.md](system-design/CASE-STUDIES.md) | System design practice prompts |
| [references/REFERENCE-INDEX.md](references/REFERENCE-INDEX.md) | Official docs and quick links |

Mark a topic complete only when you can explain it, implement it without a tutorial, and debug a realistic failure.
