# JANUS-10 Repository Creation Queue

Create these repositories under `Atlas-Ascend` using the exact spelling below. Entry numbers remain canonical even if execution order changes.

## Existing — Do Not Recreate

1. `JANUS-Human-Admin-Zero`
3. `APOLLO-Studio-Operations-Intelligence`

## Create Now

2. `HERMES-Public-Access-Relay`
4. `ATHENA-PeaceGraph`
5. `HEPHAESTUS-Agent-Forge`
6. `THOTH-ARC-Reasoning-Lab`
7. `ARGUS-FieldVision`
8. `IRIS-CallRelay`
9. `THEMIS-Legal-Proof-Engine`
10. `PLUTUS-x402-Agent-Commerce`

## Recommended Creation Defaults

- Owner: `Atlas-Ascend`
- Initialize: empty repository is acceptable; JANUS-10 will seed it.
- Visibility: **private while building unless the competition requires public source earlier**. Change only when the rules demand it or at submission lock.
- README/license/gitignore: may be omitted during GitHub creation because the seed process supplies canonical files.
- Default branch: `main`.

## On Child Repo Detection

JANUS-10 should immediately perform this sequence:

```text
1. verify exact repo identity
2. re-check current competition rules
3. create README
4. create COMPETITION five-file snapshot
5. create the canonical 16 BUILD_TRUTH files
6. create SOFTWARE_DESIGN surface
7. seed source/test/demo/proof directories through real files
8. commit product-lock baseline
9. begin implementation against deadline priority
```

## Deadline-Driven Build Order After Repo Creation

```text
P0  APOLLO      Sep 09
P1  JANUS       Sep 14
P1  IRIS        Sep 14
P2  ATHENA      Sep 30
P2  PLUTUS      Sep 30 / early Oct
P3  HERMES      Oct 23
P3  ARGUS       Oct 27
P3  HEPHAESTUS  Oct 30
P4  THEMIS      Nov 01
P4  THOTH       Nov 09
```

## Creation Receipt

For every newly created repo, add its URL to `STATUS_BOARD.md` and record:
- creation timestamp;
- initial visibility;
- initial default branch;
- first seed commit SHA;
- rules verification timestamp;
- current promotion state.

Creating the empty repo is `SEED_PENDING`, not `BUILT`.