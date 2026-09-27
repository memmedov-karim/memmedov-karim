<h1 align="center">Shikhkarim Mammadov</h1>

<p align="center">
  <b>Full-stack engineer · developer tooling &amp; platform engineering</b><br/>
  I build the tools other engineers work in — API testing platforms, engineering analytics, task intelligence.<br/>
  <sub>Competitive programmer · olympiad mathematician · Baku, Azerbaijan</sub>
</p>

<p align="center">
  <a href="https://callman.io"><img src="https://img.shields.io/badge/Product-callman.io-FF3C7E?style=for-the-badge&logo=hoppscotch&logoColor=white" alt="Callman"/></a>
  <a href="https://www.npmjs.com/~shikhkarim"><img src="https://img.shields.io/badge/npm-packages-CB3837?style=for-the-badge&logo=npm&logoColor=white" alt="npm"/></a>
  <a href="https://leetcode.com/Karimmammadov/"><img src="https://img.shields.io/badge/LeetCode-profile-FFA116?style=for-the-badge&logo=leetcode&logoColor=black" alt="LeetCode"/></a>
  <a href="https://www.hackerrank.com/sixkerimmemmedo1"><img src="https://img.shields.io/badge/HackerRank-profile-2EC866?style=for-the-badge&logo=hackerrank&logoColor=white" alt="HackerRank"/></a>
</p>

---

## About

- **What I do:** design and ship full products end to end — desktop clients, REST backends, admin panels, CLIs, CI runners and the deployment story around them.
- **Where I go deep:** multi-repo TypeScript platforms, test automation engines, on-prem/air-gapped delivery for banking-grade environments, and AI-assisted developer tooling (MCP servers, agent integrations).
- **Belief:** *the design of a project matters more than its code* — architecture that stays legible and a UI people actually enjoy beat clever implementations every time.
- **Background:** mathematics olympiads and ICPC-style contests — where I learned that the hard part is always the model, not the syntax.

---

## Featured work

### <img src="https://img.shields.io/badge/-flagship-FF3C7E?style=flat-square" alt=""/> Callman — API client &amp; test platform

> A Postman-alternative built for teams that cannot use the cloud. Collections, environments,
> multi-step test scenarios, contract checks, system-design diagrams — in a desktop app, a CLI,
> a REST backend and an MCP server, deployable fully on-premise.

