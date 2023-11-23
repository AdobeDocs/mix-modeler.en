---
title: Scoring data
description: Learn how a model's scoring data in Mix Modeler is persisted.
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
---
# Scoring data

As part of scoring a model, scoring data is persisted within a dataset in Experience Platform. This dataset is conforming to a schema created for each model in your Mix Modeler instance.

The schema for scoring data is named like `AMM AI Schema - <name of model> <id>`. For example: `AMM AI Schema - Model for Online Conversion 10120`.

The dataset, persisting the scoring data for a model, is named like `AMM AI Aggregrate Scores - <id>`, for example `AMM AI Aggregrate Scores - 10120`.


## Schema

The schema includes a field group with an object containing details about the scores. The object consists of the following fields.

| Field Name | Type | Definition | 
|---|---|---|
| **campaignGroup** | String | Name of the campaign group. | 
| **campaignName** | String | Name of the campaign. | 
| **contribution** | Double | Contribution attributed to this conversion for the given touchpoint. |
| **conversionEndDate** | Date | End date of the conversion window. |  
| **conversionName** | String | Name of the conversion that was created during the conversion definition setup step. |  
| **conversionStartDate** | Date | Start date of the conversion window. | 
| **geo** | String | The geographic location where the conversion has occurred.  | 
| **mediaChannel** | String | Name of the channel that was used during the touchpoint setup step. |  
| **mediaSubChannel** | String | Name of the subchannel. | 
| **revenue** | Double | Revenue attributed to this conversion for the given touchpoint. |  
| **scoreCreatedTime** | DateTime | Time when this score record is created. | 
| **touchpointEndDate** | Date | End date of the touchpoint window. | 
| **touchpointName** | String | Name of the touchpoint that was created during the touchpoint definition setup step. Currently the touchpoint is defined on the media channel. | 
| **touchpointStartDate** | Date | Start date of the touchpoint window. |
