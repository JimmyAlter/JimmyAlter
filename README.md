# Thiago Langone

**IT Infrastructure & Automation Engineer** — Buenos Aires, Argentina 🇦🇷

I look after the infrastructure of a six-company automotive dealer group: 30+ branch offices, 500+ Windows endpoints, six independent Active Directory domains. I don't only operate that environment — I build the tooling that runs it.

Most of my day is Windows, Active Directory, networking and PowerShell. The interesting part is what sits on top: an in-house RMM, internal MCP servers over PostgreSQL and SQL Server, and an LLM agent gateway where every security-critical path runs as deterministic code instead of model output.

---

## What I work on

**In-house RMM** — PowerShell agent running as SYSTEM on every workstation, PostgreSQL back end, Node/Express API, React dashboard. Hardware and software inventory, antivirus and disk alerts, online/offline state, remote command execution. 500+ endpoints across six companies.

**Agent platform** — an operations gateway on an LLM agent runtime: one orchestrator delegating to four isolated specialist agents, each with its own workspace and an explicit tool deny-list. Structured queries moved from 60–150 s of model inference to under 2 s by intercepting intent in code before the model ever sees the message.

**MCP servers** — five of them, exposing PostgreSQL and SQL Server to agents through fixed parameterized queries only. No free-form SQL reachable by the model, password columns excluded by construction, table allowlist validated in code rather than stated in a prompt. The pattern, rebuilt from scratch with its tests, is public: [guarded-sql-mcp](https://github.com/JimmyAlter/guarded-sql-mcp).

**Provisioning tooling** — Active Directory and Google Workspace account operations (Express, ldapjs, Google Admin SDK), with confirmation required before anything writes. A generalized PowerShell version of the AD side is public: [ad-lifecycle](https://github.com/JimmyAlter/ad-lifecycle).

---

## Public projects

| Project | What it is | Stack |
|---|---|---|
| [SystemMonitor](https://github.com/JimmyAlter/systemmonitor) | RMM console and agents: inventory, metrics, remote execution with every command audited against its operator | React · TypeScript · Node/Express · PostgreSQL · PowerShell |
| [guarded-sql-mcp](https://github.com/JimmyAlter/guarded-sql-mcp) | MCP server exposing PostgreSQL to LLM agents through a fixed catalog of read-only, parameterized queries | TypeScript · MCP SDK · PostgreSQL |
| [ad-lifecycle](https://github.com/JimmyAlter/ad-lifecycle) | PowerShell module for AD joiner / mover / leaver operations, `-WhatIf` on every write, Pester-tested | PowerShell · Pester |
| [AssetDesk](https://github.com/JimmyAlter/AssetDesk) | Small IT service desk and asset inventory: tickets, asset health, people directory | React · Vite · Node/Express · SQLite |
| [CommerceSuite](https://github.com/JimmyAlter/CommerceSuite) | Procurement storefront with server-side totals, stock and role checks | React · Vite · Node/Express · SQLite |
| [Portfolio](https://github.com/JimmyAlter/thiagolangone) | Personal site | React · Vite · TailwindCSS |

---

## Tech

**Infrastructure** Windows Server · Active Directory (LDAP, OUs, GPO) · DNS · DHCP · TCP/IP · multi-site VPN · Linux (Ubuntu, Debian)

**Automation** PowerShell · Python · Bash · Node.js · Windows Task Scheduler

**Development** Node.js/Express · React · TailwindCSS · REST APIs · PostgreSQL · SQL Server · SQLite · Git

**AI engineering** Multi-agent orchestration · per-agent tool policies · MCP server development · deterministic pre-inference interception · Ollama · Gemini API

**Operations** PDQ Inventory · Kaspersky Endpoint · Zammad · OTRS · Google Workspace Admin SDK and GAM

*Worked with, not claiming depth:* TypeScript · Next.js · Docker · MikroTik · FortiGate · Hyper-V · Prometheus · Grafana · OpenVPN

---

## How I work

Read-only by default. Explicit confirmation before anything destructive. Access rules enforced in code, not written in a prompt and hoped for. Every system documented well enough that the next person doesn't have to rediscover it — including the parts that are broken and why.

---

## Open to

Remote roles in IT automation and infrastructure engineering, applied AI / agent engineering, or platform and internal-tooling work. Based in UTC−3, overlapping a full working day with US Eastern and Central hours.

📫 [thiagoivan029@gmail.com](mailto:thiagoivan029@gmail.com) · [Portfolio](https://thiagolangone.vercel.app) · [LinkedIn](https://www.linkedin.com/in/thiago-langone-365825229/)
