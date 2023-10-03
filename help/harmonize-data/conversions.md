---
title: Conversions
description: Learn how to create conversions to use as part of harmonizing your data in Mix Modeler.
feature: Harmonized Data, Conversions
exl-id: a8559426-452a-43e8-9a60-0c0bc97d863c
---
# Conversions

Conversion events are business objectives that identify the impact of marketing activities. Examples: e-commerce orders, in-store purchases, website visits, and so forth.

You define marketing conversions for attribution analysis.

## Manage conversions

To see a table of the available conversions, in the Mix Modeler interface:

1. Select ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** from the left rail.
   
1. Select **[!UICONTROL Conversions]** from the top bar. You see a table of the conversions.

The table columns specify details about the conversion:

| Column name | Details |
| --- | ---|
| Name | The name of the conversion.  |
| Revenue | The harmonized data metric to use to calculate revenue from a conversion.  |
| Conversion metric | The harmonized data metric to use as the conversion metric for analysis. |
| Created | Date and time of the creation of the conversion. |
| Last modified | Date and time of the last modification of the conversion. |

{style="table-layout:auto"}

## Add a conversion

To add a conversion, in the ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Conversion]** interface in Mix Modeler:

1. Select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add a conversion]**.

1. In the **[!UICONTROL Create Conversion]** dialog:

    1. Enter a name for **[!UICONTROL Conversion]**, for example `Store Conversions`.
   
    1. Define the **[!UICONTROL Conversion category]**.

       1. Select a value from **[!UICONTROL *Select harmonize...*]**, for example `Conversion Type`.
   
       1. Select a value for the operator ![Chevron](../assets/icons/ChevronDown.svg), for example **[!UICONTROL is]**.

       1. Select a value from **[!UICONTROL *Select value*]** or enter a value, for example **[!UICONTROL Store]**.

    1. Select a harmonized field from **[!UICONTROL Conversion metric for analysis]**, for example **[!UICONTROL Orders]**.

    1. Select a harmonized field from **[!UICONTROL Revenue field]**, for example **[!UICONTROL Gross Demand]**.

    1. tT create the conversion, select **[!UICONTROL Create]**. To cancel the creation of a conversion, select **[!UICONTROL Cancel]**.

        ![Alt text](../assets/create-conversion.png)

1. When created, the conversion is added to the conversions table.
