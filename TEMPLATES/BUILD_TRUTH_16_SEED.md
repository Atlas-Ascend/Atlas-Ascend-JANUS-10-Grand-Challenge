# JANUS-10 — 16 Build Truth Seed

Use this template to populate each child repo. Replace bracketed fields with competition-specific facts. Do not leave TODOs in a promoted `TRUTH_LOCKED` state.

## 01_PRODUCT_TRUTH.md
- Product name / codename / repo
- Competition + track
- One-line thesis
- Core primitive / transformation
- In scope / out of scope
- Why now / why this competition

## 02_PROBLEM_USER_TRUTH.md
- Primary user
- Pain / cost / failure mode
- Current workaround
- Critical user journey
- Accessibility constraints
- Evidence that the problem exists

## 03_OUTCOME_REQUIREMENTS_TRUTH.md
- Functional requirements
- Non-functional requirements
- Sponsor requirements
- Measurable success criteria
- Explicit non-goals
- Deadline constraints

## 04_SYSTEM_ARCHITECTURE_TRUTH.md
- Components
- Runtime topology
- Trust boundaries
- External dependencies
- Failure routes
- Data/control flow

## 05_CASEGRAPH_TRUTH.md
- Domain entities
- Relationships
- Evidence links
- State transitions
- Provenance fields
- Uncertainty / contradiction representation

## 06_AGENT_WORKFORCE_TRUTH.md
- Agent roles
- Tools/permissions
- Inputs/outputs
- Handoffs
- Stop conditions
- Human approval boundaries

## 07_PACKET_EXECUTION_TRUTH.md
- Atomic unit of work
- Required fields
- State machine
- Retry/idempotency behavior
- Completion evidence
- Failure/escalation path

## 08_AUTHORITY_SAFETY_TRUTH.md
- Permitted actions
- Forbidden actions
- Approval-required actions
- Data/safety constraints
- Threat/abuse cases
- Recovery behavior

## 09_<SPONSOR>_INTEGRATION_TRUTH.md
- Required sponsor technology
- Exact role in core path
- APIs/SDKs/models/services
- Proof mechanism
- Failure behavior
- Why this cannot be replaced by a decorative call

## 10_DATA_TOOL_TRUTH.md
- Inputs / outputs
- Data model
- Retention
- External tools
- Secret handling
- Data quality / validation

## 11_RUNTIME_OBSERVABILITY_TRUTH.md
- Logs
- traces/events
- metrics
- health checks
- correlation IDs
- judge-visible telemetry

## 12_SECA_VERIFICATION_TRUTH.md
- Unit/integration/E2E tests
- Lint/typecheck/build
- security/secret checks
- sponsor-tech checks
- deployment checks
- pass/fail promotion law

## 13_PROOFGRID_EVIDENCE_TRUTH.md
- Required receipts
- SHA/version linkage
- screenshots/video/logs
- provenance evidence
- submission confirmation
- durable archive fields

## 14_UI_DEMO_TRUTH.md
- Demo persona
- opening problem state
- primary interaction
- visible system action
- transformed outcome
- technical proof beat
- failure/recovery beat
- closing impact statement

## 15_HACKATHON_SUBMISSION_TRUTH.md
- Portal fields
- category/track
- word/video limits
- required URLs
- required source visibility
- technology declarations
- IP disclosure
- judging rubric mapping
- submission deadline/timezone

## 16_DEFINITION_OF_DONE.md
A child is done only when all applicable items are true:
- competition eligibility verified;
- rules snapshot current;
- all 16 truth files complete;
- design complete;
- primary feature implemented;
- sponsor technology materially integrated;
- required automated checks pass;
- deployment/reproducible run works;
- demo is recorded/tested;
- submission package complete;
- proof receipt binds artifact to commit SHA;
- portal submission confirmation captured.

`DONE != wrote code.`  
`DONE = competition-compliant working artifact + verification + proof + submitted receipt.`