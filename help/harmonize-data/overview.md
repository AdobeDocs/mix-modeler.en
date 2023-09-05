---
title: Harmonize data
description: Learn how to harmonize data in Adobe Mix Modeler.
---

# Harmonize data

The data in Adobe Mix Modeler is of different nature depending on the source of data. The data can be:

* aggregated data, for example collected from walled garden data sources,
* even data, for example from first party data sources, like Adobe Analytics, through the Adobe Experience Platform Web or Mobile SDK, Edge Network API or source connectors.

The harmonization service of Adobe Mix Modeler assimilates the aggregate and event data into a consisent data view. This data view is the source for the plans and models in Adobe Mix Modeler.

## Example

Imagine you have the following datasets available for Adobe Mix Modeler.

**Dataset 1**

* Marketing effort dataset from Youtube. 
* Granularity of the aggregate data: day.

|Date|Date Type|Channel|Campaign|Brand|Geo|Clicks|Spend|
|---|:--:|---|---|---|---|---:|---:|
|12-31-2021|day|Youtube|Y_Fall_02|BrandX|US|10000|100|
|01-01-2022|day|Youtube|Y_Fall_02|BrandX|US|1000|10|
|01-03-2022|day|Youtube|Y_Fall_01|BrandY|CA|10000|100|
|01-04-2022|day|Youtube|Y_Summer_01|Null|CA|9000|80|

{style="table-layout:auto"}


**Dataset 2**

* Marketing effort dataset from Facebook
*Granularity of the aggregate data: week

|Date|Date Type|Channel|Campaign|Geo|Clicks|Spend|
|--- |:---:|--- |---|---|---:|---:|
|01-01-2022|week|Facebook|FB_Fall_01|US|8000|100|
|01-08-2022|week|Facebook|FB_Fall_02|US|1000|10|
|01-08-2022|week|Facebook|FB_Fall_01|US|7000|100|
|01-16-2022|week|Facebook|FB_Summer_01|CA|10000|80|

{style="table-layout:auto"}


**Dataset 3**

* Conversion dataset
* Granularity of the aggregate data - day

|Date|Date Type|Geo|Goal|Revenue|
|--- |:---: |---|---|---:|
|01-01-2022|day|US|Fashion|200|
|01-08-2022|day|US|Fashion|10|
|01-08-2022|day|US|Jewelry|1100|
|01-16-2022|day|CA|Jewelry|80|

{style="table-layout:auto"}


**Dataset 4**

* A sample experience event dataset (Web SDK events) from the customer.

|Timestamp|Identity Namespace|Identity Id|Channel|Clicks|
|--- |--- |--- |--- |---:|
|01-01-2022 00:01:01.000|ECID|64fd46ff-8c63-43b4-85a7-92b953113ba0|CSE|1|
|01-01-2022 00:01:01.000|ECID|64fd46ff-8c63-43b4-85a7-92b953113ba0|CSE|1|
|01-08-2022 00:01:01.000|ECID|2ca2a16e-caf0-4fa9-9a8b-9774b39547c4|CSE|1|
|01-08-2022 00:01:01.000|ECID|5ce99bfb-e44a-40d9-b8cd-c5408bda7cdc|CSE|1|

{style="table-layout:auto"}


**Harmonized data view**

* The harmonized view with granularity of week.
* The event data is aggregated to week granularity and added to the harmonized view.

|Date|Date Type|Channel|Campaign|Brand|Geo|Goal|Clicks|Spend|Revenue|
|--- |:---:|--- |--- |--- |---|---|---:|---:|---:|
|12-27-2021|week|Youtube|Y_Fall_02|BrandX|US|Null|11000|110|Null|
|01-03-2022|week|Youtube|Y_Fall_01|BrandY|CA|Null|10000|100|Null|
|01-03-2022|week|Youtube|Y_Summer_01|Null|CA|Null|9000|80|Null|
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


The steps to setup your harmonized data view are:

1. Define additional fields you want to use beyond the default fields already available.
1. Set up dataset rules to map fields from your aggregate or experience event datasets to harmonized fields.
1. Define Marketing touchpoints using the standard and additional harmonized fields you defined.
1. Define Conversions using the standard and additional harmonized fields you defined.
   
