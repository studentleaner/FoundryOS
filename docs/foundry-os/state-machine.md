# The State Machine Model

Most startup educational materials fail because they operate as a single, linear checklist. The reality of a startup is a series of interconnected states with regressions, dead ends, and parallel iterations.

The FoundryOS models the startup journey as a **State-Driven Machine**.

## The Necessity of State

- **Incomplete Stages:** Startups don't finish a stage perfectly. The OS tracks what is 'done', what is 'pending validation', and what is 'blocked'.
- **Regressions:** A failed GTM experiment might require the system to revert back to MVP Design (Stage 3) to fix an onboarding flow.
- **Dead Ends:** The system is explicitly designed to recognize when a branch of execution has failed completely.

## State Definitions

For every phase in the Startup Lifecycle, the System defines strict parameters:
1. **Entry Criteria:** What inputs and evidence are required to enter this stage.
2. **Exit Criteria:** What outputs and evidence are required to leave this stage and advance.
3. **Evidence Requirements:** The specific quantitative logic that determines 'success' (e.g., Conversion rate > 2%).
4. **Kill Switches:** An explicit scenario under which the project is aborted from this state.

## Operational Flow
The state machine does not allow progress without proof.
- *You cannot proceed to the Builder module (Execution) without first completing the MVP Architecture & Cost definition.*
- *You cannot define the GTM phase without an active URL and functional Event Tracking.*

The FoundryOS is a system that enforces discipline by strictly governing these state transitions.
