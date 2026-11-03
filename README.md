<div align="center">

# Alex Beattie

**Software Engineer · Final-year SE @ Strathclyde · ex-BAE Systems · Co-founder, Khaotic Events**

*I build systems that real people depend on, then keep them running.*

<br/>

[![LinkedIn](https://img.shields.io/badge/LINKEDIN-161b22?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/alexanderbeattie04/)
[![Email](https://img.shields.io/badge/EMAIL-161b22?style=for-the-badge&logo=gmail&logoColor=white)](mailto:alexbeattie04@gmail.com)
[![Khaotic](https://img.shields.io/badge/KHAOTIC_EVENTS-161b22?style=for-the-badge&logo=soundcloud&logoColor=white)](https://khaotic.uk)

</div>

---

```text
> status      final year, graduating May 2027
> seeking     forward-deployed / client-facing engineering roles, summer 2027
> placement   BAE Systems, Jun 2025 - Jun 2026, rated "Exceeds Expectations"
> building    Khaotic OS, in production 24/7
> location    Glasgow, Scotland
```

<div align="center">

<img src="/github-metrics.svg" alt="GitHub metrics" width="100%"/>

</div>

---

## Khaotic OS / Hub

The operations platform behind a UK harder styles & techno promoter. **Solo build, in production 24/7**, replacing spreadsheets as the system of record for ticketing, finance and a rep sales network**.

```mermaid
flowchart LR
    subgraph Users
        R[200+ reps<br/>WhatsApp]
        O[Operators<br/>PWA]
    end

    subgraph VPS["Hetzner VPS · Cloudflare Tunnel · no public ports"]
        HUB["khaotichub<br/>Node · Express · TypeScript<br/>portal + BFF gateway"]
        REPS["khaoticreps<br/>Java 21 · Spring Boot<br/>WhatsApp bot + identity provider"]
        PG[(PostgreSQL)]
        SQ[(SQLite · WAL)]
        JOBS["systemd timers<br/>Skiddle sync · code entry bot · backups"]
    end

    R <--> |Twilio| REPS
    O --> HUB
    HUB --> |auth + proxy| REPS
    HUB --> PG
    REPS --> SQ
    JOBS --> PG
    JOBS --> |Playwright| SK[Skiddle]
    SQ -.-> |Litestream| R2[(Cloudflare R2)]
```

| | |
|---|---|
| **Rep engine** | Self-serve discount codes, live stats, leaderboards and automated recruitment over WhatsApp |
| **Attribution** | Skiddle API plus portal automation match ~2,900 orders to individual reps for per-event P&L and payouts |
| **Ops** | Role-based access across six roles, web push, Litestream replication with a tested restore, nightly backups, pre-deploy checks |

<sub>Production code is private. Happy to walk through the architecture in an interview.</sub>

---

## 🛰️ BAE Systems · Software Engineer, Industrial Placement

| Project | What I did | Stack |
|---|---|---|
| Full-stack internal platform | Owned the frontend, designed the schema, built the API | Angular, Node.js, PostgreSQL |
| Distributed cost metrics | Took over a legacy codebase, extended it inside an HLA simulation | Java, REST, HLA |
| DSEI UK 2025 | Simulation scenarios demonstrated live at the UK's largest defence exhibition | VBS, SQF |
| 3D interior editor | Self-directed: multi-floor buildings generated from OpenStreetMap data | Godot, C# |

<sub>Placement work was on internal systems, so it doesn't appear on this profile.</sub>

---

<div align="center">

![Java](https://img.shields.io/badge/Java-161b22?style=flat-square&logo=openjdk&logoColor=white)
![Spring Boot](https://img.shields.io/badge/Spring_Boot-161b22?style=flat-square&logo=springboot&logoColor=6DB33F)
![TypeScript](https://img.shields.io/badge/TypeScript-161b22?style=flat-square&logo=typescript&logoColor=3178C6)
![Node.js](https://img.shields.io/badge/Node.js-161b22?style=flat-square&logo=nodedotjs&logoColor=339933)
![Angular](https://img.shields.io/badge/Angular-161b22?style=flat-square&logo=angular&logoColor=DD0031)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-161b22?style=flat-square&logo=postgresql&logoColor=4169E1)
![SQLite](https://img.shields.io/badge/SQLite-161b22?style=flat-square&logo=sqlite&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-161b22?style=flat-square&logo=docker&logoColor=2496ED)
![Linux](https://img.shields.io/badge/Linux-161b22?style=flat-square&logo=linux&logoColor=FCC624)
![Cloudflare](https://img.shields.io/badge/Cloudflare-161b22?style=flat-square&logo=cloudflare&logoColor=F38020)
![Playwright](https://img.shields.io/badge/Playwright-161b22?style=flat-square&logo=playwright&logoColor=2EAD33)
![Godot](https://img.shields.io/badge/Godot-161b22?style=flat-square&logo=godotengine&logoColor=478CBF)

<sub>Currently: dissertation on digital twins of commodity supply chains · No-Gi BJJ blue belt · skiing</sub>

</div>
