# Hasibul Islam

**Senior Backend Architect · 7+ years · Node.js · NestJS · TypeScript · AWS**
Building multi-tenant SaaS platforms and real-time systems that hold up under production traffic.

Currently Sr. Backend Architect at [ZMC Technologies](https://zmc-technologies.com/), shipping backend infrastructure for AI-augmented omnichannel messaging, real-estate SaaS, and business-automation platforms.

Recent production win: cut a hot-path API from **~200ms → ~20ms** through query flattening, targeted indexing, cache-aside, and serialization changes. Reproducible reference: **[api-latency-case-study](https://github.com/devhasibulislam/api-latency-case-study)** — clone, `docker compose up`, `npm run bench`, see the delta on your machine.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-in%2Fdevhasibulislam-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devhasibulislam/)
[![Portfolio](https://img.shields.io/badge/Portfolio-devhasibulislam.vercel.app-2ea44f?style=flat&logo=vercel&logoColor=white)](https://devhasibulislam.vercel.app/)
[![Email](https://img.shields.io/badge/Email-devhasibulislam%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:devhasibulislam@gmail.com)
[![YouTube](https://img.shields.io/badge/YouTube-%40devhasibulislam-FF0000?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/@devhasibulislam)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=flat&logo=whatsapp&logoColor=white)](https://wa.me/8801906315901)

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

<a href="https://www.linkedin.com/in/devhasibulislam/">LinkedIn</a> · <a href="mailto:devhasibulislam@gmail.com">Email</a> · <a href="https://devhasibulislam.vercel.app/">Portfolio</a> · <a href="https://www.youtube.com/@devhasibulislam">YouTube</a> · <a href="https://wa.me/8801906315901">WhatsApp</a>

---

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=devhasibulislam&show_icons=true&hide_border=true&count_private=true&include_all_commits=true&hide=stars&theme=default" alt="GitHub stats" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=devhasibulislam&layout=compact&hide_border=true&langs_count=8&theme=default" alt="Top languages" />
</p>
