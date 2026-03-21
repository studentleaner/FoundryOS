# System Architecture

The **VentureOS** processes rough ideas through a ruthless, sequential gauntlet. An idea must survive one layer before it is permitted to pass to the next.

This document outlines the visual flow and data processing pipeline of the system.

---

## Visual Pipeline Diagram

```mermaid
flowchart TD
    A[Idea Input Data] --> B[Module A: Structural Evaluation Engine]
    
    B -->|Score < 6| R1[REJECT / PIVOT]
    B -->|Score > 6| C[Competitor Threat & Reaction Engine]

    C --> D[Multi-Agent Debate Architecture]
    
    D --> E[Probability Assignment Engine]
    
    E --> F[Monte Carlo & Scenario Simulator]
    
    F --> G{Mode Layer Decision}
    
    G -->|Idea needs refinement| H[Personal Strategic Mode (PSM)]
    G -->|Thresholds Met| I[VC Capital Mode (VCM)]
    
    H -.->|Repositioned Idea| A
    
    I --> J[Final Capital Allocation Plan]
```

---

## Architecture Breakdown

### 1. Idea Input
The pipeline begins with standardized JSON input. Ideas cannot be vague sentences. They must explicitly define the target market, the core problem, the proposed solution, and the initial business model assumptions.

### 2. Structural Evaluation Engine (Module A)
The engine immediately assesses the fundamental architecture of the idea. It tests for genuine market gaps, economic feasibility, structural moats, and severe regulatory/fraud risks. If the structural integrity fails, the idea is immediately killed or sent back for a pivot.

### 3. Competitor Threat & Reaction Engine
If structurally sound, the idea is subjected to the threat explicitly posed by incumbents. The system calculates a 7-dimensional **Competitor Threat Score** and simulates 24 months of incumbent retaliation to estimate inevitable margin compression.

### 4. Multi-Agent Debate Architecture
The idea and its initial scores are handed to the Debate Engine. Structured AI agents (The Optimistic Founder, The Power-Law VC, The Conservative Risk Officer, etc.) score the idea individually and debate conflicts. A Final Aggregator agent assigns a composite score with a computed **Disagreement Penalty**.

### 5. Probability Assignment Engine
To prevent overconfidence, point-scores are converted into probability distributions. Variables like *Market Adoption Velocity* and *Burn Rate Variability* are assigned Low/Medium/High likelihood curves based on the debate consensus.

### 6. Monte Carlo & Scenario Simulator
The probabilities are fired through a 1000-run Monte Carlo simulation to project the idea's potential futures. Best Case, Base Case, and Worst Case scenarios are generated to calculate the critical **Upside Asymmetry Ratio** and **Survival Probability**.

### 7. The Mode Layer
Finally, the results hit the Mode Routing logic:
- If the idea's differentiation and infra-depth scores are not high enough for capital allocation, it lands in **Personal Strategic Mode (PSM)** for advisory feedback and structural upgrades.
- If the idea hits elite thresholds, it graduates to **VC Capital Mode (VCM)** to undergo strict IRR and portfolio correlation modeling.
