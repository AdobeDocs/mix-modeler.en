---
title: Use scoring data
description: Learn how a model's scoring data in Mix Modeler is persisted.
feature: Models
exl-id: 2f2c3d20-7b14-41cc-a11a-03e8ad9e5d7a
---
# Use scoring data

As part of scoring a model, scoring data is persisted within a dataset in Experience Platform. When you have enabled muti-touch attribution during model creation, additional event score data are persisted within a dataset in Experience Platform.

Each of these datasets conforms to a schema. This article documents these schemas.


## Aggregate scoring data schema

The schema for scoring data is named like `AMM AI Schema - <name of model> <id>`. For example: `AMM AI Schema - Model for Online Conversion 10120`.

The dataset, persisting the scoring data for a model, is named like `AMM AI Aggregrate Scores - <id>`, for example `AMM AI Aggregrate Scores - 10120`.

The schema includes a field group with an object containing details about the scores. The object consists of the following fields.

| Field Name | Type | Definition |
|---|---|---|
| `campaignGroup` | String | Name of the campaign group. |
| `campaignName` | String | Name of the campaign. |
| `contribution` | Double | Contribution attributed to this conversion for the given touchpoint. |
| `conversionEndDate` | Date | End date of the conversion window. |
| `conversionName` | String | Name of the conversion that was created during the conversion definition setup step. |
| `conversionStartDate` | Date | Start date of the conversion window. |
| `geo` | String | The geographic location where the conversion has occurred.  |
| `mediaChannel` | String | Name of the channel that was used during the touchpoint setup step. |
| `mediaSubChannel` | String | Name of the subchannel. |
| `revenue` | Double | Revenue attributed to this conversion for the given touchpoint. |
| `scoreCreatedTime` | DateTime | Timestamp when this score record is created. |
| `touchpointEndDate` | Date | End date of the touchpoint window. |
| `touchpointName` | String | Name of the touchpoint that was created during the touchpoint definition setup step. Currently the touchpoint is defined on the media channel. |
| `touchpointStartDate` | Date | Start date of the touchpoint window. |


## Event scoring data schema

The schema for scoring data is named like `Attribution AI Scores - <name of model> <id> - Schema`. For example: `Attribution AI Scores - Model for Online Conversion 10120 - Schema`.

The dataset, persisting the scoring data for a model, is named like `Attribution AI Scores - <name of model> <id>`, for example `Attribution AI Scores - Model for Online Conversion 10120 `.

The schema includes a field group containing an object containing details about the cores. The object is named like `attibution_AI_scores__<name of model> id`.

The field group contains the following fields.

| Field Name | Type | Description |
|---|---|---|
| `conversion` | Object | Conversion metadata columns. |
| &nbsp;&nbsp;&nbsp;&nbsp;`passThrough` | Object |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`eventType` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`channel_typeAtSource` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`dataSource` | String | Globally unique identification of a data source. <br> **Example:** `Adobe Analytics`  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`eventSource` | String | The source when the actual event happened. <br> **Example:** `Adobe.com` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`eventType` | String | The primary event type for this time-series record. <br> **Example:** `Order` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`geo` | String | The geographic location where the conversion was delivered `placeContext.geo.countryCode`. <br> **Example:** `US` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`path` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`priceTotal` | Double | Revenue obtained through the conversion <br> **Example:** `99.9` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`product` | String | The XDM identifier of the product itself. <br> **Example:** `RX 1080 ti` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`productType` | String | The display name for the product as presented to the user for this product view. <br> **Example:** `Gpus` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`quantity` | Integer | Quantity purchased during the conversion. <br> **Example:** `1`  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`receivedTimeStamp` | DateTime | Received timestamp of the conversion. <br> **Example:** `2020-06-09T00:01:51.000Z` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`skuId` | String | Stock keeping unit (SKU), the unique identifier for a product defined by the vendor. <br> **Example:** `MJ-03-XS-Black` |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`timestamp` | DateTime | Timestamp of the conversion. <br> **Example:** `2020-06-09T00:01:51.000Z`  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`totalDaysToConversion` | Integer |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`totalTouchpointCount` | Integer | |
| `customerProfile` | Object | Identity details of the user used to build the model. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`identity` | Object | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`id` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`namespace` | String | Contains the details of the user used to build the model such as `id` and `namespace`. |
| `touchpointsDetail` | Object[] | The list of touchpoint details leading to the conversion, ordered by touchpoint occurrence or timestamp.  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`scores` | Object | Touchpoint contribution to this conversion as score.|
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`algorithmicInfluenced` | Double | Influenced score is the fraction of the conversion that each marketing touchpoint is responsible for. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`algorithmicSourced` | Double | Incremental score is the amount of marginal impact directly caused by a marketing touchpoint. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`decayUnits` | Double |  Rule-based attribution score where touchpoints closer to the conversion receive more credit than touchpoints that are farther away in time from the conversion. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`firstTouch` | Double  | Rule-based attribution score that assigns all credits to the initial touchpoint on a conversion path. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`lastTouch` | Double | Rule-based attribution score that assigns all credit to the touchpoint closest to the conversion. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`linear` | Double | Rule-based attribution score that assigns equal credit to each touchpoint on a conversion path.  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`uShape` | Double | Rule-based attribution score that assigns 40% of the credit to the first touchpoint and 40% of the credit to the last touchpoint. The other touchpoints splitting the remaining 20% equally. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`touchPoint` | Object | Touchpoint metadata. |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`passThrough` | Object | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`eventType` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`campaignGroup` | String |  |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`campaignName` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`campaignTag` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`eventId` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`geo` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`mediaAction` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`mediaChannel` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`receivedTimeStamp` | DateTime | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`timestamp` | DateTime | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`isFirstInThePosition` | Integer | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`lag` | Integer | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`position` | String | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`touchpointCountToConversion` | Integer | |
| &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`touchpointName` | String | Name of the touchpoint that was configured during setup. <br> **Example:** `PAID_SEARCH_CLICK` |
| `conversionName` | String | Name of the conversion that was configured during setup. <br> **Example:** `Order`, `Lead`, `Visit`  |
| `scoreCreatedTime` | DateTime | |
| `segmentation` | String | Conversion segment such as geo segmentation, which the model is built against. When segments are absent, `segmentation` is same as `conversionName`. <br> **Example:** `ORDER_US` |





See [Schemas](../ingest-data/schemas.md) for more information.
