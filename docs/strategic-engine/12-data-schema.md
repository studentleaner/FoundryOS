# Data Schema & Versioning

Because ideas evolve as they iterate through the Personal Strategic Mode (PSM), the Strategic Intelligence Engine (SIE) is not a stateless calculator. It is a persistent database built to query how ideas improve or decay over time.

---

## 1. The Core Principle: Ideas Have Version History

When a founder realizes their initial idea has a weak moat, they will pivot the business architecture and re-submit it. The SIE tracks the exact delta between `Idea v1` and `Idea v2` to visually graph the strengthening of the strategic concept.

## 2. Standardized JSON Output Model

The system relies on an explicit, relational data structure to manage evaluations and probabilistic outcomes natively.

### Idea Source Table
Stores the raw inputs submitted by the human before any evaluations begin.
- `IdeaId`
- `Version` (v1, v2, v3...)
- `SummaryText`
- `TargetAudience`
- `DistributionPlan`

### Agent Scores Table
Logs the independent perspectives of the Multi-Agent Debate.
- `IdeaId`
- `AgentID` (VC, Risk, Infra, etc.)
- `RawScore`
- `AgentConfidence`
- `RebuttalScore` (If the score changed post-debate)

### Analysis Table
The aggregated synthesis holding the macroscopic metrics.
- `IdeaId`
- `ModeToggled` (PSM vs VCM)
- `StructuralScore`
- `ThreatScore`
- `DisagreementIndex` (The mathematical variance of the debate)

### Monte Carlo Simulation Table
Retains the results of the 1,000-run probabilistic engine.
- `IdeaId`
- `RunwaySurvivalProbability`
- `BestCaseExitOutcome`
- `WorstCaseCapitalLoss`
- `UpsideAsymmetryRatio`

By separating raw ideas, subjective agent scores, and raw probabilistic simulations, the system architecture becomes modular and allows historical querying (e.g., *"Show me all historical ideas that had an Infrastructure score > 8 but filed for bankruptcy within 12 months"*).
