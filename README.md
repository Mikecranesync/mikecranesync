# Mike Harpenau

**Maintenance technician turned founder** | 20+ years fixing industrial equipment | Building the AI layer for every PLC

> "Factory technicians spend 40% of their time diagnosing problems. What if they could just text their factory and ask what's wrong?"

[![FactoryLM](https://img.shields.io/badge/FactoryLM-Visit%20Site-1E3A8A?style=for-the-badge&logoColor=white)](https://factorylm.com)
[![YC W26](https://img.shields.io/badge/Y%20Combinator-W26%20Applicant-F97316?style=for-the-badge&logo=ycombinator&logoColor=white)](https://www.ycombinator.com/)
[![NVIDIA Cosmos](https://img.shields.io/badge/NVIDIA-Cosmos%20Cookoff%202026-76B900?style=for-the-badge&logo=nvidia&logoColor=white)](https://forums.developer.nvidia.com/t/the-nvidia-cosmos-cookoff-is-here/359090)

---

## What I'm Building

**FactoryLM** is a tiered intelligence system that pushes AI knowledge as close to the factory edge as possible — using deterministic code for common tasks and escalating to AI only when necessary.

```
Layer 3: Cloud AI (Claude, GPT)        — complex reasoning, novel problems
Layer 2: Local GPU (Llama 70B)         — medium complexity, air-gapped
Layer 1: Edge LLM (Raspberry Pi)       — real-time command translation
Layer 0: Deterministic Code + KB       — instant, free, THE GOAL
```

**The goal is to use LESS AI over time.** Every successful AI interaction gets converted into permanent code.

---

## Live Products

| Product | What It Does | Status |
|---------|-------------|--------|
| [**OpenClaw**](https://github.com/Mikecranesync/openclaw) | Industrial AI gateway — intent-aware LLM routing for factory diagnostics | Live on Telegram |
| [**FactoryLM CMMS**](https://github.com/Mikecranesync/factorylm-cmms) | ISO 55000 maintenance management, GitHub-native | In development |
| [**Industrial Skills Hub**](https://github.com/Mikecranesync/IndustrialSkillsHub) | Duolingo-style gamified training for maintenance techs | In development |
| [**Conveyor Demo**](https://github.com/Mikecranesync/factorylm-conveyor-demo) | VFD conveyor assembly — mechanical + electrical drawings | Built for YC demo |
| **factorylm.com** | Landing page | [Visit](https://factorylm.com) |

---

## The Demo

**Text your factory. AI tells you what's wrong.**

```
Phone → Telegram → OpenClaw → Live PLC Data → LLM Analysis → Diagnosis in <3 seconds
```

OpenClaw connects to **real Allen-Bradley Micro820 PLCs** via Modbus TCP, reads live tag values, runs fault detection, and returns actionable diagnosis to the technician's phone.

**Supported protocols:** Modbus TCP/RTU | EtherNet/IP | Siemens S7 | OPC UA

---

## Architecture

```
┌──────────┐  ┌──────────┐  ┌──────────┐
│ WhatsApp │  │ Telegram │  │   Slack  │
└────┬─────┘  └────┬─────┘  └────┬─────┘
     └─────────────┼─────────────┘
                   ▼
          ┌────────────────┐
          │    OpenClaw    │  Intent classification
          │   AI Gateway   │  Multi-provider LLM routing
          └───────┬────────┘
                  ▼
          ┌────────────────┐
          │  Intelligence  │  Layer 0 (code) → Layer 3 (cloud)
          │     Stack      │  Routes to cheapest capable layer
          └───────┬────────┘
                  ▼
          ┌────────────────┐
          │   PLC Edge     │  Raspberry Pi 4
          │   Gateway      │  Modbus / EtherNet/IP / S7 / OPC UA
          └────────────────┘
```

---

## Tech Stack

![Python](https://img.shields.io/badge/Python-3776AB?style=flat-square&logo=python&logoColor=white)
![FastAPI](https://img.shields.io/badge/FastAPI-009688?style=flat-square&logo=fastapi&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=flat-square&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-61DAFB?style=flat-square&logo=react&logoColor=black)
![Next.js](https://img.shields.io/badge/Next.js-000000?style=flat-square&logo=nextdotjs&logoColor=white)
![Raspberry Pi](https://img.shields.io/badge/Raspberry%20Pi-C51A4A?style=flat-square&logo=raspberrypi&logoColor=white)
![Docker](https://img.shields.io/badge/Docker-2496ED?style=flat-square&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat-square&logo=postgresql&logoColor=white)
![Tailscale](https://img.shields.io/badge/Tailscale-242424?style=flat-square&logo=tailscale&logoColor=white)

---

## GitHub Activity

<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=Mikecranesync&show_icons=true&theme=tokyonight&hide_border=true&count_private=true&include_all_commits=true" alt="GitHub Stats" height="165" />
  <img src="https://github-readme-stats.vercel.app/api/top-langs/?username=Mikecranesync&layout=compact&theme=tokyonight&hide_border=true&langs_count=8" alt="Top Languages" height="165" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=Mikecranesync&theme=tokyonight&hide_border=true" alt="GitHub Streak" />
</p>

---

## By the Numbers

- **20+ years** fixing industrial equipment (Allen-Bradley, Siemens, Fanuc)
- **4-layer architecture** validated from cloud AI to deterministic PLC code
- **< 3 second** diagnosis time from question to actionable answer
- **7 AI skills** live in production (diagnose, status, photo, work order, admin, search, chat)
- **$30/device/month** target pricing vs $500K+ incumbent solutions
- **$91B** total addressable market (predictive maintenance by 2033)

---

## Recent Activity

<!--START_SECTION:activity-->
1. ℹ️ Labeled issue [#5](https://github.com/Mikecranesync/factorylm-cmms/issues/5) in [Mikecranesync/factorylm-cmms](https://github.com/Mikecranesync/factorylm-cmms)
2. ❗ Opened issue [#5](https://github.com/Mikecranesync/factorylm-cmms/issues/5) in [Mikecranesync/factorylm-cmms](https://github.com/Mikecranesync/factorylm-cmms)
3. ℹ️ Labeled issue [#4](https://github.com/Mikecranesync/factorylm-cmms/issues/4) in [Mikecranesync/factorylm-cmms](https://github.com/Mikecranesync/factorylm-cmms)
4. ❗ Opened issue [#4](https://github.com/Mikecranesync/factorylm-cmms/issues/4) in [Mikecranesync/factorylm-cmms](https://github.com/Mikecranesync/factorylm-cmms)
5. 🗣 Commented on [#1](https://github.com/Mikecranesync/factorylm-cmms/issues/1#issuecomment-3880017611) in [Mikecranesync/factorylm-cmms](https://github.com/Mikecranesync/factorylm-cmms)
<!--END_SECTION:activity-->

---

## Featured Projects

<p align="center">
  <a href="https://github.com/Mikecranesync/openclaw">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Mikecranesync&repo=openclaw&theme=tokyonight&hide_border=true" />
  </a>
  <a href="https://github.com/Mikecranesync/factorylm-cmms">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Mikecranesync&repo=factorylm-cmms&theme=tokyonight&hide_border=true" />
  </a>
</p>
<p align="center">
  <a href="https://github.com/Mikecranesync/IndustrialSkillsHub">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Mikecranesync&repo=IndustrialSkillsHub&theme=tokyonight&hide_border=true" />
  </a>
  <a href="https://github.com/Mikecranesync/factorylm-conveyor-demo">
    <img src="https://github-readme-stats.vercel.app/api/pin/?username=Mikecranesync&repo=factorylm-conveyor-demo&theme=tokyonight&hide_border=true" />
  </a>
</p>

---

### Let's Talk

Building the AI layer for industrial automation. If you're an investor, factory operator, or maintenance professional — let's connect.

[![Email](https://img.shields.io/badge/Email-Contact%20Me-1E3A8A?style=flat-square&logo=gmail&logoColor=white)](mailto:mike@factorylm.com)
[![FactoryLM](https://img.shields.io/badge/factorylm.com-Visit-F97316?style=flat-square&logo=googlechrome&logoColor=white)](https://factorylm.com)

---

*Maintenance technician. Founder. Building what I wished existed for 20 years.*
