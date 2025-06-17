---
title: Build plans
description: Learn how to build plans in Mix Modeler.
feature: Plans
exl-id: 6d61d0b2-5871-4d00-9a35-73fff0a1c3e5
---

# Build plans

In Mix Modeler, you create a plan using the plan wizard. In the plan wizard, you can set up the details and budgets or target metrics of your plan and the underlying model to use for your plan. Once you have specified details, budget, target metrics, and model you can go ahead with an AI-recommended plan or edit the spend by channel. You have the option to define advanced configurations on average revenue per conversion and channel costs. 

You need to define the goal you want to maximize your plan against. This goal can either be a budget that you can spend or a target you want to achieve. If the goal is a target, you additionally need to specify values for the target metric to use: conversion, revenue, CPA or ROI. 

To create a plan, in the ![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** interface in Mix Modeler, select **[!UICONTROL Create plan]**.


1. In the **[!UICONTROL Plan creation]** screen:

   1. In the **[!UICONTROL Setup]** section:

      1. Enter a **[!UICONTROL Plan name]**, for example `Demo plan`. Enter a **[!UICONTROL Description]**, for example `Demo plan for Luma company`.
      1. Select a **[!UICONTROL Model]** from **[!UICONTROL _Select an option.._.]**

         ![Plan Setup](/help/assets/plan-setup.png)

   1. In the **[!UICONTROL Goal]** section, select the goal you want to optimize your plan towards. You can select between

         * **[!UICONTROL I have a budget to spend]**

           ![Plan budget](../assets/plan-budget.png)

            This option allows you to input budgets for one or more date ranges. 

            1. In the **[!UICONTROL Optimize]** container:
               1. Select a conversion from the **[!UICONTROL Select conversion]** dropdown menu.
               1. Select a model from the **[!UICONTROL Select model]** dropdown menu.
            1. Specify a **[!UICONTROL Date range]**, either by typing dates or selecting a date range using ![Calendar](/help/assets/icons/Calendar.svg).
            1. Enter a **[!UICONTROL Budget]**.
               To add additional date ranges, each with their budget, select ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**.
               To delete a date range and associated budget, select ![Close](/help/assets/icons/Close.svg).
            1. To define an optional maximum budget that you would like to constrain the plan within:
               1. Switch **[!UICONTROL Maximize budget]** on.
               1. Specify the amount of the maximum budget. The amount should be equal or higher than the total amount of the budgets specified for the date ranges.


         * **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

           ![Plan target](../assets/plan-target.png)

            1. In the **[!UICONTROL Optimize]** container
               1. Select a conversion from the **[!UICONTROL Select conversion]** dropdown menu.
               1. Select a target metric from the **[!UICONTROL Select target metric]** dropdown menu. You can select between **[!UICONTROL Conversion]**, **[!UICONTROL CPA]**, **[!UICONTROL Revenue]**, or **[!UICONTROL ROI]**.
               1. Select a model from the **[!UICONTROL Select model]** dropdown menu.
            1. Specify a Date range, either by typing dates or selecting a date range using ![Calendar](/help/assets/icons/Calendar.svg).
            1. Enter a value for the selected target metric. For example, a number for **[!UICONTROL Conversion]**, a percentage for **[!UICONTROL ROI]**, or currency values for **[!UICONTROL CPA]** and **[!UICONTROL Revenue]**.
               To add additional date ranges, each with their target metric, select ![CalendarAdd](/help/assets/icons/CalendarAdd.svg) **[!UICONTROL Add row]**.
               To delete a date range and associated target metric, select ![Close](/help/assets/icons/Close.svg).
            1. To define an optional maximum budget that you would like to constrain the plan within:
               1. Switch **[!UICONTROL Maximize budget]** on.
               1. Specify the amount of the maximum budget.


   1. Select **[!UICONTROL Next]**.

1. In the **[!UICONTROL Done with all required fields]** dialog:

    ![Plan Done](/help/assets/plan-done-required-fields.png)

    * Select ![NewPlan](/help/assets/icons/NewPlan.svg) **[!UICONTROL Create plan now]** if you want to generate an AI recommended plan with forecasted ROI. Select **[!UICONTROL OK]**. Your plan is created. 

   



    * Select ![TableEdit](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]** if you want to edit channel budget and define advanced configurations before a plan with forecasted ROI is created.  Select **[!UICONTROL OK]**, so you can define your channel spend in **[!UICONTROL Spend selection]** in the next step.

    
      >[!IMPORTANT]
      >
      >The information below is only relevant if you have selected the ![TableEdit](/help/assets/icons/TableEdit.svg) **[!UICONTROL Edit channel budgets first]**


1. In the **[!UICONTROL Spend selection]** section, for each budget date range, use the ![Chevron](/help/assets/icons/ChevronRight.svg) to open the channel distribution view for that data range.

    You can use historical reference data if you want to use past marketing spend data and insights. Consider historical reference data to:

    * Improve budget allocation by highlighting high-performing channels and poorly performing channels.
    * Support trend analysis. 
    * Identify effective strategies and avoid mistakes while configuring plans. 
    
    If you select a historical reference period, you align to previous spend pattern preferences and Mix Modeler's planning functionality can generate plans that are within your expectations. These plans should ultimately enhance stakeholder confidence, ensure that marketing plans are strategic, efficient, and that these plans are grounded in proven performance data and business needs.

    ![Spend selection](/help/assets/plan-spend-selection.png)

    1. Select the **[!UICONTROL Spend pattern]**. 
 
       * The default option is **[!UICONTROL Automatic]**. 
       * Select **[!UICONTROL Historical reference]** and enter a **[!UICONTROL Start date]** to refer to past marketing spend data already available to Mix Modeler. The **[!UICONTROL End date]** is automatically determined based on the date range for which you define the spend pattern. The proposed start date is the first available past marketing spend date available. To indicate you have selected a non-existing or invalid historical reference period, you see a ![AlertRed](/help/assets/icons/AlertRed.svg).

    1. To define budgets for each channel, enter a value for **[!UICONTROL Min]** and **[!UICONTROL Max]** or use the sliders.

    1. To toggle between currency or percentage input, select **[!UICONTROL $]** or **[!UICONTROL %]** for **[!UICONTROL View spend by]**. This toggle is disabled if you have selected target metrics that are not currency-based.

    1. When finished, select **[!UICONTROL Create]**. 
       ![Spend selection](/help/assets/plan-spend-selection.png)

    1. Select **[!UICONTROL Next]**.


   
1. In the **[!UICONTROL Advanced configurations]** section, you can enter optional advanced configurations.

   ![Plan summary](../assets/plan-advanced-configurations.png)

   * Your plan name , model, date range and total budget are summarized.

   * By default, Mix Modeler automatically calculates the average revenue per conversion using the latest historical seasonal data. In **[!UICONTROL Average Revenue per conversion]** you can define specific average revenue per conversion.

     1. For each date range in your budget:
   
        1. Select a date range from the **[!UICONTROL Date range]** dropdown menu.
        1. Enter an **[!UICONTROL Average revenue]** value.
   
     1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) Add custom average revenue per conversion unit to add a date range.
     1. Select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg) to remove a date range.

     >[!NOTE]
     >
     >If your model doesn't include historical revenue data, you must define an average revenue per conversion for each date range you specified for your budget.
     >

   * By default, Mix Modeler automatically calculates channel costs using the latest historical seasonal data. In **[!UICONTROL Channel costs]** you can define custom channel costs.

     1. For each channel in your model, define a custom channel cost.

        1. Select a channel from the **[!UICONTROL Channel]** dropdown menu.
        1. For each date range in your budget:   
           1. Select a date range from the **[!UICONTROL Date range]** dropdown menu.
           1. Enter an **[!UICONTROL Average revenue]** value.
        1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]** to add a date range.
        1. Select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg) to remove a date range.

     1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]** to add a channel.
     1. Select ![CrossSize400](/help/assets/icons/CrossSize400.svg) to remove a custom channel.

        
1. When finished, select **[!UICONTROL Create]**. 

1. In the **[!UICONTROL Create plan]** dialog, select **[!UICONTROL Create plan]** to create your plan. Select **[!UICONTROL Cancel]** to cancel the creation of your plan. A **[!UICONTROL No work is saved]** dialog is shown to confirm.

