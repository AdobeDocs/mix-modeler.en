---
title: Harmonize data
description: Learn how to harmonize data in Mix Modeler.
feature: Harmonized Data
exl-id: 6cb70762-e3b2-46a0-b028-1d6daf3edae5
---
# Harmonize data

The data in Mix Modeler is of different nature depending on the source of data. The data can be:

* aggregate or summary data, for example collected from walled garden data sources or offline advertising data gathered (like spend) from running a billboard campaign, an event, or a physical ad campaign,
* event data, for example from first party data sources. This event data can be data collected through the Adobe Analytics source connector from Adobe Analytics, or through the Experience Platform Web or Mobile SDK or Edge Network API, or data ingested using source connectors.

The harmonization service of Mix Modeler assimilates the aggregate and event data into a consistent data view. This data view, combined with internal and external factors data, is the source for the models in Mix Modeler. The service uses the highest granularity across the different datasets. For example, if one dataset has a granularity of monthly and remaining datasets do have weekly and daily granularity, the harmonization service creates a data view using monthly granularity.

## An example of harmonized data

Imagine you have the following datasets available for Mix Modeler.

**Dataset 1**
 
Contains marketing effort dataset from YouTube, with a granularity of the aggregate data set to daily.

|Date|Date Type|Channel|Campaign|Brand|Geo|Clicks|Spend|
|---|:--:|---|---|---|---|---:|---:|
|12-31-2021|day|YouTube|Y_Fall_02|BrandX|US|10000|100|
|01-01-2022|day|YouTube|Y_Fall_02|BrandX|US|1000|10|
|01-03-2022|day|YouTube|Y_Fall_01|BrandY|CA|10000|100|
|01-04-2022|day|YouTube|Y_Summer_01|Null|CA|9000|80|

{style="table-layout:auto"}


**Dataset 2** 

Contains marketing effort dataset from Facebook, with a granularity of the aggregate data set to weekly.

|Date|Date Type|Channel|Campaign|Geo|Clicks|Spend|
|--- |:---:|--- |---|---|---:|---:|
|01-01-2022|week|Facebook|FB_Fall_01|US|8000|100|
|01-08-2022|week|Facebook|FB_Fall_02|US|1000|10|
|01-08-2022|week|Facebook|FB_Fall_01|US|7000|100|
|01-16-2022|week|Facebook|FB_Summer_01|CA|10000|80|

{style="table-layout:auto"}


**Dataset 3** 

A conversion dataset, with a granularity of the aggregate data set to daily.

|Date|Date Type|Geo|Goal|Revenue|
|--- |:---: |---|---|---:|
|01-01-2022|day|US|Fashion|200|
|01-08-2022|day|US|Fashion|10|
|01-08-2022|day|US|Jewelry|1100|
|01-16-2022|day|CA|Jewelry|80|

{style="table-layout:auto"}


**Dataset 4** 

A sample experience event dataset (Web SDK events) from the customer.

|Timestamp|Identity Namespace|Identity Id|Channel|Clicks|
|--- |--- |--- |--- |---:|
|01-01-2022 00:01:01.000|ECID|64fd46ff-8c63-43b4-85a7-92b953113ba0|CSE|1|
|01-01-2022 00:01:01.000|ECID|64fd46ff-8c63-43b4-85a7-92b953113ba0|CSE|1|
|01-08-2022 00:01:01.000|ECID|2ca2a16e-caf0-4fa9-9a8b-9774b39547c4|CSE|1|
|01-08-2022 00:01:01.000|ECID|5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc|CSE|1|

{style="table-layout:auto"}


You want to build a harmonized dataset, with a granularity set to weekly. The event data is aggregated to week granularity and added to the harmonized dataset. The result is:

**Harmonized dataset**

|Date|Date Type|Channel|Campaign|Brand|Geo|Goal|Clicks|Spend|Revenue|
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
|12-27-2021|week|YouTube|Y_Fall_02|BrandX|US|Null|11000|110|Null|
|01-03-2022|week|YouTube|Y_Fall_01|BrandY|CA|Null|10000|100|Null|
|01-03-2022|week|YouTube|Y_Summer_01|Null|CA|Null|9000|80|Null|
|01-01-2022|week|Facebook|FB_Fall_01|Null|US|Null|8000|100|Null|
|01-08-2022|week|Facebook|FB_Fall_02|Null|US|Null|1000|10|Null|
|01-08-2022|week|Facebook|FB_Fall_01|Null|US|Null|7000|100|Null|
|01-16-2022|week|Facebook|FB_Summer_01|Null|CA|Null|10000|80|Null|
|12-27-2021|week|Null|Null|Null|US|Fashion|Null|Null|200|
|01-03-2022|week|Null|Null|Null|US|Fashion|Null|Null|10|
|01-03-2022|week|Null|Null|Null|US|Jewelry|Null|Null|1100|
|01-10-2022|week|Null|Null|Null|CA|Jewelry|Null|Null|80|
|01-01-2022|week|CSE|Null|Null|Null|Null|2|Null|Null|
|01-08-2022|week|CSE|Null|Null|Null|Null|2|Null|Null|

{style="table-layout:auto"}


## Setup harmonized data

To build a harmonized dataset, like in the simplified [example](#an-example-of-harmonized-data), you must follow these steps:

1. Define additional [harmonized fields](fields.md) that you want to use beyond the global harmonized fields already available.
1. Set up [dataset rules](dataset-rules.md) to map fields from your aggregate or experience event datasets to harmonized fields.
1. Define [marketing touchpoints](marketing-touchpoints.md) using the standard and additional harmonized fields that you defined.
1. Define [conversions](conversions.md) using the standard and additional harmonized fields that you defined.
   

## View harmonized data

To see your harmonized data, in the Mix Modeler interface:

1. Select ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized datasets]** from the left rail.
   
1. Select **[!UICONTROL Harmonized Data]** from the top bar. Aa recap of your harmonized data is shown based on the fields, dataset rules, marketing touchpoints and conversions you have defined.

    1. To redefine the period on which the recap of harmonized data is based, enter a date range for **[!UICONTROL Date range]** or use ![Calendar](../assets/icons/Calendar.svg) to select a data range.

    1. To modify the harmonized field columns displayed for the Harmonized data table, use ![Settings](../assets/icons/Setting.svg) to open the **[!UICONTROL Column settings]** dialog.

       1. Select ![SelectBox](../assets/icons/SelectBox.svg) one or more columns from **[!UICONTROL AVAILABLE COLUMNS]** and use ![Chevron right](../assets/icons/ChevronRight.svg) to add these columns to **[!UICONTROL SELECTED COLUMNS]**. 

       1. Select ![SelectBox](../assets/icons/SelectBox.svg) one or more columns from **[!UICONTROL SELECTED COLUMNS]** and use ![Chevron left](../assets/icons/ChevronLeft.svg) to remove the selected columns and return these columns back to **[!UICONTROL AVAILABLE COLUMNS]**.

       1. Select a column from **[!UICONTROL DEFAULT SORT]** and toggle between **[!UICONTROL Ascending]** or **[!UICONTROL Descending]**.

       1. To change the order of columns displayed, you can move a column in **[!UICONTROL SELECTED COLUMNS]** up and down through drag and drop .

    1. Select **[!UICONTROL Submit]** to submit your column setting changes. Select **[!UICONTROL Close]** to cancel any changes you made.

1. If more pages are available, use ![Arrow left](../assets/icons/ChevronLeft.svg) or ![Arrow Right](../assets/icons/ChevronRight.svg) at **[!UICONTROL Page _x_ of _x_]** to move between pages.
