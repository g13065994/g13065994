<div align="center">

# Gerald Max

**Systems Software Engineer · Security Researcher · Automotive Mechatronics Track**

Runtime Architecture · Systems Diagnostics · Data Infrastructure · Embedded Systems

</div>

---

## Executive Brief

I build software around **runtime correctness, explicit system boundaries, resource constraints, and reliable data flow**.

My current work spans desktop systems software, automation runtimes, persistence architectures, full-stack applications, and application security. Across these projects, the recurring engineering problems are the same: controlling execution under constrained environments, defining stable interfaces between components, validating untrusted state, isolating failure domains, and keeping data access predictable as systems evolve.

That foundation is increasingly directed toward **low-level and automotive systems engineering** — particularly CAN/CAN-FD communication, ECU diagnostics, microcontroller firmware, sensor/actuator interfaces, telemetry acquisition, and resource-constrained embedded software.

The objective is not simply to build applications, but to understand the systems underneath them.

---

## Project Architecture

<table>
<tr>
<td width="50%" valign="top">

### Liquid WhatsApp

**Electron · Node.js · Chromium · Legacy macOS**

Unofficial desktop WhatsApp client engineered for **legacy Intel Macs running macOS Catalina**, with an emphasis on reliability under constrained hardware.

**Architecture**

- Isolated main-process caching architecture
- Custom runtime integrity verification
- Strict Content Security Policy and sandbox boundaries
- Localized FFmpeg binary transcoding pipeline
- Electron/Chromium process isolation
- Compatibility-oriented runtime behavior for legacy Intel hardware

**Engineering focus**

`Runtime Integrity` · `Process Isolation` · `IPC` · `Native Binaries` · `Legacy Systems`

<a href="https://github.com/g13065994/Liquid-Whatsapp-Intel-MacOS">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=g13065994&repo=Liquid-Whatsapp-Intel-MacOS&theme=dark&hide_border=true&show_owner=true" width="100%">
</a>

</td>

<td width="50%" valign="top">

### MATEO-FMB

**Node.js · ws3-fca · Event-Driven Runtime**

Facebook Messenger automation framework designed around **dependency contract stability and runtime resource control**.

**Architecture**

- Pinned `ws3-fca@3.5.2` dependency contract
- Host-aware runtime control-plane governor
- CPU and memory pressure monitoring
- Bounded event queues
- Message-pacing arrays for controlled throughput
- Runtime behavior designed for production pressure

**Engineering focus**

`Resource Governance` · `Event Queues` · `Backpressure` · `Dependency Contracts` · `Runtime Control`

<a href="https://github.com/g13065994/MATEO-FMB">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=g13065994&repo=MATEO-FMB&theme=dark&hide_border=true&show_owner=true" width="100%">
</a>

</td>
</tr>

<tr>
<td width="50%" valign="top">

### Mateo-XMD

**Node.js · Multi-Device Messaging · Persistence Abstraction**

Extensible multi-device WhatsApp automation engine built around a **unified data abstraction layer**.

**Architecture**

- Backend-independent persistence interface
- Hot-swappable storage implementations
- Un-indexed local JSON persistence
- Transactional SQLite storage
- Cloud MongoDB backend
- Separation between automation logic and persistence concerns

**Engineering focus**

`Data Abstraction` · `Persistence` · `Transactions` · `Backend Portability` · `Modular Runtime Design`

<a href="https://github.com/g13065994/Mateo-XMD">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=g13065994&repo=Mateo-XMD&theme=dark&hide_border=true&show_owner=true" width="100%">
</a>

</td>

<td width="50%" valign="top">

### ENKAYS-MINIMARKET

**Next.js · TypeScript · Prisma · PostgreSQL**

Full-stack commercial platform built around the **Next.js App Router** and a type-safe relational data layer.

**Architecture**

- Next.js App Router application model
- Server-side application logic
- Strict Zod request/data validation
- Prisma ORM relational mappings
- PostgreSQL persistence
- Typed boundaries between application and database layers

**Engineering focus**

`Type Safety` · `Relational Modeling` · `Server Validation` · `Data Integrity` · `Full-Stack Architecture`

