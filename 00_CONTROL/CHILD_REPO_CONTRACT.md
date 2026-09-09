# JANUS-10 Child Repository Contract

Every repository created under this campaign is independent competition IP with a shared operating contract.

## Required Root

```text
README.md
LICENSE
BUILD_TRUTH/
SOFTWARE_DESIGN/
COMPETITION/
src/
tests/
demo/
proof/
```

## Required Build Truth Set

Create exactly sixteen truth documents at child-repo seed time:

```text
BUILD_TRUTH/
├── 01_PRODUCT_TRUTH.md
├── 02_PROBLEM_USER_TRUTH.md
├── 03_OUTCOME_REQUIREMENTS_TRUTH.md
├── 04_SYSTEM_ARCHITECTURE_TRUTH.md
├── 05_CASEGRAPH_TRUTH.md
├── 06_AGENT_WORKFORCE_TRUTH.md
├── 07_PACKET_EXECUTION_TRUTH.md
├── 08_AUTHORITY_SAFETY_TRUTH.md
├── 09_<SPONSOR>_INTEGRATION_TRUTH.md
├── 10_DATA_TOOL_TRUTH.md
├── 11_RUNTIME_OBSERVABILITY_TRUTH.md
├── 12_SECA_VERIFICATION_TRUTH.md
├── 13_PROOFGRID_EVIDENCE_TRUTH.md
├── 14_UI_DEMO_TRUTH.md
├── 15_HACKATHON_SUBMISSION_TRUTH.md
└── 16_DEFINITION_OF_DONE.md
```

Position 09 is deliberately sponsor-specific. For JANUS it is `09_STRANDS_INTEGRATION_TRUTH.md`; for APOLLO it should describe Gemini/Google Cloud + chosen partner; for ATHENA, RevenueCat/app-store integration; etc.

## Required Competition Set

```text
COMPETITION/
├── RULES_SNAPSHOT.md
├── REQUIREMENTS.md
├── JUDGING_RUBRIC.md
├── IP_AND_PROVENANCE.md
└── SUBMISSION_CHECKLIST.md
```

## Required Software Design Surface

Use the JANUS-Human-Admin-Zero design depth as baseline. Child repos must describe, at minimum:

1. Product system spec
2. System architecture
3. Domain model
4. CaseGraph/evidence graph contract when applicable
5. State machine
6. Authority/policy engine
7. Agent/workforce contracts when applicable
8. Sponsor runtime design
9. Tool adapter architecture
10. API/event contracts
11. Persistence/replay design
12. Runtime observability
13. Security/threat model
14. Verification/test strategy
15. UI/demo flow
16. Deployment topology

## Child README Contract

Every README must expose within the first screen:
- competition and track;
- deadline;
- one-line product thesis;
- exact human/user problem;
- required sponsor technology;
- demo command/link;
- current build state;
- verification command;
- provenance statement.

## Source / Provenance Law

A child may borrow **patterns and bounded adapters** from the Ghost Atlas estate, but any pre-existing source copied or materially adapted must be declared in `COMPETITION/IP_AND_PROVENANCE.md` when competition rules require disclosure. Never imply newly written hackathon code existed before the build window, and never imply pre-existing estate code was created during the hackathon.

## Promotion States

`SEED → RULES_LOCKED → TRUTH_LOCKED → DESIGNED → BUILDING → VERIFIED → DEPLOYED → SUBMISSION_READY → SUBMITTED → RESULT_ARCHIVED`

Promotion requires proof; status prose alone cannot promote a repository.

## Non-Reskin Test

Before product lock, answer YES to all:
- Does it solve a different primary problem from the other nine?
- Does its core user journey differ?
- Does its domain model differ?
- Does it exploit the sponsor technology for a necessary reason?
- Would a judge understand it as a standalone product without knowing Ghost Atlas?

Any NO blocks product lock.