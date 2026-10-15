<h1>Raul Silveira</h1>

Full-stack software developer in Brazil, building software for the power sector.

I work end to end: database and query plans, APIs, front-end, tests, deploy and
production support. Most of my days go into **Notus**, a supervision and outage
management platform used by power distribution companies to follow their grid
in real time.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-black?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/raulsilveirati/)
[![Discord](https://img.shields.io/badge/Discord-black?style=for-the-badge&logo=discord&logoColor=9580ff)](https://discord.com/users/raulsilveira)
[![Email](https://img.shields.io/badge/Email-black?style=for-the-badge&logo=gmail&logoColor=9580ff)](mailto:raulasacademico@gmail.com)

<h2>⚡ &nbsp;What I've been building</h2>

**Notus: from legacy desktop to a multi-client web platform**

- Replaced a set of legacy C++ desktop tools with a React + Fastify web
  application: event logs (SOE), outages, analog charts, load and voltage
  profiles, equipment and protection settings, and generation reports.
- One codebase serves clients on **Oracle, MariaDB and SQL Server**. Business
  rules live in a shared core and each database gets its own adapter, so a new
  client is configuration, not a fork.
- Reverse engineered a legacy C++ outage generator and rewrote it as a
  scheduled TypeScript service with an API and a fidelity harness against the
  original output.

**Performance on real utility data**

- Tables with tens of millions of SCADA events. Took a key Oracle query from
  16 s to 27 ms by keeping date math out of SQL so the index stays usable, and
  pushed deduplication, filtering and pagination into the database.
- Chart downsampling that keeps the minimum and maximum of each time bucket
  instead of averages, so short peaks and outages stay visible on long ranges.

**Quality and operations**

- About 1,000 unit and route tests, Playwright screen tests against a
  deterministic demo build with a frozen clock, and CI on GitHub Actions.
- Security hardening: mandatory JWT secrets, role-based access, rate limiting,
  Content-Security-Policy and environment validation at startup.
- Observability with Prometheus metrics and Grafana; Windows Server deploys
  behind Caddy with automatic HTTPS.
- A public demo that runs entirely in the browser, generating a coherent fake
  grid (weather, outages, events, load curves) so the product can be shown
  without exposing any customer data.

<h2>💻 &nbsp;Tech Stack</h2>

<div style="display: inline_block">
    <img align="center" alt="TypeScript" src="https://img.shields.io/badge/TypeScript-black?style=for-the-badge&logo=typescript&logoColor=white" />
    <img align="center" alt="Node.js" src="https://img.shields.io/badge/Node.js-black?style=for-the-badge&logo=nodedotjs&logoColor=white" />
    <img align="center" alt="Fastify" src="https://img.shields.io/badge/Fastify-black?style=for-the-badge&logo=fastify&logoColor=white" />
    <img align="center" alt="NestJS" src="https://img.shields.io/badge/NestJS-black?style=for-the-badge&logo=nestjs&logoColor=white" />
    <img align="center" alt="React" src="https://img.shields.io/badge/React-black?style=for-the-badge&logo=react&logoColor=white" />
    <img align="center" alt="Tailwind CSS" src="https://img.shields.io/badge/Tailwind_CSS-black?style=for-the-badge&logo=tailwindcss&logoColor=white" />
    <img align="center" alt="C#" src="https://img.shields.io/badge/C%23-black?style=for-the-badge&logo=csharp&logoColor=white" />
    <img align="center" alt=".NET" src="https://img.shields.io/badge/.NET-black?style=for-the-badge&logo=dotnet&logoColor=white" />
</div>
<br/>
<div style="display: inline_block">
    <img align="center" alt="Oracle" src="https://img.shields.io/badge/Oracle-black?style=for-the-badge&logo=oracle&logoColor=white" />
    <img align="center" alt="SQL Server" src="https://img.shields.io/badge/SQL_Server-black?style=for-the-badge&logo=microsoftsqlserver&logoColor=white" />
    <img align="center" alt="MariaDB" src="https://img.shields.io/badge/MariaDB-black?style=for-the-badge&logo=mariadb&logoColor=white" />
    <img align="center" alt="PostgreSQL" src="https://img.shields.io/badge/PostgreSQL-black?style=for-the-badge&logo=postgresql&logoColor=white" />
    <img align="center" alt="Prisma" src="https://img.shields.io/badge/Prisma-black?style=for-the-badge&logo=prisma&logoColor=white" />
    <img align="center" alt="Docker" src="https://img.shields.io/badge/Docker-black?style=for-the-badge&logo=docker&logoColor=white" />
    <img align="center" alt="Playwright" src="https://img.shields.io/badge/Playwright-black?style=for-the-badge&logo=playwright&logoColor=white" />
    <img align="center" alt="GitHub Actions" src="https://img.shields.io/badge/GitHub_Actions-black?style=for-the-badge&logo=githubactions&logoColor=white" />
</div>

<h2>☕ &nbsp;Off the keyboard</h2>

Coffee lover. Happiest when a slow query finally hits the index.
