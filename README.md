# Hasibul Islam

**Senior Backend Architect · 7+ years · Node.js · NestJS · TypeScript · AWS**
Building multi-tenant SaaS platforms and real-time systems that hold up under production traffic.

Currently Sr. Backend Architect at [ZMC Technologies](https://zmc-technologies.com/), shipping backend infrastructure for AI-augmented omnichannel messaging, real-estate SaaS, and business-automation platforms.

Recent production win: cut a hot-path API from **~200ms → ~20ms** through query flattening, targeted indexing, cache-aside, and serialization changes. Reproducible reference: **[api-latency-case-study](https://github.com/devhasibulislam/api-latency-case-study)** — clone, `docker compose up`, `npm run bench`, see the delta on your machine.

[![LinkedIn](https://custom-icon-badges.demolab.com/badge/LinkedIn-in%2Fdevhasibulislam-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devhasibulislam/)
[![Portfolio](https://img.shields.io/badge/Portfolio-devhasibulislam.vercel.app-2ea44f?style=flat&logo=vercel&logoColor=white)](https://devhasibulislam.vercel.app/)
[![Email](https://img.shields.io/badge/Email-devhasibulislam%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:devhasibulislam@gmail.com)
[![Telegram](https://img.shields.io/badge/Telegram-%40devhasibulislam-26A5E4?style=flat&logo=telegram&logoColor=white)](https://t.me/devhasibulislam)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=flat&logo=whatsapp&logoColor=white)](https://wa.me/8801906315901)
[![YouTube](https://img.shields.io/badge/YouTube-%40devhasibulislam-FF0000?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/@devhasibulislam)

---

## What I do

- **Design multi-tenant NestJS backends** with clean domain boundaries, per-tenant isolation, and background workers that survive real load.
- **Diagnose latency end-to-end** — query plans, connection pools, cache layers, serialization — with benchmarks, not guesses.
- **Ship AI-augmented ingestion pipelines** (WhatsApp, Messenger, Instagram, web chat) with idempotency, retry, and dead-letter handling.
- **Own systems from schema to deploy** — Postgres/Mongo schema design, Docker, Nginx, PM2, GitHub Actions, AWS/DigitalOcean.

## Production systems

Live products I've designed, built, or scaled. Source under NDA; happy to walk through architecture and my specific contributions in an interview.

| Product | What it does | My focus |
|---|---|---|
| **[Ayrshare](https://www.ayrshare.com/)** | Developer-first unified social-media API — publish, schedule, analytics, comments and DMs across 13+ networks (X, Facebook, Instagram, LinkedIn, TikTok, YouTube, Telegram, Threads, Bluesky, Reddit, Pinterest, Snapchat, Google Business). Native MCP server for AI agents. Powers 10,000+ teams incl. Ubisoft, Oracle, Red Hat, RE/MAX, Ford, Shutterstock, Condé Nast. 30M+ API calls/day, 99.99% uptime. | Backend engineering on the multi-tenant publishing pipeline, network integrations, and API surface |
| **[RogerRoger](https://rogerroger.io/)** | Unified inbox for sales — Email, LinkedIn, WhatsApp, Instagram and Telegram in one place; Kanban deal boards; CRM; shared drafts and team assignment | Inbox aggregation backend, provider adapters, deal/board APIs |
| **[MessageMind](https://messagemind.ai/)** | AI-driven omnichannel customer engagement across WhatsApp / Messenger / Instagram / web chat | Backend architecture, message pipeline, LLM integration |
| **[WeWise](https://wewise.co.il/)** | WhatsApp marketing automation, customer flow, and campaign analytics | Multi-tenant backend, campaign runtime, analytics ingest |
| **[FoorWeb](https://foorweb.net/)** | SaaS for customizable digital storefronts and business automation | Storefront service, tenant provisioning |
| **[NadlanOne](https://nadlanone.co.il/)** | Real-estate management with property listings, broker tools, analytics | Listings backend, broker workflows, dashboards |
| **[ZDSL](https://zdsl.com.bd/)** | Enterprise automation for real-estate service providers in Bangladesh | Enterprise backend, automation workflows |

## Selected open-source work

- **[mallahyari/system-design-visualizer#4](https://github.com/mallahyari/system-design-visualizer/pull/4)** — added Google Gemini as an alternative to OpenAI for image-to-diagram analysis. Merged Dec 2025.

## Stack

**Runtime & Language** — Node.js, TypeScript
**Frameworks** — NestJS, Express, Next.js
**Data** — MongoDB, PostgreSQL, MySQL, Redis
**Messaging & Realtime** — BullMQ, RabbitMQ, MQTT, Socket.io, Redis Pub/Sub, WebSockets
**Cloud & Ops** — AWS, DigitalOcean, Docker, Nginx, PM2, GitHub Actions
**Testing** — Jest, Supertest, Cypress, autocannon
**Cross-cutting** — GraphQL, REST, Webhooks, multi-tenant SaaS, caching, performance optimization

## Currently building

Public code artifacts for the production systems above:

1. **[api-latency-case-study](https://github.com/devhasibulislam/api-latency-case-study)** — *published.* Reproducible NestJS + Postgres + Redis reference for the 200ms → 20ms techniques. Docker Compose, autocannon benchmarks, atomic commits per optimization.
2. **`nestjs-multitenant-starter`** *(next)* — header/subdomain tenant resolver with Postgres RLS-based isolation, seed data, and isolation tests.
3. **`webhook-ingest-worker`** *(after)* — ingest → BullMQ → worker with idempotency, retry, backoff, and DLQ — the pattern behind MessageMind's message pipeline.

## Contact

<a href="https://www.linkedin.com/in/devhasibulislam/">LinkedIn</a> · <a href="mailto:devhasibulislam@gmail.com">Email</a> · <a href="https://devhasibulislam.vercel.app/">Portfolio</a> · <a href="https://t.me/devhasibulislam">Telegram</a> · <a href="https://wa.me/8801906315901">WhatsApp</a> · <a href="https://www.youtube.com/@devhasibulislam">YouTube</a>

---

<p align="center">
  <a href="https://github.com/devhasibulislam?tab=followers"><img src="https://img.shields.io/github/followers/devhasibulislam?style=flat&logo=github&label=Followers&labelColor=24292e&color=1f6feb" alt="GitHub followers" /></a>
  <a href="https://github.com/devhasibulislam?tab=repositories"><img src="https://img.shields.io/badge/Public%20Repos-see%20all-24292e?style=flat&logo=github" alt="Public repositories" /></a>
  <a href="https://github.com/devhasibulislam/api-latency-case-study"><img src="https://img.shields.io/github/stars/devhasibulislam/api-latency-case-study?style=flat&logo=github&label=Stars%20%C2%B7%20api-latency-case-study&labelColor=24292e&color=f7b32b" alt="Stars on api-latency-case-study" /></a>
</p>
