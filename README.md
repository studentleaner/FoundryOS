# FoundryOS

## What this project is
The repository hosts two massive paradigms:

1. **FoundryOS** (The "Builder Muscle"). It is an end-to-end system that ingests a raw product idea, extracts metadata, enforces clarity through a rigid structural process, and outputs a live, hosted, observable system ready for real-world user validation. 
2. **The VentureOS** (The "Investor Brain"). This acts as a continuous risk-modeling and evaluation engine that monitors the Builder Muscle, analyzing real-world behavior to generate live data rooms, valuation models, and automated "Fund/Hold/Kill" verdicts.

*Not slides. Not theory. Something that runs.*

## Why it exists
Most founders spend months "building" when they are actually just "thinking." The market is flooded with knowledge providers (courses, books) and structure providers (templates, checklists) but is starved for **execution enforcers**. The OS forces decisions to be made based on execution signals rather than feelings. 

## Key idea
**Decision Compression.** We compress months of ambiguity into 24 hours of evidence. We do not teach strategy; we force decisions using real execution signals. By the end of the sprint, you will know if this product deserves the next 90 days of your life. 

## Features
- **Idea Intake & Metadata Extraction:** Forces clarity on the problem, ICP, and constraints.
- **Automated Workflow Engine:** Design core workflows (trigger → action → outcome) before writing code.
- **Built-in Observability:** Forces event tracking, error capture, and usage metrics from day one.
- **Decision Engine:** Automatically recommends whether to Kill, Continue, or Pivot based on actual traction metrics.
- **Single-Channel GTM:** Enforces a single-channel experiment to validate acquisition cost.

## How it works (high level)
1. **Intake:** Define the problem, target user, and constraints.
2. **Architecture:** Secure hosting, tech stack, and cost bounds.
3. **Workflow Design:** Automate the manual path with logic triggers.
4. **Execution:** Build the skeleton app or wire APIs.
5. **Observability:** Instrument the platform with logs and analytics.
6. **GTM Experiment:** Deploy one channel, measure conversion.
7. **Reality Check:** Review the data and decide to Kill, Pivot, or Scale.

## Architecture overview
The architecture prioritizes reliability, observability, and simplicity using the 12-Factor App methodology. It integrates standard presentation layers (Next.js/React or No-Code), unifies workflows via serverless triggers or API integration engines, persists state in managed storage (PostgreSQL/S3), and pushes absolute transparency through deep observability tooling.

For full details, see the [Architecture Document](./docs/foundry-os/architecture.md).

## Lifecycle overview
The system relies on the **12-Stage Canonical Lifecycle**:
1. Ideation & Intent
2. Validation
3. Business Design
4. MVP Spec
5. Analytics
6. GTM & SEO
7. Retention (PMF)
8. Operations & Revenue
9. Scale
10. Governance & Legal
11. Fundraising & PR
12. Exit Strategy

For the comprehensive breakdown, read the [12-Stage Lifecycle Framework](./docs/foundry-os/12-stage-lifecycle.md) and the [90-Day Roadmap](./docs/foundry-os/90-day-implementation-roadmap.md).

## Documentation Links

### Execution OS
- [System Overview](./docs/foundry-os/overview.md)
- [Architecture & Layers](./docs/foundry-os/architecture.md)
- [The 12-Stage Lifecycle](./docs/foundry-os/12-stage-lifecycle.md)
- [The 90-Day Implementation Roadmap](./docs/foundry-os/90-day-implementation-roadmap.md)
- [The 8-Pillar Meta-System](./docs/foundry-os/the-8-pillar-system.md)
- [Validation Mechanics](./docs/foundry-os/validation-mechanics.md)
- [Core Differentiators](./docs/foundry-os/core-differentiators.md)

### VentureOS
- [1. Landing Page & Vision](./docs/venture-os/1-landing-page-vision.md)
- [2. First Principles & Laws](./docs/venture-os/2-first-principles.md)
- [3. System Architecture Flow](./docs/venture-os/3-system-architecture.md)
- [4. Structural Evaluation Engine](./docs/venture-os/4-structural-evaluation-engine.md)
- [5. Competitor Threat & Reaction Engine](./docs/venture-os/5-competitor-threat-engine.md)
- [6. Multi-Agent Debate Architecture](./docs/venture-os/6-multi-agent-debate.md)
- [7. Probability Assignment Methodology](./docs/venture-os/7-probability-assignment.md)
- [8. Monte Carlo & Scenario Simulator](./docs/venture-os/8-monte-carlo-simulator.md)
- [9. Personal Strategic Mode (PSM)](./docs/venture-os/9-personal-strategic-mode.md)
- [10. VC Capital Mode (VCM)](./docs/venture-os/10-vc-capital-mode.md)
- [11. Mode Switching Logic](./docs/venture-os/11-mode-switching-logic.md)
- [12. Data Schema & Versioning](./docs/venture-os/12-data-schema.md)
- [13. System Roadmap & Extensions](./docs/venture-os/13-system-roadmap.md)
- [14. Versioning & Evolution](./docs/venture-os/14-versioning-evolution.md)

## License

MIT License

Copyright (c) 2024

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
