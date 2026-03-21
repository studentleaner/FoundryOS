# Multi-Agent Debate Architecture

Single-model evaluation fails because one perspective dominates, hidden assumptions go unchallenged, and optimism bias creeps in. Real investment decisions involve conflict. 

The **Multi-Agent Debate Architecture (MADA v1)** creates a simulated investment committee to systematically stress-test ideas through forced disagreement.

---

## 1. The 7 Evaluator Agents

The system spawns 7 independent evaluation agents, each provided with the exact same standardized input JSON. They evaluate the idea through completely different lenses and biases.

1. **Founder Agent:** Bias: Optimistic. Focuses on MVP clarity, speed to market, and execution complexity. 
2. **Early VC Agent:** Bias: Power-law seeking. Focuses on 10x scaling potential, TAM, and exit paths.
3. **Risk Agent:** Bias: Conservative. Focuses on fragility, regulatory exposure, and incumbent retaliation.
4. **Commoditization Agent:** Bias: AI-era realism. Focuses on clone speed, open-source threats, and margin compression timelines.
5. **Infrastructure Depth Agent:** Bias: Long-term dominance. Focuses on stack position, data moats, and control plane potential.
6. **Distribution Agent:** Bias: Go-to-Market realism. Focuses on CAC pressure, channel leverage, and sales cycle friction.
7. **Capital Efficiency Agent:** Bias: Financial prudence. Focuses on burn rate risk, gross margin potential, and resilience under capital scarcity.

---

## 2. The Debate Flow

### Round 1: Independent Scoring
Each agent outputs a raw score (0-10), structured reasoning, critical risks/upsides, and a **Confidence Level (0-1)**.

### Round 2: The Rebuttal Phase
The system generates a *Disagreement Matrix*. If the Risk Agent scores a 4.0 but the Founder Agent scores an 8.5, both agents are shown the conflicting scores and forced to either defend their position or adjust their score. This simulates mathematical board debate.

### Round 3: Aggregation & Variance Penalty
The `FinalDecisionAgent` computes the composite score based on a role-based weight matrix (e.g., Risk and VC carry higher weights than Founder). 

> [!IMPORTANT]
> **The Disagreement Index:** If the standard deviation (σ) across the 7 agents is greater than 1.5, a strict **Variance Penalty** is applied to the final score. 
> 
> *Formula: Final Score = Mean × (1 − (σ / 10))*
> 
> High disagreement signifies mathematical uncertainty, heavily penalizing the idea's "safe" baseline score.
