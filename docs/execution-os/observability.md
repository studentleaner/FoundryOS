# Observability

A system that cannot be observed does not exist in the Startup OS paradigm. Observability must be baked into the architecture from Day 1 to ensure that failures are visible and quantifiable.

## Core Observability Pillars

### 1. Logs
Every significant system event must be logged.
- **System Events:** Database interactions, third-party API payloads.
- **Audit Trails:** What user initiated what action and when.
- **Tools:** ELK Stack, Logtail, Datadog.

### 2. Metrics
The heartbeat of the infrastructure and the product.
- **System Metrics:** Uptime, latency, error rates.
- **Product Metrics:** Signups, feature usage, drop-offs *(see [analytics.md](./analytics.md))*.
- **Tools:** Prometheus, Grafana, CloudWatch.

### 3. Tracing
Essential for understanding latency and bottlenecks within distributed architectures.
- **Distributed Traces:** Correlation IDs tracking requests across microservices or serverless functions.
- **Tools:** Jaeger, Datadog APM.

### 4. Errors
An application without error tracking is flying blind.
- **Capture:** Unhandled exceptions, frontend crash reports.
- **Alerting:** Notifications routed directly to Slack or SMS when critical thresholds are breached.
- **Tools:** Sentry, Bugsnag.

## Implementation Strategy
- Implement observability before the first user arrives.
- "Log everything, alert on actionable anomalies."
- The system establishes baseline error rates and automatically flags deviations.
