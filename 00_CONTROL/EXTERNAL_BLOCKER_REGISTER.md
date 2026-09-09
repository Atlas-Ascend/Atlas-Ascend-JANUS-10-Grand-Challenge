# JANUS-10 External Blocker Register

Snapshot: **2026-09-09**.

These are not software-baseline blockers. They are external credentials, registrations, organizer announcements, human media, or competition submission actions that cannot be truthfully promoted from repository code alone.

| Entry | External blocker | Owner/action required | Release behavior |
|---|---|---|---|
| JANUS | AWS/Strands live execution proof; Devpost registration; video/submission | entrant credentials + contest actions | keep deterministic runtime available; do not claim sponsor proof |
| HERMES | CALL-E API key; authorized phone target; required community PR; video/submission | entrant/CALL-E | `HERMES_MODE=demo` until live credentials exist |
| APOLLO | AssemblyAI API key; microphone demo; video/deck/submission | entrant/AssemblyAI | deterministic transcript fixture remains visibly synthetic |
| ATHENA | Sep 10 sponsor track/SDK announcement + registration | organizer + entrant | do not invent partner integration before kickoff |
| HEIMDALL | IBM Bob event access and Sep 25 kickoff | organizer + entrant | pre-event baseline remains disclosed; no Bob-built claim |
| HESTIA | final Alexa+ compatible/simulated end-to-end evidence; public/video/submission | entrant/Amazon contest | deployed MCP product may be tested independently |
| ARGUS | AWS credentials/resources and representative evaluation corpus | entrant/AWS | OpenCV 5 causal vision proof remains valid; AWS gate stays UNVERIFIED |
| ARTEMIS | local Ollama node; Nosana access/job; Arweave transaction capability | entrant/providers | hosted boundary demo remains synthetic for external compute/provenance |
| VULCAN | Nebius/NVIDIA credentials/model access | entrant/providers | deterministic tournament is valid; sponsor inference stays unclaimed |
| MAAT | Sep 18 challenge/track announcement | organizer + entrant | baseline stays pre-event and disclosed |

## Human-only campaign gates

The following require an explicit external human/account action and must not be fabricated:
- accepting contest terms / registration;
- providing API keys or cloud credentials;
- choosing an authorized real phone target;
- account billing/credit enrollment;
- publishing private repositories when the submission requires public source;
- recording/uploading entrant demo videos or pitch materials when an external hosting account is required;
- pressing final submission buttons and accepting submission attestations;
- tax/payment identity actions;
- claiming awards/results.

## Operational rule

When a blocker clears, the child repo should receive a fresh proof artifact containing the external run identifier, timestamp, exact release SHA, relevant provider IDs, verification result, and any redactions required for safe publication.
