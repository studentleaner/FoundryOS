# Risk Models

The VentureOS evaluates startups by deconstructing them into fundamental, measurable risk vectors. If a risk vector exceeds acceptable parameters, the system penalizes the project's overall viability score.

## 1. Market & Traction Risk
The highest-weighted risk model. Evaluates if the market actually cares.
- **Execution Gap Viability:** Does the product's funnel convert faster/better than industry baselines?
- **CAC vs LTV Decay:** If Customer Acquisition Cost rises without a corresponding increase in LTV, the trajectory is penalized.
- **Activation Latency:** How long does it take for a signed-up user to trigger the "North Star" event? Speed reduces risk.

## 2. Technical & Infra Risk
Evaluates the robustness of the Builder Muscle.
- **Mean Time To Recovery (MTTR):** How fast does the system recover from an error tracked in Sentry?
- **Observability Coverage:** Are all critical workflows mapped with corresponding telemetry? Unmapped workflows increase risk.
- **Cost Scaling:** If server costs rise exponentially compared to user acquisition, architectural risk is flagged.

## 3. Execution & Team Risk
Evaluates the founder/team based strictly on execution velocity.
- **Decision Latency:** The time delta between a system alert (e.g., Conversion drop) and a code/workflow change designed to fix it.
- **Iteration Velocity:** How many distinct, observable workflow changes are made per week? Low iteration implies stagnation.

## 4. Cap Table & Structural Risk
An administrative evaluation primarily concerning investability.
- **Equity Dilution Forecast:** Assessing the cost envelope (runway) against the upcoming funding requirements.
- **Legal Hygiene Flagging:** Ensuring standard IP assignment and company registration logs exist in the data room.

## The Composite Score
All vectors are aggregated into the **VentureOS Viability Index (0-100)**. 
- **>80:** Highly Investable (Strong Fund signal).
- **50-79:** Operational (Hold/Pivot logic required).
- **<50:** Structurally Flawed (Kill signal).
