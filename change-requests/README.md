# Change Requests: dea-catalog-data-products

This index tracks every change request that lands on this repository.

| CR | Title | Status | Notes |
|----|-------|--------|-------|
| [CR-DP-CAT-01](CR-DP-CAT-01-catalogue-foundation.md) | Catalogue foundation (kit bring-up) | Landed (this PR) | Standard kit: pointer, dependencies, schema projection, gates 1-6, workflows, FOUNDATIONS, record standard. No records admitted. |
| CR-DP-CAT-02 | Initial population | Planned | Evidence-gated seed population per FOUNDATIONS §7. |

## Numbering

Series tag `CR-DP-CAT-NN`, sequential. Cross-repo CRs that touch this
repository are recorded here with their home-repo identifier.
| [CR-DPO-CAT-02](CR-DPO-CAT-02-dpo-cat-02.md) | Entity Ingestion Groundwork (candidate intake queue + gates) | **Proposed (this PR)** | Gated intake: queue + blocking queue gate + admission tool (candidate-state subtrees, content-derived ids); pin v2.6.0→v2.8.0 + shard-aware toolchain re-vendor. No records. |
| [CR-DPO-CAT-03](CR-DPO-CAT-03-dpo-cat-03.md) | DataProduct Candidate Corpus | **Landed (this PR)** | 2557 queue submissions from 1 bank(s); manifest with sha256s; queue gate CONFORMANT; no entities change. |
| [CR-DPO-CAT-04](CR-DPO-CAT-04-dpo-cat-04.md) | DataProduct Candidate Admission Batch 01 (Information about medical professionals … Programme Wind Energy Zone (SAPRO Wind Energy) Styria) | **Landed (this PR)** | Admitted 1400 `DataProduct` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1400, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-DPO-CAT-05](CR-DPO-CAT-05-dpo-cat-05.md) | DataProduct Candidate Admission Batch 02 (Local Property Tax LPT statistics October 2019 … Health centres and clinics in the municipality of Velike Lašče) | **Landed (this PR)** | Admitted 1157 `DataProduct` CANDIDATE records via the gated intake workflow (queue gate → admission tool → catalog gates); candidates +1157, canonical unchanged; records at `lifecycle_status: proposed` in `candidates/` subtrees. |
| [CR-DPO-CAT-06](CR-DPO-CAT-06-cr-dpo-cat-06.md) | CR Naming/Numbering Correction | **Landed (this PR)** | Programme batch CRs renamed to house-form CR-prefixed identifiers (mapping in the CR); content unchanged. |
| [CR-DPO-CAT-08](CR-DPO-CAT-08-cr-dpo-cat-08.md) | Shard Subdivision (R5 Remedy) | **Landed (this PR)** | Over-cap shards subdivided (two-character sub-shards); toolchain depth-3 shard walking incl. digit-shard name fix; candidates 2,557 restored; ids untouched. |
| [CR-DPO-CAT-09](CR-DPO-CAT-09-cr-dpo-cat-09.md) | Canonical Admission Wave (2557) | **Landed (this PR)** | 2557 records promoted candidates/ -> canonical root; ladder completed; evidence preserved; canonical 2557, candidates 0. |
