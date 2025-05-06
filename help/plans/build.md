---
title: Build plans
description: Learn how to build plans in Mix Modeler.
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
---

# Build plans

In Mix Modeler, you create a plan using the plan canvas. In the plan canvas, you can set up the details and budgets of your plan and the underlying model to use for your plan. Once you have specified details, budget and model you can go ahead with an AI-recommended plan or edit the spend by channel.

To create a plan, in the ![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** interface in Mix Modeler, select **[!UICONTROL Create plan]**.

1. In the **[!UICONTROL Plan creation]** screen:

    1. In the **[!UICONTROL Setup]** section:

        1. Enter a **[!UICONTROL Plan name]**, for example `Demo plan`. Enter a **[!UICONTROL Description]**, for example `Demo plan for Luma company`.
        1. Select a **[!UICONTROL Model]** from **[!UICONTROL _Select an option.._.]**
        1. You can select ![LinkOut](/help/assets/icons/LinkOut.svg) **[!UICONTROL Create model]** to create a model directly from within the plan creation. This will open a new tab in your browser and show the [Models](../models/overview.md) interface.

           ![Plan Setup](/help/assets/plan-setup.png)

    1. In the **[!UICONTROL Budget]** section:

        1. Specify a date range, either by typing dates or selecting a date range using ![Calendar](/help/assets/icons/Calendar.svg).
        1. Enter a budget.
        
       To add additional date ranges, each with their budget, select ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**.
        
       To delete a date range and associated budget, select ![Close](/help/assets/icons/Close.svg).

       To define a specified maximum budget:
       
       1. Switch **[!UICONTROL Maximize budget]** on.
       1. Specify the amount of maximum budget. The amount should be equal or higher than the total amount of budgets specified for the date ranges.

          ![Plan budget](/help/assets/plan-budget.png)

    1. Select **[!UICONTROL Next]**.

1. In the **[!UICONTROL Done with all required fields]** dialog:

    ![Plan Done](/help/assets/plan-done-required-fields.png)

    * Select ![NewPlan](../assets/icons/NewPlan.svg) **[!UICONTROL Create plan now]** if you want to generate an AI recommended plan with forecasted ROI.

      Select **[!UICONTROL OK]**. Your plan is created.


    * Select ![TableEdit](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]** if you want to edit channel budget before creating a plan with forecasted ROI.

      Select **[!UICONTROL OK]**, so you can define your channel spend in **[!UICONTROL Spend selection]** in the next step.

    

1. In the **[!UICONTROL Spend selection]** section, for each budget date range, use the ![Chevron](/help/assets/icons/ChevronRight.svg) top open the channel distribution view for that data range.

    1. To define budgets for each channel, enter a value for **[!UICONTROL Min]** and **[!UICONTROL Max]** or use the sliders.

    1. To toggle between currency or percentage input, select **[!UICONTROL $]** or **[!UICONTROL %]** for **[!UICONTROL View spend by]**.

       ![Spend selection](/help/assets/plan-spend-selection.png)

    1. When finished, select **[!UICONTROL Create]**. 

    1. In the **[!UICONTROL Create plan]** dialog, select **[!UICONTROL Create plan]** to create your plan. Select **[!UICONTROL Cancel]** to cancel the creation of your plan. A **[!UICONTROL No work is saved]** dialog is shown to confirm.

1. In the Advanced configurations section, you c