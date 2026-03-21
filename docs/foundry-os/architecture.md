# Architecture Overview

The **FoundryOS** relies on a clear, robust architecture to function as a resilient system rather than a fragile prototype. The architecture principles favor observability, simplicity, and ease of deployment.

## Core Architectural Principles
- **12-Factor App:** Applications must adhere to the 12-factor methodology for cloud-native readiness.
- **Reliability First Design:** Simple infrastructure > clever infrastructure. The foundation must be reliable enough to capture real data without collapsing.
- **Cost-Aware:** The architecture should fit within a defined cost envelope (targeting free tiers or low-cost serverless tools for the MVP).

## System Layers

### 1. The Presentation / Execution Layer
This is the interface the user interacts with. Whether it's a web app, mobile app, or internal tool, this layer must be instrumented from day one.
- **Tools:** Next.js, React, or lightweight no-code tools for MVPs.
- **Data Flow:** Captures user actions and sends events to the Observability layer.

### 2. The Application / Workflow Layer
This layer handles business logic, trigger-action mapping, and automation workflows.
- **Components:** Managed APIs, serverless functions (AWS Lambda, Vercel Functions), or workflow engines (Make, Zapier).
- **Data Flow:** Translates user actions into system state changes and external API calls.

### 3. The Infrastructure & Storage Layer
Where state is persisted. 
- **Components:** Managed databases (PostgreSQL, MongoDB), object storage (S3), and CDNs.
- **Characteristics:** Automated backups, separated environments (dev/prod).

### 4. The Observability & Analytics Layer
The most critical layer for a data-driven FoundryOS.
- **Components:** Logging (ELK, Datadog), APM (Sentry), Analytics (Mixpanel, Amplitude).
- **Data Flow:** Aggregates metrics to inform the Decision Engine.

## Data Flow: Idea to Execution
1. **Metadata Capture:** Raw ideas and constraints are saved as structured data.
2. **Scaffold Generation:** The OS outputs a functional repo structure and CI/CD pipeline based on the data.
3. **Event Tracking:** Defined event schemas are wired into the deployed app before traffic arrives.
4. **Feedback Loop:** Observability tools capture real-world traffic data and pipe it to decision dashboards.

## Environments
- **Local / Dev:** For rapid iteration.
- **Production:** Live URL with full observability instrumentation enabled.

*(For detailed visual representations, see [diagrams.md](./diagrams.md))*
