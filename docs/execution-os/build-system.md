# Build System & Infrastructure

The build system in the Startup OS is designed to go from 0 to live in under 24 hours. The focus is exclusively on speed, proof of life, and observability.

## The Principles of the Build

1. **"Proof of life" over full product.** The goal isn't a finished product; the goal is a real user action producing a real system response.
2. **Standardization.** The Startup OS outputs a standard repository structure with basic CI/CD.
3. **No-Code / API Wiring first.** Before building a custom backend, attempt to wire APIs or use a no-code skeleton.

## Infrastructure Layers

### 1. Repository
- The system generates a boilerplate repo with pre-configured templating.
- **Tools:** GitHub, GitLab.

### 2. CI/CD Pipeline
- Continuous deployment is non-negotiable. Code that is pushed must be built and deployed without manual intervention.
- **Tools:** GitHub Actions, Vercel Deployments, AWS Amplify.

### 3. Hosting
- Default to cheap, managed, or serverless execution environments. The infrastructure must not require a dedicated DevOps resource initially.
- **Options:** Vercel, Heroku, AWS Lambda, Supabase (for DB + API).

### 4. Boilerplate / Templates
- Use off-the-shelf UI components and templates to assemble the front end instead of custom designing.
- Integration scaffolds (Stripe checkout, Supabase Auth) pre-configured.

## Output Deliverables
By the end of the Build phase (Hour 11-14), the outcome must be:
- A live URL.
- One functioning, testable user flow.
- A functional event pipeline that sends data to the Observability layer.
