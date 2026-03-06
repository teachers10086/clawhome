# ClawHome / 龙虾之家

![License](https://img.shields.io/badge/license-MIT-green)
![Status](https://img.shields.io/badge/status-early-blue)
![Language](https://img.shields.io/badge/lang-English%20%7C%20中文-orange)

English | [中文](./README.zh-CN.md)

A curated home for the Claw ecosystem — projects, comparisons, naming notes, and deployment guidance.

> ClawHome is a curated directory of Claw-family open-source AI assistant projects on GitHub. It focuses on representative, ecosystem-shaping projects rather than claiming absolute completeness.

---

## What is ClawHome?

ClawHome is a guide to the emerging **Claw ecosystem**: a family of open-source AI assistant projects centered around **OpenClaw** and related derivatives, lightweight implementations, embedded variants, local-first forks, and orchestration layers.

This repository helps readers quickly answer questions such as:

- What are the main Claw projects on GitHub?
- What is each project for?
- Which project fits my environment?
- What is the difference between OpenClaw, PicoClaw, MimiClaw, LocalClaw, and Mimiclaw?
- Which projects are suitable for self-hosting, local inference, embedded deployment, or multi-agent orchestration?

---

## Quick Start

If you are new to the Claw ecosystem:

- Choose **OpenClaw** if you want the main self-hosted personal assistant experience.
- Choose **LocalClaw** if you prefer local-first deployment with local model providers.
- Choose **PicoClaw** if you want a lightweight, small-footprint assistant runtime.
- Choose **MimiClaw** if you want an embedded assistant on low-cost hardware.
- Explore **Mimiclaw** if you are interested in manager-worker or workforce-style multi-agent orchestration.

---

## Included Projects

This repository currently focuses on the following representative projects:

- OpenClaw
- MimiClaw (`memovai/mimiclaw`)
- PicoClaw
- LocalClaw
- Mimiclaw (organization / orchestration direction)

As the ecosystem evolves, more projects, forks, registries, and infrastructure tools may be added.

---

## Ecosystem Map

### A. Core assistant runtimes
Projects whose primary goal is to provide an AI assistant runtime.

- **OpenClaw** — the main self-hosted assistant platform
- **LocalClaw** — a local-first variant built around local model workflows
- **PicoClaw** — a lightweight runtime focused on small-footprint deployment
- **MimiClaw** — an embedded implementation for constrained hardware

### B. Orchestration / organization layer
Projects focused on agent teams, workforce-like execution, or manager-worker structures.

- **Mimiclaw** — a direction centered on orchestrating multiple agents

### C. Ecosystem infrastructure
Future entries may include:

- skill registries
- deployment tooling
- plugin ecosystems
- docs hubs
- community forks
- comparison dashboards

---

## Project Comparison

| Project | Primary Role | Best For | Deployment Style | Main Characteristics | Maturity |
|---|---|---|---|---|---|
| OpenClaw | Core self-hosted personal assistant | General-purpose self-hosted AI assistant | Desktop / server / self-hosted | Multi-channel, extensible, central runtime | Active |
| LocalClaw | Local-first assistant variant | Privacy-focused local usage | Local machine | Reduced cloud dependence, local models | Early-active |
| PicoClaw | Lightweight assistant runtime | Edge and low-resource experiments | Lightweight hardware / edge | Small-footprint, fast, minimal | Early |
| MimiClaw | Embedded assistant | Low-cost, low-power hardware assistant | Embedded device | ESP32-class direction, always-on hardware concept | Early |
| Mimiclaw | Multi-agent orchestration direction | Workforce / manager-worker experiments | Multi-agent setup | Parallel agent execution, organizational abstraction | Experimental |

> Notes:
> - “Maturity” here is a practical community-facing label, not an official upstream classification.
> - This table is intended for orientation, not as a benchmark.

---

## Detailed Entries

### 1) OpenClaw
**Type:** Core runtime / self-hosted personal AI assistant

**Best for:**
- users who want a general-purpose self-hosted assistant
- developers who want a central assistant runtime
- people who want multi-channel integrations and extensibility

**Typical environment:**
- desktop development machine
- home server
- VPS / self-hosted server

**Why it matters:**
OpenClaw is the conceptual center of the Claw ecosystem. Many related projects can be understood as simplifications, specializations, or extensions of the OpenClaw idea.

---

### 2) LocalClaw
**Type:** Local-first OpenClaw-style variant

**Best for:**
- users who prioritize privacy
- users who want to rely on local model providers
- people running local inference stacks

**Typical environment:**
- local development machine
- offline-friendly workflows
- local LLM setups

**Why it matters:**
LocalClaw represents the “local-first” direction in the ecosystem. It is useful for users who want more control over data, context, and inference dependencies.

---

### 3) PicoClaw
**Type:** Lightweight Claw-style assistant

**Best for:**
- resource-constrained deployments
- edge experiments
- minimal-footprint assistant runtime exploration

**Typical environment:**
- lightweight hardware
- edge devices
- experimental environments

**Why it matters:**
PicoClaw represents the “small, fast, portable” direction of the ecosystem.

---

### 4) MimiClaw
**Repository naming note:** `memovai/mimiclaw`

**Type:** Embedded assistant implementation

**Best for:**
- embedded and IoT experimentation
- low-cost always-on assistants
- highly constrained hardware use cases

**Typical environment:**
- embedded boards
- low-power devices
- experimental hardware assistants

**Why it matters:**
MimiClaw represents the hardware-native branch of the ecosystem.

---

### 5) Mimiclaw
**Type:** Orchestration / workforce-style multi-agent direction

**Best for:**
- users exploring manager-worker agent structures
- multi-agent experimentation
- organizational abstractions on top of assistant runtimes

**Typical environment:**
- multi-agent environments
- orchestration experiments
- task delegation workflows

**Why it matters:**
Mimiclaw represents the “AI organization” or “digital workforce” direction of the ecosystem.

---

## Naming Confusion

One of the most confusing parts of the ecosystem is the name **Mimiclaw**.

There are at least two different meanings people may refer to:

### `memovai/mimiclaw`
This repository is often introduced as **MimiClaw**, and is generally associated with the embedded / ESP32-style direction.

### `Mimiclaw`
This may also refer to a broader organization or orchestration direction related to multiple agents or workforce-like execution.

For clarity, **ClawHome treats them as separate entries**.

---

## Suggested Evaluation Dimensions

To keep the repository consistent, each project should ideally be described using the same dimensions:

- **Positioning** — personal assistant, local-first runtime, embedded assistant, orchestration layer, ecosystem infrastructure
- **Tech stack** — TypeScript, Go, C, local model stack, etc.
- **Deployment barrier** — desktop, server, Docker, embedded board, local LLM runtime
- **Interaction mode** — Telegram, Slack, WhatsApp, CLI, web, Matrix, etc.
- **Best-fit scenario** — personal automation, privacy-first assistant, edge deployment, hardware assistant, agent teamwork
- **Maturity** — stable, active, early, experimental

---

## Who is this repository for?

ClawHome is useful for:

- developers trying to understand the Claw ecosystem quickly
- users choosing between different Claw-style projects
- contributors tracking ecosystem directions
- readers comparing self-hosted, embedded, local-first, and multi-agent approaches

---

## Contribution Guide

Contributions are welcome.

You can help by:

- adding missing Claw-related projects
- correcting outdated descriptions
- improving classification and comparison criteria
- expanding deployment notes
- clarifying naming conflicts
- adding links to upstream repositories and docs

### Recommended submission format

When opening a PR, please include:

- project name
- repository link
- short summary
- main use case
- deployment environment
- notable technical characteristics
- maturity notes
- evidence from upstream README or docs

---

## Roadmap

Planned improvements for ClawHome:

- add more ecosystem entries
- add links to upstream repositories
- add a machine-readable project index
- add tags and filtering
- add deployment examples
- add a “which project should I choose?” section
- add ecosystem timeline

---

## Disclaimer

This is a community-curated overview repository.

Project scope, naming, positioning, and maturity may change quickly as the ecosystem evolves. Always verify important technical or deployment decisions against the upstream project repositories and official documentation.

---

## License

MIT
