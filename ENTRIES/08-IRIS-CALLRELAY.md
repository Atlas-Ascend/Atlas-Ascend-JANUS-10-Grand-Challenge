# Entry 08 — IRIS / CallRelay

**Repo to create:** `Atlas-Ascend/IRIS-CallRelay`  
**Competition:** CALL-E: Your Code Is Calling  
**Prize:** $10,000 cash  
**Deadline:** Sep 14, 2026 11:45 PM SGT — official portal controls  
**Priority:** P1

## Product Thesis

A governed exception-resolution agent that turns an unresolved workflow into a purposeful real phone call, captures structured outcomes from the conversation and hands verified results back to the originating workflow.

## Judge-Visible Transformation

`unresolved exception → call objective + authority boundary → real outbound call → structured conversation events → verified outcome → workflow handoff`

## Core Difference

IRIS is not “an AI receptionist.” It is a bridge between digital workflows and the human phone channel when the only practical next step is to call somebody.

## MVP Proof

Start with a workflow blocked by missing confirmation. IRIS creates a bounded call brief, places a real call through the competition-required mechanism, states purpose appropriately, collects only authorized information, recognizes success/failure/ambiguity and returns a structured result with call metadata and follow-up requirements.

## Safety / Consent Contract

- identify the call purpose appropriately;
- no impersonation or deceptive identity;
- no harassment/repeated calling loop;
- no collection beyond necessary scope;
- sensitive data redacted from logs where appropriate;
- human escalation for ambiguous or consequential commitments.

## Win Characteristics

- real call, not simulated transcript;
- immediate practical value;
- strong state machine around call outcomes;
- excellent handling of interruption/voicemail/no-answer/ambiguity;
- structured post-call artifact;
- crisp two-minute demo.