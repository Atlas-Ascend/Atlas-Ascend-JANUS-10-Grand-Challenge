# JANUS-10 Canonical Competition Pipeline

This pipeline is inherited by every JANUS-10 child repo. Entry-specific sponsor requirements may extend it but may not silently bypass a gate.

## State Machine

```text
DISCOVERED
  ↓ G0
ELIGIBILITY_VERIFIED
  ↓ G1
RULES_FROZEN
  ↓ G2
PRODUCT_LOCKED
  ↓ G3
BUILD_TRUTH_COMPLETE
  ↓ G4
SOFTWARE_DESIGN_COMPLETE
  ↓ G5
SCAFFOLDED
  ↓ G6
IMPLEMENTED
  ↓ G7
SPONSOR_TECH_PROVEN
  ↓ G8
VERIFIED
  ↓ G9
DEPLOYED
  ↓ G10
DEMO_PROVEN
  ↓ G11
SUBMISSION_READY
  ↓ G12
SUBMITTED
  ↓ G13
RESULT_ARCHIVED
```

## G0 — Eligibility Gate

Required proof:
- competition is currently accepting registration/submission or otherwise currently active;
- entrant category permits the actual entrant;
- geographic restrictions checked;
- solo/team constraints checked;
- age/status/student restrictions checked;
- registration prerequisite recorded;
- no known deadline has already expired.

**FAIL = do not build against that contest.** Move the product to a reserve target.

## G1 — Rules Snapshot Gate

Create child `COMPETITION/` files:
- `RULES_SNAPSHOT.md`
- `REQUIREMENTS.md`
- `JUDGING_RUBRIC.md`
- `IP_AND_PROVENANCE.md`
- `SUBMISSION_CHECKLIST.md`

Record source URL, capture date, deadline/timezone, required technologies, repository visibility requirement, demo/video limits, judging weights, prize path, ownership/licensing language, and pre-existing-code rules.

## G2 — Product Lock Gate

The child manifest must answer:
- What exact problem is solved?
- Who experiences it?
- What is the single judge-visible transformation?
- Why is this product non-obvious?
- Why does this competition sponsor technology materially matter?
- What is explicitly out of scope?

No generic “AI assistant” products pass this gate.

## G3 — 16 Build Truth Gate

Every child repo must contain these exact inherited filenames, adapted to the product and sponsor stack:

1. `01_PRODUCT_TRUTH.md`
2. `02_PROBLEM_USER_TRUTH.md`
3. `03_OUTCOME_REQUIREMENTS_TRUTH.md`
4. `04_SYSTEM_ARCHITECTURE_TRUTH.md`
5. `05_CASEGRAPH_TRUTH.md`
6. `06_AGENT_WORKFORCE_TRUTH.md`
7. `07_PACKET_EXECUTION_TRUTH.md`
8. `08_AUTHORITY_SAFETY_TRUTH.md`
9. `09_<SPONSOR>_INTEGRATION_TRUTH.md` — preserve position 09 while renaming sponsor-specific integration truth where appropriate
10. `10_DATA_TOOL_TRUTH.md`
11. `11_RUNTIME_OBSERVABILITY_TRUTH.md`
12. `12_SECA_VERIFICATION_TRUTH.md`
13. `13_PROOFGRID_EVIDENCE_TRUTH.md`
14. `14_UI_DEMO_TRUTH.md`
15. `15_HACKATHON_SUBMISSION_TRUTH.md`
16. `16_DEFINITION_OF_DONE.md`

Truth files describe reality and required evidence; they are not marketing copy.

## G4 — Software Design Gate

Minimum design surface:
- product/system specification;
- architecture and deployment topology;
- domain model / CaseGraph contract;
- state machine;
- authority/safety policy;
- agent/workforce contracts when agentic;
- sponsor runtime/integration design;
- tool adapter architecture;
- API/event contracts;
- persistence/replay design;
- observability;
- threat model;
- test strategy;
- UI/demo flow.

The design must make implementation choices explicit enough that another senior engineer could build it.

## G5 — Scaffold Gate

Required:
- runnable project structure;
- dependency manifests and lockfiles;
- environment example with no secrets;
- lint/typecheck/test commands;
- CI workflow where practical;
- local/dev start path;
- deployment target path;
- license/provenance notice.

## G6 — Implementation Gate

Definition:
- primary user journey works end-to-end;
- failure paths are handled;
- sponsor technology is inside the core path, not decorative;
- no hardcoded demo-only success response;
- no unimplemented critical UI control;
- all external calls surface deterministic error behavior.

## G7 — Sponsor-Tech Proof Gate

A judge must be able to see evidence of the required technology doing material work.

Proof may include:
- runtime logs;
- API requests/responses with secrets redacted;
- cloud console/runtime evidence;
- dependency/import evidence;
- trace spans;
- screenshots/video;
- source paths;
- reproducible verification command.

## G8 — SECA Verification Gate

Run, at minimum where applicable:
- install/build;
- unit tests;
- integration tests;
- lint;
- typecheck;
- security/secret scan;
- smoke test;
- primary E2E path;
- sponsor integration test;
- deployment health check.

A red required check blocks promotion.

## G9 — Deployment Gate

The judge-facing artifact must be reachable or reproducibly runnable under competition rules. Record deployment URL, build commit SHA, build time, environment, and health proof.

## G10 — Demo Gate

Demo sequence:
1. state the human problem in one sentence;
2. show input/problem state;
3. trigger the real system;
4. expose the key reasoning/automation/evidence path;
5. show the transformed outcome;
6. show sponsor technology proof;
7. show verification/provenance;
8. close on measurable impact.

No architecture-tour-first demos.

## G11 — Submission Ready Gate

Required package:
- competition title/category/track;
- product title and one-line thesis;
- public description;
- source repository state required by rules;
- working demo/deployment link;
- video within duration limit;
- screenshots;
- technology list;
- sponsor-tech explanation;
- judging-criteria mapping;
- IP/pre-existing work disclosure;
- team/entrant details;
- proof receipt;
- final deadline check.

## G12 — Submission Gate

A submission is only `SUBMITTED` when there is a portal confirmation, timestamp, submission identifier or equivalent receipt. A filled README is not submission proof.

## G13 — Result / Archive Gate

Capture:
- final submission SHA;
- submitted artifact links;
- confirmation receipt;
- judge feedback;
- placement/prize;
- reusable technical lessons;
- whether the product graduates into the broader estate, remains standalone, pauses, or archives.

## Timeboxing Law

Urgency does not remove gates. For short windows, reduce product scope, not truth/verification. The minimum winning build is a narrow complete system, not a broad broken system.

## Campaign Handoff

`JANUS-10 target ledger → child repo → Build Truth → Software Design → implementation → SECA → ProofGrid → competition portal → JANUS-10 result ledger`.