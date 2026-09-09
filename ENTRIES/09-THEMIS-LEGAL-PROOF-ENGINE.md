# Entry 09 — THEMIS / Legal Proof Engine

**Repo to create:** `Atlas-Ascend/THEMIS-Legal-Proof-Engine`  
**Competition:** BLI Legal Tech Hackathon 2  
**Advertised value:** approximately $50,000 bounties/support in current listings; official bounty table controls  
**Window:** through approximately Nov 1, 2026  
**Priority:** P4

## Product Thesis

An evidence-first legal/compliance reasoning engine that separates claims from sources, models obligations and exceptions, identifies missing proof, and produces an auditable review packet for a human decision-maker.

## Judge-Visible Transformation

`documents + question → claim/evidence graph → obligation/rule mapping → contradiction/gap detection → bounded analysis → review packet + provenance`

## Competition Fit

BLI emphasizes legal tech, RegTech, compliance, finance, blockchain and AI. THEMIS should target one official bounty only after the child repo snapshots the current DoraHacks bounty/rules table. Do not force blockchain into the product unless the selected bounty makes it materially useful.

## MVP Proof

Load a controlled legal/compliance case containing documents, assertions and incomplete evidence. THEMIS builds a provenance graph, cites each material conclusion to source evidence, marks unsupported claims, surfaces conflicting evidence and exports a structured review packet.

## Authority Boundary

THEMIS is legal/compliance decision support, not an autonomous lawyer or court. It must clearly distinguish source text, extracted facts, inferred relationships and recommendations.

## Win Characteristics

- extraordinary provenance discipline;
- practical reviewer workflow;
- clear evidence gaps rather than hallucinated certainty;
- selected protocol/bounty integration is useful;
- strong privacy/security model;
- judge can inspect exactly why each conclusion exists.