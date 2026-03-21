# Workflow Engine & Automation

The Workflow Engine is the core process automation component of the FoundryOS. It prevents founders from performing manual, unscalable tasks and forces them to design robust operational systems from day one.

## Core Philosophy
We define workflows based on the **Trigger–Action–Outcome** framework. Every manual process must be mapped and eventually automated.

## Elements of a Workflow

### 1. Triggers
The catalyst for an action. Triggers can be:
- **User-initiated:** A user signs up, clicks a button, or submits a form.
- **System-initiated:** A scheduled cron job, a webhook from an external service, or a state change within the system.
- **Data-driven:** A threshold is crossed (e.g., metric drops below a certain SLA, or an error rate spikes).

### 2. States
The OS is a state-driven machine *(see [state-machine.md](./state-machine.md))*. Every workflow operates on entities that have precise states:
- e.g., `Lead` -> `Qualified` -> `Customer` -> `Churned`.
Workflows mutate these states deterministically.

### 3. Actions
The discrete tasks the system executes in response to a trigger:
- **API Calls:** Integrating with Stripe, Sendgrid, or CRMs.
- **Data Transformations:** Modifying, enriching, or filtering data.
- **Notifications:** Informing users or internal teams via email or Slack.

### 4. Events
The observable footprints left by the workflow. Every action execution emits an event that is captured by the Observability and Analytics modules.

## Happy Paths vs. Failure Paths
Most founders only design the "Happy Path." The FoundryOS forces the design of clear Failure Paths.
- **Error Capture:** If an API call fails, the workflow must log the error and transition the state to an error state.
- **Manual Automation Escalation:** If an automated workflow fails, an event is triggered to escalate to a human reviewer (Human-in-the-Loop orchestration).

## Deliverables from Workflow Design
- **Workflow Diagrams:** Visual maps of the triggers, actions, and data flows.
- **Trigger-Action Maps:** Explicit configuration documentation.
- **MVP Automation Scripts:** The actual implemented integrations (using Make, Zapier, or custom code pipelines).
