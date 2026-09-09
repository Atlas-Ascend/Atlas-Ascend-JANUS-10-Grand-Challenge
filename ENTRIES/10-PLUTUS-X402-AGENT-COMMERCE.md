# Entry 10 — PLUTUS / x402 Agent Commerce

**Repo to create:** `Atlas-Ascend/PLUTUS-x402-Agent-Commerce`  
**Competition:** Algorand Global x402 Challenge  
**Prize:** $100,000 USD top-five pool + 500,000 ALGO leaderboard pool  
**Application deadline listing:** Sep 30, 2026; challenge measurement/finalist process continues into early October  
**Priority:** P2

## Product Thesis

A machine-native commerce layer where software agents can discover a useful API capability, understand its price/contract, make an x402 payment, invoke the service and receive cryptographic and application-level proof that the paid capability was actually delivered.

## Judge-Visible Transformation

`agent need → capability discovery → price/contract → x402 payment → API execution → response → payment/service receipt`

## Competition Core

The paid endpoint must run on Algorand MainNet through the required x402 flow. The competition is usage-sensitive: a technically elegant endpoint with no legitimate use is weaker than a small capability people or agents repeatedly call.

## MVP Proof

Publish one genuinely valuable paid endpoint with a clean machine-readable contract. Demonstrate discovery, payment settlement, successful invocation, failed/insufficient-payment behavior, receipt generation and live usage telemetry. Then add an agent client that autonomously decides when the capability is worth purchasing under a bounded budget.

## Safety / Economic Boundaries

- explicit per-call and session budgets;
- no unlimited autonomous spending;
- idempotency/replay protection where needed;
- clear failure/refund semantics when service is not delivered;
- secrets/private keys never appear in repo or proof logs;
- testnet/local simulation before MainNet proof.

## Win Characteristics

- useful endpoint with a reason to pay;
- frictionless agent discovery and invocation;
- real MainNet settlement proof;
- credible usage/volume strategy without fabricated traffic;
- clean developer experience;
- strong observability and receipts;
- obvious long-term machine-economy potential.