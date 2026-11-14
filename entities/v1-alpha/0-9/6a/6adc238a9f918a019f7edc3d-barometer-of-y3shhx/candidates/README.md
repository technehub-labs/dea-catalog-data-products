# Barometer of companies with valid EGR qualifications by department – Legibat

> # Companies with a valid RGE qualification Statistics produced by **Metaleads**, operator of [Legibat](https://legibat.fr). Method and presentation: [https://legibat.fr/etude-couverture-rge](https://legibat.fr/etude-couverture-rge). ## Sources and date - [List of companies RGE — ADEME](https://data.ademe.fr/data-fair/api/v1/datasets/liste-des-entreprises-rge-2), updated: 2026-10-23T03:02:58.191Z. - [API Administrative division](https://geo.api.gouv.fr/departments), codes of municipalities and departments INSEE. - Observation as of 2026-10-24; 157884 source lines collected in full. ## Method SIREN separate by department, at least one qualification whose dates frame the extraction date inclusively. Fields broken down and then deduplicated by SIREN/department/domain; equality in lexical order. Communes and departments INSEE via API Administrative division. Invalid dates or SIRET and unresolved addresses are excluded and counted. Does not verify SIRENE administrative status, assurances or overall compliance. A company located in several departments is counted in each. The main domain is the one with the most distinct SIRENs. Departments without observation are present with zero staff. The file keeps the departmental codes as text, including 01, 2A and 2B. ## Quality and limits 0 lines with invalid dates; 0 with invalid SIRET; 468 active lines without a solved department. These first two categories may overlap. 56605 separate companies in solved departments. The departmental sum (58345) may exceed this total. "Active" in the column name means **valid qualification**, not administratively active establishment. This game is neither a certification nor an overall compliance measure. It does not contain the individual coordinates of the source. ## Reuse Open License 2.0 (`lov2`). Award: ADEME; INSEE repositories via API Administrative decoupage; Metaleads / Legibat treatment. Anticipated frequency: annual, to be carried out by the producer.

## Identity

- **Record id**: `dea:data-product-6adc238a9f918a019f7edc3d-barometer-of-y3shhx`
- **Type**: DataProduct
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the EU Open Data Portal hub search API. The dataset record is published and machine-verifiable at the cited landing page. No data-product-specific fields are asserted at candidate state.

- kind: `published-document` — reference: https://data.europa.eu/data/datasets/6adc238a9f918a019f7edc3d (data.europa.eu dataset 6adc238a9f918a019f7edc3d; publisher: Legibat - Observatoire de la Conformité BTP)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
