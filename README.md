# FoundryOS

## What this project is
**FoundryOS** (The "Builder Muscle") is an end-to-end execution system that ingests a raw product idea, extracts metadata, enforces clarity through a rigid structural process, and outputs a live, hosted, observable system ready for real-world user validation.

*Not slides. Not theory. Something that runs.*

*(Note: The strategic and capital evaluation engine, **VentureOS**, has been explicitly decoupled into its own repository: [https://github.com/studentleaner/VentureOS](https://github.com/studentleaner/VentureOS))*

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
