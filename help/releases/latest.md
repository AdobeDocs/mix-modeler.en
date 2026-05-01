---
title: View the current Mix Modeler release notes
description: Latest Mix Modeler release notes
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
TQID: https://experienceleague.adobe.com/8o2hpkneIUMbBNEZfw9TsQLaGuPOxqF-XA2TV9cJnqc
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Mix Modeler
feature_v2:
  - id: ca6bcd6f-f5ca-4e5f-a5ae-7dce7177bde9
    internal-label: Release notes
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: bcc5edb5-84c3-4940-9f84-ed88b6c16274
    internal-label: Experimentation
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
autotag-review: '2026-05-01T09:06:55.437Z'
---
# Current Mix Modeler release notes

**Last update**: February 26, 2026.

These release notes cover the latest release of Mix Modeler. Mix Modeler releases operate on a continuous delivery model, which allows for an approximate monthly release cadence. Accordingly, these release notes get updated, so check them regularly.

## March 2026

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **Channel adstock** | You can incorporate domain expertise, experimentation results, or previous channel analyses directly into the model advanced configuration through [Channel adstock](/help/models/build.md#channel-adstock). And show [channel adstock insights](/help/models/insights.md#channel-adstock) within the channel analysis of a model. | March 30, 2026 | March 30, 2026 |

## February 2026

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **Harmonized factors workflow** | Factors are now managed as part of a [harmonized factors workflow](/help/harmonize-data/overview.md#factors). This simplifies how to [define factor data](/help/ingest-data/schemas.md#factor-standard-fields-field-group), how to [manage internal and external factors as part of your dataset rules](/help/harmonize-data/dataset-rules.md#factor-datasets), and how to use factor data in [models](/help/models/build.md#configure). | February 25, 2026 | February 25, 2026 |
| **[!UICONTROL Granular incrementality reporting]** | Define harmonized fields so you can drill down in the reporting of your model using [granular insights reporting fields](/help/models/build.md#granular-insights-reporting-fields), instead of having to create separate models. | February 18, 2026 | February 18, 2026 |

## January 2026

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset rules]** | [Updated dataset rules table](/help/harmonize-data/dataset-rules.md). You can search for one or more dataset rules and view, edit, or delete a dataset rule directly from the table.  | January 13, 2026 | January 13, 2026 |
| **[!UICONTROL Current spend]** | Add a current spend point in the [marginal response curve visualization](/help/models/insights.md#marginal-response-curves) in Model insights. | January 13, 2026 | January 13, 2026 |
| **[!UICONTROL Sort and resize columns]** | Added sort and resize of columns in the [Models](/help/models/overview.md) and [Plans](/help/plans/overview.md) table. | January 13, 2026 | January 13, 2026 |
| **Fixes** | Fixes for following tickets: <ul><li>AMM-3328: Field Input disabled for new operators for Factors</li><li>AMM-3359: Date picker and combobox lock up.</li><li>AMM-3441: Duplicating a plan does not auto fill in the date range and budget.</li></ul> | January 13, 2026 | January 13, 2026 |


## Release strategy

[!UICONTROL Mix Modeler] uses feature flags (also known as "toggles") to control the visibility of new features, allowing for controlled scale testing prior to full release. This release strategy includes the following phases:

* **Limited Testing**: A phased release begins with testing by internal Adobe users. It is then made available to a small group of customer accounts to ensure that the feature meets customer needs and expectations. 

* **Start of Rollout**: Rollout of a phased release begins with the Limited Testing phase. The release is then scaled from 0% to 100% availability to customers over the course of a couple months. Phased rollout happens at the Experience Cloud Organization level, so all entitled users in an organization receive the same experience.

