# JANUS-10 GRAND CHALLENGE

**Campaign ID:** GA-JANUS-10-2026  
**Owner:** Atlas-Ascend  
**Control Plane:** JANUS-10  
**Campaign State:** ACTIVE  
**Verified Competition Board:** 2026-09-08 America/Los_Angeles

JANUS-10 is the campaign control plane for ten independent, competition-grade software builds. Each child repository must be a genuinely distinct product solving a distinct problem. The Ghost Atlas estate may provide bounded architecture patterns, governance, verification, proof, and engineering leverage, but the competition repos are not allowed to become reskins of the same application.

## Campaign Law

1. One competition → one product → one repository → one submission ledger.
2. No fake completion. Every promotion requires executable evidence.
3. No replacement builds inside the Ghost Atlas estate. Reuse only through explicit bounded interfaces and documented provenance.
4. Competition rules outrank internal architectural preference.
5. Eligibility is a hard gate. Student-only contests are excluded from the canonical ten.
6. A banner prize number is not enough. Record cash, credits/tokens, category prize, deadline, and actual win path separately.
7. Each child repo inherits the JANUS-Human-Admin-Zero sequence: 16 Build Truth files → Software Design → Scaffold/Implementation → Verification → Demo → Competition package → Proof receipt.
8. Every submission must preserve IP provenance and disclose pre-existing components when rules require it.
9. Every product must have a judge-visible working path. Slides alone do not count.
10. Deadline pressure may reorder execution priority without renumbering entries.

## Canonical Ten

| # | Codename / Child Repo | Competition | Advertised Prize | Deadline | State |
|---|---|---|---:|---|---|
| 01 | `JANUS-Human-Admin-Zero` | AWS Agents for Humans Hackathon | $40,000 cash | Sep 14, 2026 | ACTIVE |
| 02 | `HERMES-Public-Access-Relay` | Build, Ship, Shape: Amazon Developer Hackathon | $138,000 cash | Oct 23, 2026 | REPO TO CREATE |
| 03 | `APOLLO-Studio-Operations-Intelligence` | Agentic Cinema: The Blockbuster Hackathon | $75,000 cash | Sep 9, 2026 | ACTIVE / P0 |
| 04 | `ATHENA-PeaceGraph` | RevenueCat Shipaton 2026 — Peace Prize lane | $740,000 cash campaign pool | Sep 30, 2026 | REPO TO CREATE |
| 05 | `HEPHAESTUS-Agent-Forge` | Nebius x NVIDIA Global AI Hackathon | $50,000 cash | Oct 30, 2026 | REPO TO CREATE |
| 06 | `THOTH-ARC-Reasoning-Lab` | ARC Prize 2026 — Paper Track | $450,000 total track pool | Nov 9, 2026 | REPO TO CREATE |
| 07 | `ARGUS-FieldVision` | OpenCV AI Competition 2026, powered by AWS | $20,250 cash | Oct 27, 2026 | REPO TO CREATE |
| 08 | `IRIS-CallRelay` | CALL-E: Your Code Is Calling | $10,000 cash | Sep 14, 2026 | REPO TO CREATE |
| 09 | `THEMIS-Legal-Proof-Engine` | BLI Legal Tech Hackathon 2 | ~$50,000 advertised bounties/support* | Nov 1, 2026 | REPO TO CREATE |
| 10 | `PLUTUS-x402-Agent-Commerce` | Algorand Global x402 Challenge | $100,000 USD + 500,000 ALGO | Sep 30 / early Oct 2026 | REPO TO CREATE |

\*BLI prize listings differ across aggregators; the competition ledger treats the final official bounty table as authoritative and requires re-verification before project lock.

## Deadline Execution Queue

**P0 — immediate:** APOLLO / Agentic Cinema (Sep 9).  
**P1 — next:** JANUS / Agents for Humans + IRIS / CALL-E (Sep 14).  
**P2 — September finish:** ATHENA / RevenueCat + PLUTUS / x402 (Sep 30).  
**P3 — October:** HERMES / Amazon (Oct 23), ARGUS / OpenCV (Oct 27), HEPHAESTUS / Nebius-NVIDIA (Oct 30).  
**P4 — November:** THEMIS / BLI Legal Tech (Nov 1), THOTH / ARC Paper Track (Nov 9).

## Child Repository Minimum Shape

```text
<CHILD_REPO>/
├── README.md
├── BUILD_TRUTH/                 # exactly 16 canonical truth files
├── SOFTWARE_DESIGN/             # product-specific design repo layer
├── COMPETITION/                 # rules, rubric, IP/provenance, submission checklist
├── src/                         # implementation
├── tests/                       # executable verification
├── demo/                        # judge-visible demo assets/scripts
├── proof/                       # receipts, screenshots, run evidence, hashes
└── LICENSE
```

## Command-to-Proof Pipeline

`TARGET → ELIGIBILITY → RULES SNAPSHOT → PRODUCT THESIS → 16 BUILD TRUTH → SOFTWARE DESIGN → SCAFFOLD → IMPLEMENT → INTEGRATE REQUIRED SPONSOR TECH → TEST → SECA GATE → DEPLOY → DEMO → SUBMISSION PACKAGE → PROOFGRID RECEIPT → SUBMIT → ARCHIVE RESULT`

See `00_CONTROL/PIPELINE.md` for gates and `00_CONTROL/COMPETITION_REGISTER.md` for the live target ledger.

## Current Definition of Campaign Success

JANUS-10 is successful when all ten child repos exist, each is independently competition-compliant, each has a working product and reproducible verification path, and every submitted claim can be traced to proof. Winning is the objective; ten high-grade shipped artifacts and a repeatable competition factory are the minimum durable output.