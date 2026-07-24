# Hasibul Islam

**Senior Backend Architect · 7+ years · Node.js, NestJS, TypeScript, AWS**
I build multi-tenant SaaS backends and real-time systems that hold up in production.

Currently Sr. Backend Architect at [ZMC Technologies](https://zmc-technologies.com/), shipping backend infrastructure for AI-augmented messaging, real-estate SaaS, and business-automation platforms.

The recent thing I'm proudest of: I took a hot-path API from **~200ms to ~20ms** by flattening the queries, adding the right index, dropping in a cache-aside layer, and cutting the serialization down to what the caller actually needs. I rebuilt the whole technique in a public repo: **[api-latency-case-study](https://github.com/devhasibulislam/api-latency-case-study)**. Clone it, `docker compose up`, `npm run bench`, and you can watch the delta on your own machine.

[![LinkedIn](https://custom-icon-badges.demolab.com/badge/LinkedIn-in%2Fdevhasibulislam-0A66C2?style=flat&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/devhasibulislam/)
[![Portfolio](https://img.shields.io/badge/Portfolio-devhasibulislam.vercel.app-2ea44f?style=flat&logo=vercel&logoColor=white)](https://devhasibulislam.vercel.app/)
[![Email](https://img.shields.io/badge/Email-devhasibulislam%40gmail.com-EA4335?style=flat&logo=gmail&logoColor=white)](mailto:devhasibulislam@gmail.com)
[![Telegram](https://img.shields.io/badge/Telegram-%40devhasibulislam-26A5E4?style=flat&logo=telegram&logoColor=white)](https://t.me/devhasibulislam)
[![WhatsApp](https://img.shields.io/badge/WhatsApp-Chat-25D366?style=flat&logo=whatsapp&logoColor=white)](https://wa.me/8801906315901)
[![YouTube](https://img.shields.io/badge/YouTube-%40devhasibulislam-FF0000?style=flat&logo=youtube&logoColor=white)](https://www.youtube.com/@devhasibulislam)

---

## What I do

I design multi-tenant NestJS backends: how the tenants are isolated, where the domain boundaries live, and how the background workers stay honest when the queue backs up.

I chase latency the boring way, by measuring. Query plans, connection pools, cache layers, serialization. Whichever one is lying about the p95, I want the number before and the number after.

I build ingestion pipes for AI-augmented messaging. WhatsApp, Messenger, Instagram, web chat, with the pieces that stop the LLM from ever finding out a delivery failed: idempotency keys, retry with backoff, dead-letter queues.

I own the whole path from schema to deploy. Not just the middle. Postgres and Mongo schemas, Docker, Nginx, PM2, GitHub Actions, AWS and DigitalOcean.

## Production systems

Most of the source is under NDA, so the list below is what you can go visit. I'm happy to walk through architecture and what was specifically mine in an interview.

| Product | What it is | What I worked on |
|---|---|---|
| **[Ayrshare](https://www.ayrshare.com/)** | Developer-first unified social-media API. One endpoint publishes, schedules, pulls analytics, and manages comments and DMs across 13+ networks (X, Facebook, Instagram, LinkedIn, TikTok, YouTube, Telegram, Threads, Bluesky, Reddit, Pinterest, Snapchat, Google Business). Ships a native MCP server for AI agents. 30M+ API calls a day at 99.99% uptime, powering 10,000+ teams including Ubisoft, Oracle, Red Hat, RE/MAX, Ford, Shutterstock, and Condé Nast. | Backend on the multi-tenant publishing pipeline, network integrations, and API surface |
| **[MessageMind](https://messagemind.ai/)** | AI agent that runs the whole front desk across WhatsApp, Gmail, Instagram, Outlook, Messenger, SMS/iMessage, voice, and web chat. Does six jobs out of the box (greet, qualify, book, follow up, resolve, escalate) and connects to 50+ tools like HubSpot, Salesforce, Calendly, Stripe, and Shopify with two-way sync. Meta Business Partner, GDPR compliant, Frankfurt hosting, 99.99% uptime, 5,000+ companies live, most in under 24 hours. | Backend architecture, cross-channel message pipeline, LLM orchestration, integration layer |
| **[RogerRoger](https://rogerroger.io/)** | Unified sales inbox that brings Email, LinkedIn, WhatsApp, Instagram, and Telegram into one place. Turns every message into a deal on a Kanban board, with shared drafts, task assignment, a lightweight CRM, and reminders so leads don't go cold. | Inbox aggregation backend, per-channel provider adapters, deal and board APIs |
| **[WeWise](https://wewise.co.il/)** | WhatsApp lead-automation for Israeli SMBs. Sits on your web form (WordPress, Wix, Rav-Messer, or anything with a webhook), fires a personalised WhatsApp message to every new lead within seconds, and pushes the same lead into your CRM in parallel. Reported outcomes with real customers: 26+ hours of unqualified-lead calls saved per month, ~28% lift in conversion. | Multi-tenant backend, webhook ingest, WhatsApp session management, CRM sync |
| **[FoorWeb](https://foorweb.net/)** | Algerian e-commerce SaaS. Free-to-paid store builder with 80+ shipping-carrier integrations, an app marketplace, local payment rails (BaridiMob, CIB, Dahabeya), digital-product delivery, abandoned-cart flows, and stock/order management. Founded 2018, part of the Foorweb group alongside FoorAi and FoorCall. | Storefront service, tenant provisioning, order/shipping/stock pipeline |
| **[NadlanOne](https://nadlanone.co.il/)** | Brokerage software that Israeli agencies have used for 20+ years. It runs the day-to-day of a real-estate office: the country's largest property feed updated in real time, CMA (comparative market analysis) reports, lead intake, tasks, digital signatures with unlimited contracts, WhatsApp and marketing automation, and call recording. | Listings backend, CMA report generation, broker workflows, marketing/WhatsApp automation |
| **[ZDSL](https://zdsl.com.bd/)** | Corporate and project portal for Zubion Development Solutions Limited, a Bangladeshi real-estate developer active since 2012 and part of the Zubion Group. Runs the project catalogue (ongoing, upcoming, completed), landowner and client portals, video galleries, project geo-map, and the group's REHAB/RAJUK/BLDA membership presentation. | Backend, project catalogue, landowner and client portals, media pipeline |

## Open source

- **[mallahyari/system-design-visualizer#4](https://github.com/mallahyari/system-design-visualizer/pull/4)** - I added Google Gemini as an alternative provider to OpenAI for the image-to-diagram analysis. Merged upstream in Dec 2025.

More coming as I publish the repos below.

## Stack

**Language and runtime:** Node.js, TypeScript
**Frameworks:** NestJS, Express, Next.js
**Data:** MongoDB, PostgreSQL, MySQL, Redis
**Messaging and realtime:** BullMQ, RabbitMQ, MQTT, Socket.io, Redis Pub/Sub, WebSockets
**Cloud and ops:** AWS, DigitalOcean, Docker, Nginx, PM2, GitHub Actions
**Testing:** Jest, Supertest, Cypress, autocannon
**Cross-cutting:** GraphQL, REST, webhooks, multi-tenant SaaS, caching, performance

## Currently building

I'm turning the patterns behind the production systems above into public reference repos, one at a time.

1. **[api-latency-case-study](https://github.com/devhasibulislam/api-latency-case-study)** - *published*. A reproducible NestJS + Postgres + Redis reference for the 200ms to 20ms techniques. Docker Compose, autocannon benchmarks, and one commit per optimization.
2. **`nestjs-multitenant-starter`** *(next)* - header and subdomain tenant resolvers, Postgres RLS for isolation, seed data, and tests that prove one tenant can't read another's rows.
3. **`webhook-ingest-worker`** *(after that)* - ingest, BullMQ, worker, with idempotency, retry with backoff, and a dead-letter queue. Same pattern that sits behind MessageMind's message pipeline.

## Contact

<a href="https://www.linkedin.com/in/devhasibulislam/">LinkedIn</a> · <a href="mailto:devhasibulislam@gmail.com">Email</a> · <a href="https://devhasibulislam.vercel.app/">Portfolio</a> · <a href="https://t.me/devhasibulislam">Telegram</a> · <a href="https://wa.me/8801906315901">WhatsApp</a> · <a href="https://www.youtube.com/@devhasibulislam">YouTube</a>

---

<p align="center">
  <a href="https://github.com/devhasibulislam?tab=followers"><img src="https://img.shields.io/github/followers/devhasibulislam?style=flat&logo=github&label=Followers&labelColor=24292e&color=1f6feb" alt="GitHub followers" /></a>
  <a href="https://github.com/devhasibulislam?tab=repositories"><img src="https://img.shields.io/badge/Public%20Repos-see%20all-24292e?style=flat&logo=github" alt="Public repositories" /></a>
  <a href="https://github.com/devhasibulislam/api-latency-case-study"><img src="https://img.shields.io/github/stars/devhasibulislam/api-latency-case-study?style=flat&logo=github&label=Stars%20%C2%B7%20api-latency-case-study&labelColor=24292e&color=f7b32b" alt="Stars on api-latency-case-study" /></a>
</p>
