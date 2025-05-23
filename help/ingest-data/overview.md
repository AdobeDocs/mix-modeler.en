---
title: Ingest data overview
description: Learn how to ingest data into Mix Modeler.
feature: Datasets, Event Datasets, Summary Datasets, Aggregate Datasets
exl-id: dc16a601-bbd9-467b-8a7e-c32654d4069a
---
# Ingest data overview

Mix Modeler works with event level data, aggregate or summary marketing effort data from various walled gardens, and aggregrate or summary data from any other source, like offline advertising, internal factors or external factors. 

Customers can use any kind of data that is ingested into Experience Platform as datasets and which is based on schemas using the XDM ExperienceEvent or XDM Summary Metrics as the base class. 

For example:

* data collected using the Adobe Analytics source connector and transformed into datasets conforming to the default or a custom version of the Adobe Analytics schema, or alternatively,
* data collected using the Experience Platform Web SDK, Mobile SDK, or Edge Network Server API for collecting customer interactions on web, mobile, or any other type of device,
* aggregate or summary data from walled gardens (like Facebook, YouTube), traffic sources or offline advertising data,
* non-marketing aggregate or summary data containing internal or external factors that are useful for model building.

You can use any kind of mechanism, supported by Experience Platform, to ingest your experience event-level, aggregate marketing effort data, and data from other sources. Ingestion mechanisms include the Experience Platform SDKs, APIs, source connectors, streaming and batch ingestion. To learn more about ingesting your data in Experience Platform for use in Adobe Mix Modeler, see [Data Ingestion overview](https://experienceleague.adobe.com/en/docs/experience-platform/ingestion/home).

## Guidelines

To ingest data into Experience Platform for use with Mix Modeler, follow these guidelines:

* There should not be any overlap in the incremental data that is added to the datasets.
* All data from a single source should be of the same granularity.
* Date and granularity are mandatory fields in the underlying schema for all aggregate data ingested as datasets
* Channel is a mandatory field in the underlying schema for all marketing effort / spend data ingested as datasets.


## Examples

Find below some examples of data typically used in Mix Modeler beyond the more standard experience event data.

+++ Aggregate marketing effort data

| Geo | Date | Date Type | Channel | Campaign | Click | Earned | Engagement | Impression | Open | Owned | Sent | Spend |
|---|:--|---|:---:|---|--:|---|--:|---|---|---|--:|--:|
|AMER|2021-10-31|day|EMAIL| |12752| | | | | |1132945| |
|AMER|2021-10-31|day|FB| |148844| | | | | | | 42111 | 
|AMER|2021-10-31|day|YT| | | |2314452| | | | | 10540 |
|JPN|2021-10-21|day|EMAIL| |21089| | | | | |3283626| |
|JPN|2021-10-21|day|SOCIAL| | | |621| | | | | 74512 |

{style="table-layout:auto"}

+++

+++ Aggregate conversion data

| Geo | Date | Date Type | Product | Units Sold | Revenue |
|---|:---|:---:|---|--:|--:|
|EMEA|2021-09-13|day|Creator Economy|603|36537.68|
|EMEA|2021-09-13|day|Metaverse|55|21704.37|
|JPN|2022-05-30|day|Pro Imaging| 487|64469.60|
|JPN|2022-05-30|day|Document Cloud|642|100509.07|

{style="table-layout:auto"}

+++

+++ External factors data

| Data | Date Type | Factor | Value |
|---|:---:|:---:|:---|
|2020-08-02|week|SPX|3325.866|
|2020-08-09|week|SPX|3364.158|
|2020-08-16|week|SPX|3385.858|
|2020-08-23|week|SPX|3497.965|

{style="table-layout:auto"}

+++

To work with data in Mix Modeler, you need data collected in datasets and modeled after schemas in Experience Platform. The Mix Modeler interface provides easy access to both the Experience Platform Schemas and Datasets UI.


## Validate

To validate whether your data is properly available in Mix Modeler, you can do the following:

* Use visualizations in  [Overview](/help/overview.md).
* Download and inspect data from [Harmonized data](/help/harmonize-data/overview.md) in Harmonized datasets.

To validate whether your data is ingested properly in Experience Platform, you can [write and execute SQL queries using Experience Platform Query Service](https://experienceleague.adobe.com/en/docs/experience-platform/query/home).


>[!MORELIKETHIS]
>
>See for more details on how to manage schemas and datasets:
>
>* [Schemas](schemas.md)
>* [Datasets](datasets.md)
