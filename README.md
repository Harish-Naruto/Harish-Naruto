<h1 align="center">Harish Narote</h1>

<p align="center">
  <b>Backend &amp; Distributed Systems</b> · Go · gRPC · System Design
</p>

<p align="center">
  I build services meant to survive production, and solve problems in C++ for fun.
</p>

<p align="center">
  <a href="https://linkedin.com/in/harish-narote-600717339"><img src="https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn" /></a>
  <a href="mailto:harishnarote7@gmail.com"><img src="https://img.shields.io/badge/Gmail-EA4335?style=for-the-badge&logo=gmail&logoColor=white" alt="Gmail" /></a>
  <a href="https://leetcode.com/u/leandraw005/"><img src="https://img.shields.io/badge/LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode" /></a>
  <a href="https://www.codechef.com/users/mr_forgotten"><img src="https://img.shields.io/badge/CodeChef-4B4638?style=for-the-badge&logo=codechef&logoColor=white" alt="CodeChef" /></a>
</p>

## About

- I write **Go** for backend and distributed infrastructure: gRPC services, workflow orchestration, and real-time game servers.
- I learn **system design by building it**: control-plane / data-plane splits, DAG scheduling, Redis-backed state, and failure handling that actually gets exercised.
- Full-stack when a project calls for it, with **TypeScript**, React, and Turborepo monorepos.
- **Competitive programming in C++** on LeetCode and CodeChef.

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://www.gitskins.com/api/section/pet-device?username=Harish-Naruto&mode=light" />
  <img src="https://www.gitskins.com/api/section/pet-device?username=Harish-Naruto&mode=dark" alt="My GitHub contribution pet" />
</picture>

## Projects

### [Distributed Workflow Engine](https://github.com/Harish-Naruto/Distributed-Workflow-Engin)

*Go · gRPC · PostgreSQL*

Workflow orchestrator where pipelines are declared as DAGs in YAML. A coordinator parses and
validates the graph, detects cycles, persists state, and dispatches ready tasks to stateless
workers over bidirectional gRPC streams, so the control plane and data plane scale independently.

<!-- TODO screenshot: architecture diagram or a terminal capture of a DAG run -->

### [Space Striker](https://github.com/Harish-Naruto/Space-Striker-Server)

*Go · Gin · Gorilla WebSocket · Redis*

Real-time multiplayer Battleship backend on a clean-architecture layout. HTTP handles room
creation, then the connection upgrades to WebSockets for gameplay. Redis holds game state and
drives turn timeouts through Pub/Sub.

**[▶ Play it live](https://space-striker-client.harishnarote7.workers.dev/)**

<!-- TODO screenshot: a game in progress -->

### [Code Collab](https://github.com/Harish-Naruto/code-collab)

*TypeScript · Yjs · Turborepo · Supabase*

Collaborative code editor: several people editing at once with live cursors, backed by Yjs CRDTs.
Four services (API, WebSocket, Yjs, frontend) in a pnpm + Turborepo monorepo, Dockerised end to end.

<!-- TODO screenshot or GIF: two cursors editing the same file -->

### [UUID Generator](https://github.com/Harish-Naruto/UUID_Generator)

*Go · gRPC*

Snowflake-style 64-bit IDs served over gRPC: 41-bit timestamp, 10-bit worker identity, 12-bit
per-millisecond sequence, with a concurrency-safe counter.

### [URL Shortener](https://github.com/Harish-Naruto/URL-Shortener)

*Go · Gin · GORM · PostgreSQL*

Base62 link shortener where seven characters cover roughly 3.5 trillion URLs. HTTP API plus a
minimal landing page.

### [gRPC Streaming Patterns](https://github.com/Harish-Naruto/gRPC_method_Implementation)

*Go · gRPC · Buf*

All four RPC modes, unary, server-stream, client-stream and bidirectional, written out as a
working reference.

C++ problem solving lives in [DSAL](https://github.com/Harish-Naruto/DSAL), Go fundamentals in [golang](https://github.com/Harish-Naruto/golang).

## Tech Stack

**Languages**

<img src="https://skillicons.dev/icons?i=go,cpp,ts,js,py" alt="Go, C++, TypeScript, JavaScript, Python" />

**Backend &amp; Services**

<img src="https://skillicons.dev/icons?i=nodejs,express,bun" alt="Node.js, Express, Bun" />

gRPC · Protocol Buffers · Buf · Gin · GORM · WebSockets

**Frontend**

<img src="https://skillicons.dev/icons?i=react,nextjs,tailwind,vite" alt="React, Next.js, Tailwind CSS, Vite" />

**Data &amp; Storage**

<img src="https://skillicons.dev/icons?i=postgres,redis,supabase,prisma" alt="PostgreSQL, Redis, Supabase, Prisma" />

**Tooling &amp; Infra**

<img src="https://skillicons.dev/icons?i=docker,git,linux,cloudflare,pnpm" alt="Docker, Git, Linux, Cloudflare, pnpm" />

Turborepo · Make

## GitHub

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Harish-Naruto&theme=default" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/stats?username=Harish-Naruto&theme=github_dark" alt="Stars, commits, pull requests and issues" />
</picture>

<picture>
  <source media="(prefers-color-scheme: light)" srcset="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Harish-Naruto&theme=default" />
  <img src="https://github-profile-summary-cards.vercel.app/api/cards/most-commit-language?username=Harish-Naruto&theme=github_dark" alt="Languages by commit volume" />
</picture>

## Currently Learning

- **Distributed systems**: consensus, fault tolerance, and execution semantics under partial failure.
- **Retries and idempotency**, and what "exactly once" actually costs.
- **Production concerns**: backpressure, observability, and graceful degradation.
- **Go in depth**: concurrency patterns, context propagation, and testing discipline.

## Get in touch

Open to backend and distributed systems work. The fastest way to reach me is
[LinkedIn](https://linkedin.com/in/harish-narote-600717339) or
[harishnarote7@gmail.com](mailto:harishnarote7@gmail.com).
