---
title: Schemas
description: Learn how to manage the schemas required to ingest data into Mix Modeler.
feature: Schemas
---

# Schemas

To manage schemas, supporting the data you want to ingest in Experience Platform and use in Mix Modeler:

1. Go to the Mix Modeler interface.

1. Select ![Schemas](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, underneath **[!UICONTROL DATA MANAGEMENT]**. 

See the [Schemas UI overview](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) for more information.

## Aggregate or summary data

It is highly recommended to use the XDM Summary Metrics class as the base of the schema underlying any aggregate or summary data you want to ingest in Experience Platform and use in Mix Modeler.

Use the XDM Summary Metrics class for:

- walled garden data, for example data from Facebook or YouTube.

- external factors data, like data from SPX (S&P 500 stock price indices), weather data,

- internal factors data, for example price changes, a holiday calendar.

>[!IMPORTANT]
>
>The schema definition must contain at least one numeric field (using Integer, Double, Boolean, or other numeric type) to support the required metrics for the ingested data.

A schema using the **[!DNL XDM Summary Metrics]** base class can be simple, as shown in the **[!DNL ExternalFactorSummarySchema]** below.

![External Factors Schema](../assets/external-factors-schema.png)

This simple schema can be used to ingest datasets containing data for, for example:

- Competitor index data

  | timestamp | date_type | factor | value |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000Z | week | competitor_index | 289.8 |
  | 2020-12-05T00:00:00.000Z | week | competitor_index | 291.2 |
  | 2020-12-12T00:00:00.000Z | week | competitor_index | 280.07 |
  | ... | ... | ... | ... |
 
- Public holiday data

  | timestamp | date_type | factor | value |
  |---|---|---|--:|
  | 2020-11-28T00:00:00.000Z | week | all_holidays_flag | 0.0 |
  | 2020-12-05T00:00:00.000Z | week | all_holidays_flag | 0.0 |
  | 2020-12-12T00:00:00.000Z | week | all_holidays_flag | 0.0 |
  | 2020-12-19T00:00:00.000Z | week | all_holidays_flag | 0.0 |
  | 2020-12-26T00:00:00.000Z | week | all_holidays_flag | 1.0 |
  | ... | ... | ... | ... |


See below for a more comprehensive example of a **[!DNL LumaPaidMarketingSchema]** using the **[!DNL XDM Summary Metrics]** as the base class. The schema uses dedicated field groups (annotated with colors) for metrics (**[!DNL AMMMetrics]**), dimensions (**[!DNL AMMDimensions]**), and other customer-specific information (**[!DNL CustomerSpecific]**). 

![Summary Schema](../assets/summary-schema.png)

Given the asynchronous nature of profile ingestion, when collecting aggregate or summary data from external sources, it is encouraged to use the External Source System Audit Details field group as part of a schema. This field group defines a set of audit properties for external sources.