<a href="https://github.com/g13065994/ENKAYS-MINIMARKET">
<img src="https://github-readme-stats.vercel.app/api/pin/?username=g13065994&repo=ENKAYS-MINIMARKET&theme=dark&hide_border=true&show_owner=true" width="100%">
</a>

</td>
</tr>
</table>

---

## Engineering Stack

| Domain | Technologies |
|---|---|
| **Languages** | JavaScript · TypeScript · SQL · HTML · CSS |
| **Application Frameworks** | Next.js · React · Electron |
| **Core Runtimes** | Node.js · Chromium · Electron |
| **Data Engineering** | PostgreSQL · Prisma · SQLite · MongoDB · JSON |
| **Validation & Contracts** | Zod · Dependency Pinning · Schema Validation |
| **Systems Engineering** | Process Isolation · IPC · Runtime Integrity · Resource Monitoring · Event Queues |
| **Media / Native Tooling** | FFmpeg · Native Binary Integration |
| **Application Security** | CSP · Sandboxing · Integrity Verification · Trust Boundaries |
| **Diagnostics** | Wireshark · Runtime Inspection · Network Analysis |
| **Development Infrastructure** | Git · GitHub · GitHub Actions |
| **Emerging Domain** | CAN/CAN-FD · ECU Diagnostics · Microcontrollers · Sensor/Actuator Systems |

---

## Engineering Principles

**Explicit contracts**  
Interfaces and dependencies should have predictable behavior and clearly defined boundaries.

**Bounded resources**  
Queues, workers, caches, and event pipelines should behave predictably under load instead of relying on unlimited growth.

**Isolation by default**  
Security boundaries and failure domains should be explicit at the process, runtime, and data layers.

**Validated state**  
Input crossing a trust boundary should be validated before it becomes application state.

**Portable abstractions**  
Core application logic should not become unnecessarily coupled to a single persistence engine or infrastructure provider.

**Observability**  
Systems should expose enough runtime information to diagnose their actual behavior rather than relying on assumptions.

**Deterministic behavior**  
Correctness matters most when a system is operating under constrained resources, degraded conditions, or unexpected input.

---

## Automotive Systems Direction

My software engineering work is increasingly converging with **automotive mechatronics and embedded systems**.

| Systems Layer | Engineering Direction |
|---|---|
| **Vehicle Network** | CAN / CAN-FD communication and frame analysis |
| **ECU Layer** | Diagnostics, communication protocols, fault-state analysis |
| **Embedded Compute** | Microcontrollers, peripherals, firmware architecture |
| **Telemetry** | Sensor acquisition, logging, structured data pipelines |
| **Control Systems** | Real-time resource management and deterministic execution |
| **Security** | Automotive communication and ECU trust boundaries |
| **Physical Interface** | Sensors, actuators, signal conditioning |

The long-term direction is to carry the same principles used in application and systems software into **embedded automotive environments where timing, memory, communication reliability, and hardware constraints become first-class engineering requirements**.

---

## Systems Perspective

```text
Application Layer
        │
        ▼
Runtime / Process Architecture
        │
        ├── IPC
        ├── Resource Governance
        ├── Integrity Verification
        └── Security Boundaries
        │
        ▼
Data / Persistence Layer
        │
        ├── JSON
        ├── SQLite
        ├── PostgreSQL
        └── MongoDB
        │
        ▼
Systems Diagnostics
        │
        ├── Network Analysis
        ├── Runtime Inspection
        └── Protocol Analysis
        │
        ▼
Embedded / Automotive Layer
        │
        ├── Microcontrollers
        ├── CAN / CAN-FD
        ├── ECU Diagnostics
        └── Sensors / Actuators
```

---

## Profile Telemetry

<!--
Minimal telemetry block — enable when the preferred providers are finalized.

GitHub activity:
https://github-readme-stats.vercel.app/api?username=g13065994&show_icons=true&theme=dark&hide_border=true

Commit activity:
https://streak-stats.demolab.com/?user=g13065994&theme=dark&hide_border=true

Language distribution:
https://github-readme-stats.vercel.app/api/top-langs/?username=g13065994&layout=compact&theme=dark&hide_border=true
-->

---

<div align="center">

**Systems Software → Embedded Systems → Automotive Diagnostics → Mechatronics**

</div>
