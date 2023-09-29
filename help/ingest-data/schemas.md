---
title: Schemas
description: Learn how to manage the schemas required to ingest data into Adobe Mix Modeler.
feature: Schemas
---

# Schemas

To manage schemas, supporting the data you want to ingest in Adobe Experience Platform and use in Adobe Mix Modeler:

1. Go to the Adobe Mix Modeler interface.

1. Select ![Schemas](../assets/icons/Schemas.svg) **[!UICONTROL Schemas]**, underneath **[!UICONTROL DATA MANAGEMENT]**. 

See the [Schemas UI overview](https://experienceleague.adobe.com/docs/experience-platform/xdm/ui/overview.html?lang=en) for more information.

## Aggregate or summary data

It is highly recommended to use the XDM Summary Metrics class as the base of the schema underlying any aggregate or summary data you want to ingest in Experience Platform and use in Adobe Mix Modeler.

See below for an example of a **[!DNL LumaPaidMarketingSchema]** using the XDM Summary Metrics as the base class and dedicated field groups (annotated with colors) for metric (**[!DNL AMMMetrics]**), dimensions (**[!DNL AMMDimensions]**) and other customer specific information (**[!DNL CustomerSpecific]**). 

![Summary Schema](../assets/summary-schema.png)

To define a set of audit properties, it is strongly encouraged to use the External Source System Audit Details fieldgroup, as part of a schema used for collecting aggregate or summary data from external sources.
