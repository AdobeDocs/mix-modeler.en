---
title: Mix Modeler overview
description: Get an overview of the functionality and capabilities of Mix Modeler.
short-description: Get an overview of the functionality and capabilities of Mix Modeler.
feature: Plans, Harmonized Data, Models
exl-id: aa1018d5-b073-4dfb-b40c-ca16a8970b2f
TQID: https://experienceleague.adobe.com/66NcfgGeMriaUXgpJ-h2MV2PBISSE5GMz3WWuF-i2u4
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Mix Modeler
feature_v2:
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
subfeature_v2:
  - id: a9505d76-24a1-4ffe-bd01-6ac32d5af453
    internal-label: Model insights
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: c2be0313-b3ae-45e0-b454-d20bf54b23f2
    internal-label: Measurement
  - id: cdd65e7e-8839-44a2-bc21-0e03623b5dd1
    internal-label: Optimization
  - id: d00e9f03-e50b-4162-b143-0c0817c937c2
    internal-label: Customer journeys
  - id: e1e0219c-f879-479f-8427-888ed2a6e9c2
    internal-label: Insights
  - id: eb30f47f-d87a-400f-8f78-63ce7979ff56
    internal-label: Machine learning
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# Mix Modeler overview

Mix Modeler, powered by Adobe Sensei, enables marketers to measure campaigns and optimize planning holistically across all channels: paid, earned, and owned. Its unified methodology measures incrementally at both marketing touchpoints and aggregate levels, while ensuring fully consistent results.

Mix Modeler provides the incremental impact of all marketing activities on business and campaign outcomes through a holistic (end-to-end) measurement application for digital and offline marketing. 

Mix Modeler provides the following types of optimized and actionable insights at a strategic and tactical level, so you can better understand:

* marketing spend and resulting performance across various channels, and
* recommended investment levels to achieve future business objectives.


To accomplish this functionality, Mix Modeler combines: 

* bottoms-up (event-level) data and top-down (aggregate-level) data,
* external market factors and internal factors, and
* predictive and transfer machine-learning methodologies.

The AI/ML bi-directional transfer learning unifies marketing mix modeling (MMM) and multi-touch attribution (MTA) results to ensure consistent results across measurement and planning in a cookie-less world. 

![Bidirectional transfer learning](/help/assets/birdirectional-transfer-learning.png){width="500" align="center"}


## Capabilities

Mix Modeler offers the following capabilities:

| Capability | Description |
|---|---|
| **Measure incremental performance** | Understand the incremental ROI and impact of marketing across business goals or tactical campaign goals. |
| **Unify results across MMM and MTA** | Make more confident decisions through the unification of marketing mix modeling (MMM) and multi-touch attribution (MTA) models via transfer learning. |
| **Optimally allocate budgets** | Identify optimal budget allocation based on marketing spend and impact to goals. |
| **Create & compare budget scenarios** | Develop multiple budget plans and compare their impact to make optimal decisions for your business. |

{style="table-layout:auto"}

>[!MORELIKETHIS]
>
>[Understand the Mix Modeler workflow](workflow.md)


### Marketing Mix Modeling (MMM)

Marketing mix modeling in Mix Modeler is a privacy-friendly machine learning analysis used to measure the incremental impact of various marketing tactics and business factors on conversion metrics. It helps businesses and marketers to understand

* the effectiveness of their marketing strategies, 
* the effects of business factors on customer behavior, and 
* what drives ROI and conversions. 
  
This comprehensive analysis empowers businesses to allocate marketing budgets strategically across various business lines, regions, channels, and campaigns while also providing predictive insights into the business impact of future events.

Mix Modeler's marketing mix modeling capabilities are foundational to solving the following use cases:

* Executive reporting: Allow executives to understand the true incremental impact of marketing, both as a whole and by channel, region, SKU, etc.
* Strategic planning: Inform long-term marketing strategies and set realistic goals and benchmarks for future campaigns
* Comprehensive measurement: Holistic analysis of how different marketing and business factors interact and contribute to overall sales and performance
* Scenario analysis: Allow businesses to simulate different marketing scenarios and strategies and predict their outcomes


### Multi-Touch Attribution (MTA)

The multi-touch attribution in Mix Modeler is an optional machine learning analysis that you can leverage to attribute credits to event-level touchpoints leading to conversion events. This attribution is used by marketers to help quantify the marketing impact of each individual marketing touchpoint across customer journeys that are trackable. These digital marketing campaign touchpoints typically are display ad clicks, email sends, email opens, and paid search clicks. Multi-touch attribution cannot measure most offline touchpoints such as print ads, billboards, or TV commercials and business factors. These touchpoints only have summary level data that cannot be stitched to customer journeys. 

Mix Modeler's multi-touch attribution supports two categories of scores:

* Algorithmic scores, which include incremental and influenced scores:
  * The influenced score is the fraction of the conversion that each marketing touchpoint is responsible for.
  * The incremental score is the amount of marginal impact directly caused by a marketing touchpoint. This score removes the baseline (the portion of conversion attained without any marketing activities) from the influenced score.
    
* Rule-based scores, which include First touch, Last touch, Linear, U-shaped, and Time-Decay.

You can use the multi-touch attribution capability of Mix Modeler in the following use cases:

* Campaign budget allocation: Inform budget allocation decisions across marketing channel.
* Campaign optimization: Within each channel, understand which campaigns, creatives, and keywords are working better for which SKUs or Geos. This understanding allows you to look at each channel so the marketing team can optimize their tactics.
* Full-funnel event-level attribution: Understand marketing's impact across the entire customer journey. For example, free account signup to paid conversion and beyond.
* Partner evaluations: Evaluate the effectiveness of agencies and partners, based on attribution results.

See [Model Insights - Attribution](../models/insights.md#attribution) on how to access the multi-touch attribution insights within Mix Modeler.


