# CR-DPO-CAT-08: Shard Subdivision (R5 Remedy — Two-Level Shards)

**Status**: Landed (this PR)
**Layer**: Catalog tooling (storage layout)
**Owner**: Emmanuel A. Otchere
**Date**: 2026-11-15
**Admission authority**: layout only (no record changes)
**Trigger**: Catalog population programme. The weekly reconciler (R5) flagged over-cap shard directories created by this programme's corpora (`contributions/queue/0-9` and `entities/v1-alpha/0-9` at 1,062 entries each — the CKAN dataset ids are opaque, so digit-prefixed slugs clustered) — remedy per entity-storage-layout.md §4 and the CR-MET-024/metrics subdivide recipe.
**Carrier**: Single PR on feature branch `feat/cr-dpo-cat-08`. PR review, not direct push.

## 1. What this CR does

1. **Subdivides the two over-cap shard directories into two-character sub-shards** (every resulting directory holds well under the 800-entry cap; GitHub's 1,000-entry listing cap respected).
2. **Upgrades the vendored toolchain to depth-3 shard walking**: `regenerate_catalog.py` (shard descent + relative-path rel-dir), `check_catalog_index.py` (shard descent), `check_contributions.py` (rglob queue walk). The shard-name test accepts 1–2 character alnum shards — digits included (`str.islower()` is False for pure-digit names, which is why the first regen after subdivision skipped 790 numeric-shard subtrees; caught locally, fixed here).
3. `CATALOG.yaml` regenerated; `counts.candidates: 2557` restored post-subdivision. Record ids are untouched (the admission hash excludes the slug, so re-sharding is id-stable).

## 2. Verification

- All gates green locally (parse/pointer/posture/queue/schema/documentation/index `--strict`/`regen --check`).
- R5 post-merge: the two over-cap findings for this repo are gone; `candidates: 2557` unchanged.

## 3. NOT-List

- No record content changes; no ids change; no canonical admissions.
- No gate-semantics changes beyond the depth-3 shard walk.
