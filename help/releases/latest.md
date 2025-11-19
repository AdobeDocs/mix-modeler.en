---
title: View the current Mix Modeler release notes
description: Latest Mix Modeler release notes
feature-set: Experience Cloud
feature: Release Notes
exl-id: 38a47672-2af2-437c-b769-4d5febb941f5
---
# Current Mix Modeler release notes

**Last update**: November 12, 2025.

These release notes cover the latest release of Mix Modeler. Mix Modeler releases operate on a continuous delivery model, which allows for an approximate monthly release cadence. Accordingly, these release notes get updated, so check them regularly.



## November 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Plans tracking]** | Allow users to understand how the execution of marketing plans tracks to what is planned. So you can feel confident how marketing performs. Or identify opportunities and risks earlier to correct course and achieve business goals. The [Performance to plan visualizations](/help/dashboard/plans.md#performance-to-plan) are updated and allow configuration for metric and granularity. | November 12, 2025 | November 12, 2025 |
| **[!UICONTROL Channel synergy insights]** | Reveals how marketing channels work together to create greater impact. With these insights, you can confidently explain past marketing performance and adjust marketing spend accordingly to maximize the overall return of your marketing portfolio. A Channel synergy matrix is available in [Model insights](/help/models/insights.md#channel-synergy) and [Plan insights](/help/plans/insights.md#channel-synergies). | November 12, 2025 | November 12, 2025 |
| **Fixes** | Fixes for following tickets: <ul><li>AMM-2920: Plans creation flow and migration.</li><li>AMM-3282: Scientific notation for vary small numbers in large grids.</li></ul> | November 12, 2025 | November 12, 2025 |


## September 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Dataset mapping validations]** | Added validations to Experience Platform dataset mappings for harmonized fields. | September 9, 2025 | September 9, 2025 |
| **[!UICONTROL Context menu on links to model and plans]** | Enabled browser context menu on links to models and plans. You can now use that browser context menu to open a specific plan or model in a new tab or window. | September 9, 2025 | September 9, 2025 |
| **Fixes** | Fixes for following tickets: <ul><li>AMM-3101: Fixed incorrect mapping creation for rules: `event_date` was passed as field name instead of `timestamp`.</li><li>AMM-3092: Fixed unable to change the channel max constraint value on a duplicated budget based plan.</li><li>AM3130: Fixed wrong **[!UICONTROL Run frequency]** information on a detail popup window of a model.</li><li>AMM3158: Updated labels for the **[!UICONTROL Select target metric]** options as part of the **[!UICONTROL Optimize]** pane in the [Plans create](/help/plans/build.md) interface.</li><li>AMM 3176: Fixed unable to view [Breakdown by channel](/help/models/insights.md#breakdown) visualization in **[!UICONTROL Attribution]** tab in **[!UICONTROL Model Insights]**.</li></ul> | September 9, 2025 | September 9, 2025 |
| **Fixes** | Fixes for following tickets: <ul><li>AMM-3174: Improved experience when no existing plans are available.</li><li>AMM-3216: Enhanced validation for custom date ranges.</li><li>AMM-3240: Fixed run model frequency display.</ul> | September 23, 2025 | September 23, 2025 |


## July - August 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **[!UICONTROL Compare plans update]** | The [Compare plans](/help/plans/compare.md) UI now shows additional details for paid marketing:  ROI or CPA, and revenue. | August 20, 2025 | August 20, 2025 | 
| **Harmonization updates** | All datasets rules now use a similar [generic Map to harmonized fields experience](/help/harmonize-data/dataset-rules.md), irrespective of the dataset type. When you map a standard harmonized field from a summary dataset, Mix Modeler tries to deduce the corresponding Experience Platform dataset field automatically. | July 29, 2025 | July 29, 2025 |


## May - June 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **Goal based plans** | Next to budgets, you can define a goal (target) when you [create](/help/plans/build.md) or [edit](/help/plans/insights.md#edit-plan) a plan. Examples of target metrics are revenue, conversion, CPA, or ROI. | June 18, 2025 | July 8, 2025 |
| **Spend pattern config** | When you build a plan, you now do have the option to use [historical reference](/help/plans/build.md) data (like past marketing spend data and insights) when defining the spend pattern for for each budget date range. | May 14, 2025 | May 14, 2025 |
| **Advanced plan configurations** | You can define [advanced configurations](/help/plans/build.md) for your plan, like average revenue per conversion and channel costs. | May 14, 2025 | May 14, 2025 | 

## March - April 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **Model drift detection** | When you open a model, you are [prompted to retrain the model when model drift is detected](/help/models/insights.md#model-drift). | April 3, 2025 | May 7, 2025 |
| **Marginal channel return in plan insights** | A [marginal channel return](/help/plans/insights.md#marginal-channel-return) visualization is added to Plan insights, which shows marginal break even and plan return for all or selected channels. | April 3, 2025 | April 24, 2025 | 


## January - February 2025

| Feature | Description | [Rollout start](#release-strategy) | [General Availability](#release-strategy) |
|---|---|---|---|
| **Nested conditions** | You can create nested conditions using AND and OR when you define an eligible data population as part of the [configuration of a model](/help/models/build.md#configure). | January 15, 2025 | February 18, 2025 |
| **View reports** | You can view a report on a [conversion](/help/harmonize-data/conversions.md#view-report) or a [marketing touchpoint](/help/harmonize-data/marketing-touchpoints.md#view-report) you have defined as part of harmonizing data. | January 15, 2025 | February 18, 2025 |
| **Delete confirmations** | You are prompted to confirm the deletion of a [plan](/help/plans/overview.md#delete-plans) or a [model](/help/models/overview.md#delete-models). | January 15, 2025 | February 18, 2025 |
| **Factors UI improvement** | You can select which [factors](/help/models/insights.md#factors-beta) you want to display in Model insights. | January 15, 2025 | February 18, 2025 |
| **Error handling** | User-friendly error messages and improved user experience for error scenarios in data harmonization and plans. | February 18, 2025 | February 18, 2025 |
| **Model status** | Redefinition of [model statuses](/help/models/overview.md#manage-models) across the model lifecycle. | February 18, 2025 | February 18, 2025 |


## Release strategy

[!UICONTROL Mix Modeler] uses feature flags (also known as "toggles") to control the visibility of new features, allowing for controlled scale testing prior to full release. This release strategy includes the following phases:

* **Limited Testing**: A phased release begins with testing by internal Adobe users. It is then made available to a small group of customer accounts to ensure that the feature meets customer needs and expectations. 

* **Start of Rollout**: Rollout of a phased release begins with the Limited Testing phase. The release is then scaled from 0% to 100% availability to customers over the course of a couple months. Phased rollout happens at the Experience Cloud Organization level, so all entitled users in an organization receive the same experience.