[![callman-core](https://img.shields.io/npm/v/callman-core?style=flat-square&label=callman-core&color=CB3837&logo=npm&logoColor=white)](https://www.npmjs.com/package/callman-core)
[![callme-cli](https://img.shields.io/npm/v/callme-cli?style=flat-square&label=callme-cli&color=CB3837&logo=npm&logoColor=white)](https://www.npmjs.com/package/callme-cli)
[![callman-mcp](https://img.shields.io/npm/v/callman-mcp?style=flat-square&label=callman-mcp&color=CB3837&logo=npm&logoColor=white)](https://www.npmjs.com/package/callman-mcp)

**Eight repositories, one engine.** `callman-core` is the shared request/scenario runtime — the
desktop app, the backend, the CLI and the MCP server all execute requests through exactly the
same code path, so a scenario behaves identically on a laptop, in CI and on a bank's air-gapped
server.

| Surface | Stack | What it does |
| --- | --- | --- |
| **Desktop app** | Electron · React · TypeScript | The product UI: request editor, visual scenario canvas, diagram editor, UI-test recorder |
| **Core engine** | TypeScript | Request execution, scenario graph runtime, assertions, contract checks, AI prompt layer |
| **Backend** | Express · Mongoose · workers | Workspaces, collaboration, scheduling, scenario runner, approval flows |
| **CLI runner** | Node.js | CI-friendly collection runs, HTML/JSON reports, exit codes |
| **MCP server** | Model Context Protocol | Lets Claude Code, Cursor, Codex and Gemini CLI drive a Callman account through the REST API |
| **Admin panels** | NestJS · React · pnpm workspaces | Cloud and on-prem control planes (licensing, users, LDAP, storage, analytics) |
| **On-prem** | Docker Compose · Helm · Kubernetes | Air-gapped deployment, TLS/mTLS, LDAP auth, Prometheus metrics |

**Engineering highlights**

- **Protocol breadth beyond HTTP** — Kafka produce/consume with a pooled client layer, PostgreSQL stored-function testing with transactional rollback, Redis and database steps inside a single scenario graph.
- **Security &amp; enterprise auth** — OAuth2 flows, mutual TLS, LDAP/AD integration, Windows DPAPI-backed secret storage, scoped personal access tokens.
- **Scenario engine** — a directed graph of request / condition / loop / sub-scenario / AI nodes with variable propagation, retries, approvals and replayable run reports.
- **AI, centralised** — one prompt/parser layer in `callman-core` powering the in-app assistant, scenario generation and the MCP tool surface, with BYOK and managed key modes.
- **Ships like enterprise software** — Helm charts, offline install bundles, per-company desktop builds with electron-updater feeds, `/ops` JSON + Prometheus endpoints, in-app release notes gated in CI.

<br/>

### DevSense — engineering intelligence

> Multi-provider DORA, cycle-time, throughput and review-quality analytics for banking-grade
> engineering organisations. Self-hosted bundle or SaaS.

Ingests GitLab, GitHub and Bitbucket into **one canonical data model**, so the metrics engine and
the UI never touch provider-specific types — a new provider is just another adapter.

`NestJS` · `React + Vite` · `BullMQ workers` · `MongoDB` · `Redis` · `Turborepo` · pluggable AI providers

<br/>

### TaskSense — task intelligence platform

> Provider-agnostic task and delivery intelligence, built as a clean pnpm + Turborepo monorepo
> with its own MCP app so agents can work the backlog alongside humans.

`NestJS (OpenAPI)` · `React + Vite` · `Tailwind v4 design tokens` · shared TS/ESLint/Prettier presets · MCP

---

## How I work

- **Design first.** Information architecture and interaction design before implementation — for the UI *and* the module graph.
- **One engine, many surfaces.** Shared runtimes over duplicated logic; if two clients can disagree about behaviour, they eventually will.
- **Built for the worst environment.** Air-gapped, proxied, LDAP-only, no internet — if it works there, it works anywhere.
- **Automate the boring part.** Codegen, CI gates, release tooling and AI agents wired into the actual workflow, not bolted on.

---

## Tech stack

**Languages**

![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)
![Java](https://img.shields.io/badge/Java-ED8B00?style=flat-square&logo=openjdk&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![C++](https://img.shields.io/badge/C++-00599C?style=flat-square&logo=cplusplus&logoColor=white)

**Frontend**

![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Vite](https://img.shields.io/badge/Vite-646CFF?style=flat-square&logo=vite&logoColor=white)
![TailwindCSS](https://img.shields.io/badge/Tailwind-06B6D4?style=flat-square&logo=tailwindcss&logoColor=white)
![React Query](https://img.shields.io/badge/TanStack_Query-FF4154?style=flat-square&logo=reactquery&logoColor=white)
![Electron](https://img.shields.io/badge/Electron-47848F?style=flat-square&logo=electron&logoColor=white)

**Backend**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=flat-square&logo=nodedotjs&logoColor=white)
![Express](https://img.shields.io/badge/Express-000000?style=flat-square&logo=express&logoColor=white)
![NestJS](https://img.shields.io/badge/NestJS-E0234E?style=flat-square&logo=nestjs&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-6DB33F?style=flat-square&logo=springboot&logoColor=white)

**Data &amp; messaging**

![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=flat-square&logo=mongodb&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![MySQL](https://img.shields.io/badge/MySQL-4479A1?style=flat-square&logo=mysql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DC382D?style=flat-square&logo=redis&logoColor=white)
![Kafka](https://img.shields.io/badge/Kafka-231F20?style=flat-square&logo=apachekafka&logoColor=white)

**Infra &amp; delivery**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat-square&logo=kubernetes&logoColor=white)
![Helm](https://img.shields.io/badge/Helm-0F1689?style=flat-square&logo=helm&logoColor=white)
![Prometheus](https://img.shields.io/badge/Prometheus-E6522C?style=flat-square&logo=prometheus&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/CI-2088FF?style=flat-square&logo=githubactions&logoColor=white)
![Linux](https://img.shields.io/badge/Linux-FCC624?style=flat-square&logo=linux&logoColor=black)

**AI &amp; tooling**

![MCP](https://img.shields.io/badge/Model_Context_Protocol-000000?style=flat-square&logo=anthropic&logoColor=white)
![Anthropic](https://img.shields.io/badge/Claude-D97757?style=flat-square&logo=anthropic&logoColor=white)
![OpenAI](https://img.shields.io/badge/OpenAI-412991?style=flat-square&logo=openai&logoColor=white)
![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=flat-square&logo=vitest&logoColor=white)
![pnpm](https://img.shields.io/badge/pnpm-F69220?style=flat-square&logo=pnpm&logoColor=white)
![Turborepo](https://img.shields.io/badge/Turborepo-EF4444?style=flat-square&logo=turborepo&logoColor=white)

<sub>Also: Arduino &amp; embedded tinkering, Kali Linux, and far too much time spent on developer ergonomics.</sub>

---

## Delivered for clients

| Project | What it is |
| --- | --- |
| [muallim.edu.az](https://muallim.edu.az/) | Azerbaijan educational news portal |
| [edu-live.com](https://test.edu-live.com/) | International opportunities portal |
| [teamportal.info](https://www.teamportal.info/) | Exam management system |
| [kingjob.pro](https://www.kingjob.pro/) | Applicant tracking system |

---

## Competitive programming &amp; olympiads

[![E-Olymp](https://img.shields.io/badge/E--Olymp-sixkerim-0B7285?style=flat-square)](https://www.eolymp.com/az/users/sixkerim)
[![LeetCode](https://img.shields.io/badge/LeetCode-Karimmammadov-FFA116?style=flat-square&logo=leetcode&logoColor=black)](https://leetcode.com/Karimmammadov/)
[![CodeChef](https://img.shields.io/badge/CodeChef-kerim__288-5B4638?style=flat-square&logo=codechef&logoColor=white)](https://www.codechef.com/users/kerim_288)
[![HackerRank](https://img.shields.io/badge/HackerRank-profile-2EC866?style=flat-square&logo=hackerrank&logoColor=white)](https://www.hackerrank.com/sixkerimmemmedo1)

<details>
<summary><b>Awards &amp; certificates</b></summary>

<br/>

| Achievement | |
| --- | --- |
| International Mathematical Olympiad — participant | [certificate](https://drive.google.com/file/d/1oouH60xq481QR0eQc_JHTBEvhmaEDzNe/view) |
| Mathematical Olympiad of Azerbaijan — **Bronze Medal** | [certificate](https://drive.google.com/file/d/1cJWwpw1ehEecZEoA8bJaTna1AhPXind9/view?usp=sharing) |
| ICPC Azerbaijan Regional Contest 2021 — Honorable Mention | [certificate](https://drive.google.com/file/d/1r8w_xKJyU4OXyG3Jo_jS97MaZS8NZMQh/view?usp=sharing) |
| ICPC Azerbaijan Regional Contest 2020 — Honorable Mention | [certificate](https://drive.google.com/file/d/1AL1DGykg1JO1adURDfRo65v_yAhk6k9E/view?usp=sharing) |
| SnackDown 2021 — Global Programming Competition | [certificate](https://drive.google.com/file/d/1oHm3w6kGVGOsm8ZnuO4neMDM2gdYRDri/view) |
| HackerRank — Python (Skill Certificate) | [certificate](https://www.hackerrank.com/certificates/d1d4b4b40e0c) |
| HackerRank — JavaScript (Skill Certificate) | [certificate](https://www.hackerrank.com/certificates/855c3e400598) |

</details>

---

## GitHub

<p align="center">
  <img height="165" src="https://github-readme-stats.vercel.app/api?username=memmedov-karim&show_icons=true&include_all_commits=true&count_private=true&hide_border=true&theme=radical&bg_color=0D1117&title_color=FF3C7E&icon_color=FF3C7E" alt="GitHub stats"/>
  <img height="165" src="https://github-readme-stats.vercel.app/api/top-langs/?username=memmedov-karim&layout=compact&langs_count=8&hide_border=true&theme=radical&bg_color=0D1117&title_color=FF3C7E" alt="Top languages"/>
</p>

<p align="center">
  <img height="165" src="https://streak-stats.demolab.com?user=memmedov-karim&hide_border=true&theme=radical&background=0D1117&ring=FF3C7E&fire=FF3C7E" alt="GitHub streak"/>
</p>

<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=memmedov-karim&theme=radical&no-frame=true&no-bg=true&column=7&margin-w=8" alt="Trophies"/>
</p>

---

<p align="center">
  <sub>Currently building <a href="https://callman.io"><b>Callman</b></a> — and shipping it into places the internet cannot reach.</sub>
</p>
