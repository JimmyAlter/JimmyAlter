# Thiago Langone

**IT Infrastructure & Automation Engineer** — Buenos Aires, Argentina 🇦🇷

I look after the infrastructure of a six-company automotive dealer group: 30+ branch offices, 500+ Windows endpoints, six independent Active Directory domains. I don't only operate that environment — I build the tooling that runs it.

Most of my day is Windows, Active Directory, networking and PowerShell. The interesting part is what sits on top: an in-house RMM, internal MCP servers over PostgreSQL and SQL Server, and an LLM agent gateway where every security-critical path runs as deterministic code instead of model output.

---

## What I work on

**In-house RMM** — PowerShell agent running as SYSTEM on every workstation, PostgreSQL back end, Node/Express API, React dashboard. Hardware and software inventory, antivirus and disk alerts, online/offline state, remote command execution. 500+ endpoints across six companies.

**Agent platform** — an operations gateway on an LLM agent runtime: one orchestrator delegating to four isolated specialist agents, each with its own workspace and an explicit tool deny-list. Structured queries moved from 60–150 s of model inference to under 2 s by intercepting intent in code before the model ever sees the message.

**MCP servers** — five of them, exposing PostgreSQL and SQL Server to agents through fixed parameterized queries only. No free-form SQL reachable by the model, password columns excluded by construction, table allowlist validated in code rather than stated in a prompt.

**Provisioning tooling** — Active Directory and Google Workspace account operations (Express, ldapjs, Google Admin SDK), with confirmation required before anything writes.

---

## Public projects

| Project | What it is | Stack |
|---|---|---|
| [SystemMonitor](https://github.com/JimmyAlter/remote-monitoring-dashboard) | RMM console: inventory, metrics, remote commands, file and task management | React · TypeScript · Node/Express · PostgreSQL |
| [AssetDesk](https://github.com/JimmyAlter/AssetDesk) | IT service desk and asset inventory — tickets, device health, people directory | React · Vite · Node/Express · SQLite |
| [CommerceSuite](https://github.com/JimmyAlter/CommerceSuite) | B2B procurement platform with inventory tracking and status auditing | React · Vite · Node/Express |
| [Portfolio](https://github.com/JimmyAlter/thiagolangone) | Personal site | React · Vite · TailwindCSS |

---

## Tech

**Infrastructure** Windows Server · Active Directory (LDAP, OUs, GPO) · DNS · DHCP · TCP/IP · multi-site VPN · MikroTik · Linux (Ubuntu, Debian)

**Automation** PowerShell · Python · Bash · Node.js · Windows Task Scheduler

**Development** Node.js/Express · React · Next.js · TypeScript · TailwindCSS · REST APIs · PostgreSQL · SQL Server · SQLite · Git

**AI engineering** Multi-agent orchestration · per-agent tool policies · MCP server development · deterministic pre-inference interception · Ollama · Gemini API

**Operations** PDQ Inventory · Kaspersky Endpoint · Zammad · OTRS · Google Workspace Admin SDK and GAM

*Worked with, not claiming depth:* Prometheus · Grafana · OpenVPN · Hyper-V

---

## How I work

Read-only by default. Explicit confirmation before anything destructive. Access rules enforced in code, not written in a prompt and hoped for. Every system documented well enough that the next person doesn't have to rediscover it — including the parts that are broken and why.

---

## Open to

Remote roles in IT automation and infrastructure engineering, applied AI / agent engineering, or platform and internal-tooling work. Based in UTC−3, overlapping a full working day with US Eastern and Central hours.

📫 [thiagoivan029@gmail.com](mailto:thiagoivan029@gmail.com) · [Portfolio](https://thiagolangone.vercel.app) · [LinkedIn](https://www.linkedin.com/in/thiago-langone-365825229/)
