---
title: Marketing touchpoints
description: Learn how to create marketing touchpoints to use as part of harmonizing your data in Mix Modeler.
feature: Harmonized Data, Marketing Touch Points
exl-id: 42851107-7568-4bc9-92ca-3cba713a522e
---
# Marketing touchpoints {#marketing-touchpoints}

>[!CONTEXTUALHELP]
>id="harmonizeddata_marketingtouchpoints_create"
>title="Marketing touchpoints"
>abstract="Marketing touchpoints are recipient, individual, and or cookie-level marketing events used to evaluate the impact of marketing investments on numeric or revenue-based conversions." 


Marketing touchpoints are recipient, individual, and or cookie-level marketing events used to evaluate the impact of marketing investments on numeric or revenue-based conversions.

You define marketing touchpoints to assist you in attribution analysis.

## Manage marketing touchpoints

To see a table of the available marketing touchpoints in the Mix Modeler interface:

1. Select ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** from the left rail.
   
1. Select **[!UICONTROL Marketing touchpoint]** from the top bar. You see a table of the marketing touchpoints. If more pages are available, use ![Arrow left](/help/assets/icons/ChevronLeft.svg) or ![Arrow Right](/help/assets/icons/ChevronRight.svg) at **[!UICONTROL Page _x_ of _x_]** to move between pages of the table.

The table columns specify details about the marketing touchpoint:

| Column name | Details |
| --- | ---|
| Name | The name of the marketing touchpoint.  |
| Spend metric | The harmonized data metric to use to calculate touchpoint spend.  |
| Volume metric | The harmonized data metric to use to calculate touchpoint volume. |
| Rule | The touchpoint rule to use. |
| Created | Date and time of the creation of the marketing touchpoint. |
| Last modified | Date and time of the last modification of the marketing touchpoint. |


## Add a marketing touchpoint

To add a marketing touchpoint, in the ![DataSearch](/help/assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Marketing touchpoint]** interface in Mix Modeler:

1. Select ![Add](/help/assets/icons/AddCircle.svg) Add marketing touchpoint.

1. In the **[!UICONTROL Marketing touchpoint]** dialog.

    1. Enter a name for **[!UICONTROL Touchpoint Name]**, for example `Luma Touchpoint`.

    1. Define a **[!UICONTROL Touchpoint rule]**.

       1. Select a value from **[!UICONTROL *Select harmonized*]**, for example **[!UICONTROL Brand]**.

       1. Select a value for operator ![Chevron](/help/assets/icons/ChevronDown.svg), for example **[!UICONTROL is]**.

       1. Select a value from **[!UICONTROL *Select value*]** or enter a value, for example **[!DNL Luma]**.

    1. Select a harmonized field from **[!UICONTROL Touchpoint volume]**, for example **[!UICONTROL Impressions]**.

    1. Select a harmonized field from **[!UICONTROL Touchpoint spend]**, for example **[!UICONTROL Cost]**.
   
       ![Marketing touchpoint](/help/assets/create-touchpoint.png)

    1. To create the marketing touchpoint, select **[!UICONTROL Create]**. To cancel the creation of a marketing touchpoint, select **[!UICONTROL Cancel]** .

1. When created, the touchpoint is added to the marketing touchpoints table.


## View details

To view details of a marketing touchpoint:

1. Select ![More](/help/assets/icons/More.svg) when hovering over a marketing touchpoint name in the table.

1. Select ![View](/help/assets/icons/ViewDetail.svg) **View**. A dialog shows details of the marketing touchpoint. See [Add a marketing touchpoint](#add-a-marketing-touchpoint) for more information. Select **[!UICONTROL Cancel]** to close the dialog.


## View report

To view a report of a marketing touchpoint:

1. Select ![More](/help/assets/icons/More.svg) when hovering over a marketing touchpoint name in the table.

1. Select ![GraphTrend](/help/assets/icons/GraphTrend.svg) **View report**. A dialog shows a report of the marketing touchpoint.

   ![Marketing touchpoint view report](../assets/marketingtouchpoint-view-report.png)

   * To change the granularity to report on, select a value from the **[!UICONTROL Weekly]** dropdown menu.
   * To change the period to report on, enter a start and end date or use ![Calendar](/help/assets/icons/Calendar.svg) to define a period in the calendar popup.

1. Select **[!UICONTROL Close]** to close the dialog.

## Delete a marketing touchpoint

To delete a marketing touchpoint:

1. Select ![Delete](/help/assets/icons/Delete.svg) **Delete** when hovering over a marketing touchpoint name in the table. 
1. In the **[!UICONTROL Delete touchpoint]** dialog confirmation dialog select **[!UICONTROL Delete]** to permanently delete the marketing touchpoint.

