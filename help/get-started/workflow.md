---
title: Mix Modeler workflow
description: Understand the typical workflow for Mix Modeler.
feature: Ingest Data, Plans, Harmonized Data, Models
exl-id: 200ff846-5d78-4b25-a425-bfd558b88c88
---
# Mix Modeler workflow

See this video for an introduction to the user workflow in Mix Modeler.

>[!VIDEO](https://video.tv.adobe.com/v/3424854/?learn=on)


A typical workflow in Mix Modeler consists of the following activities:

![Alt text](../assets/ApplicationWorkflow.svg)

|  | Activity | Description |
|---|---|---|
| ![Data](../assets/icons/Data.svg){width="100"} | [**Ingest data**](../ingest-data/overview.md) | Ingest event data from Experience Platform (for example Adobe Analytics, Web SDK, other sources), aggregated data from marketing channels (for example TV, walled gardens, email, owned and operated activities), external factors data from customers (for example price changes in subscription service) and internal factors data (for example holiday plans). |
| ![DataCheck](../assets/icons/DataCheck.svg){width="100"} | [**Harmonize data**](../harmonize-data/overview.md) | Configure mapping rules and conflict resolution rules to merge the various marketing datasets needed to measure and plan campaign performance in Mix Modeler. |
|  ![FileConfig](../assets/icons/FileGear.svg){width="100"} | [**Configure models**](../models/create.md) | Configure model instances with marketing touchpoints (for example channels), conversion definitions and internal and external factors. |
| ![FileData](../assets/icons/FileData.svg){width="100"}  | [**Train and score models**](../models/overview.md) | Create aggregate and event-level scores using machine-learning training and scoring.  |
| ![FileChart](../assets/icons/FileChart.svg){width="100"} | [**Create plans**](../plans/overview.md) |  Determine the best allocation of marketing funds to achieve a business objective by using the output of Mix Modeler's models. |
| ![Dashboard](../assets/icons/Dashboard.svg){width="100"} | [**Overview dashboard**](../dashboard/overview.md) | Get insights on harmonized data, models, and plans, using various configurable widgets. |

{style="table-layout:auto"}

The detailed data-oriented flowchart below illustrates how:

* harmonized data is based on:

  * experience event data (originating from Analytics source connector, collected through Experience Platform SDKs and APIs, ingested through source connectors, or using streaming ingestion),
  * aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources, or offline advertising data, and 
  * definitions of harmonized fields and dataset rules.

* a model is based on:

  * the conversion and marketing touchpoint definitions resulting from the harmonized data and 
  * non-marketing aggregate or summary data containing internal or external factors.

* mult-touch attribution event scores can potentially be fed back into Experience Platform data lake for use in subsequent model configuration, training and scoring.

![Comprehensive workflow](../assets/comprehensive-workflow.svg)
