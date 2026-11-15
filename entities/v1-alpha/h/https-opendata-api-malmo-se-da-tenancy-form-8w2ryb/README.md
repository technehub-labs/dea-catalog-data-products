# Tenancy form - Statistical data for Malmö's areas

> Shows the number of apartments divided by rental, tenant-owned or ownership. “Apartment” is used here to refer to both apartments in apartment buildings and single-family homes; a villa is considered an apartment in these statistics, for example. The number of apartments may be greater than the number of residential households if no one is registered in the apartment due to administrative delays, lack of a residence permit among those living in the apartment, failure to register on time, if no one simply lived in the apartment on 31/12 of the year the statistics apply or due to other similar reasons. All apartments included in the apartment register are included in the statistics, but only areas with more than 30 apartments in total are reported. Data from the apartment register. **Variable description** You find it [here](https://malmo.se/download/18.4968b1201a03e2e59771007/1791175330421/Variabelbeskrivning%20statistikunderlag%20f%C3%B6r%20Malm%C3%B6s%20omr%C3%A5den.pdf) ! **APIs** Using the API call _https://opendata%2dapi.malmo.se/api/3/action/resource_search?query=description:malm%C3%B6%20statistics,_ you can retrieve all data sets that contain statistical data for Malmö's areas in JSON format. In each instance of result/results in the JSON result, there is an "id" property for each resource. The value of "id" can be used to retrieve the data for the respective statistics variable (according to the value of the "name" property). API call to retrieve the statistics data: _https://opendata%2dapi.malmo.se/api/3/action/datastore_search?resource_id=[id value]_ Feel free to use the numbers, but cite “City Office, Malmö City” as the source.

## Identity

- **Record id**: `dea:data-product-https-opendata-api-malmo-se-da-tenancy-form-8w2ryb`
- **Type**: DataProduct
- **Version**: 0.1.0
- **Lifecycle**: proposed (candidate corpus; admitted via the gated intake
  workflow; canonical admission is a separate evidence-gated step)

## Evidence

Cited from the EU Open Data Portal hub search API. The dataset record is published and machine-verifiable at the cited landing page. No data-product-specific fields are asserted at candidate state.

- kind: `published-document` — reference: https://data.europa.eu/data/datasets/https-opendata-api-malmo-se-dataset-cc6f2194-2861-4fda-a279-b2f4e0be7861 (data.europa.eu dataset https-opendata-api-malmo-se-dataset-cc6f2194-2861-4fda-a279-b2f4e0be7861; publisher: Malmö stad)

## Classification-or-relationships

Deferred: relationship assertions are not made at candidate admission;
bindings land at canonical admission with per-assertion evidence.

## Provenance

Ladder passage: candidate (2026-11-14, Emmanuel A. Otchere).

## Governance

Functional owner: Emmanuel A. Otchere. Steward: Emmanuel A. Otchere. Approval: proposed
(candidate corpus; the approval decision belongs to canonical admission).
