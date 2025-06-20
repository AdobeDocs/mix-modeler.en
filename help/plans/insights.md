---
title: Plan insights
description: Learn how to see insights of your plan and edit a plan in Mix Modeler.
feature: Plans
exl-id: 91385595-284f-4fcb-b54b-9539905e552b
---
# Plan insights

  
In [!UICONTROL Plan insights], your plan insights are created, showing the [!UICONTROL Model], the [!UICONTROL Data range], and the [!UICONTROL Plan target] on which the plan is based.


When the insights are created, you see an overview of your plan, consisting of: 

- A header that displays the [!UICONTROL Model], the [!UICONTROL Data range], and the [!UICONTROL Plan target] on which the plan is based.
  - In case you have defined a goal based plan, a badge indicates the status of your target Possible options are:

    - [!BADGE Target achievable]{type=Positive}
    - [!BADGE Target unachievable]{type=Negative}

  - Select ![ChevronDown](/help/assets/icons/ChevronDown.svg) **[!UICONTROL Show more]** to show more details.

- [[!UICONTROL Forecasted paid channel ROI] visualization](#forecasted-paid-channel-spend-and-roi)
- [[!UICONTROL Forecasted revenue] visualization](#forecasted-revenue)
- [[!UICONTROL Forecasted conversion] visualization](#forecasted-conversions)
- [[!UICONTROL Marginal channel return] visualization](#marginal-channel-return)
- [[!UICONTROL Data range breakdown] table of the plan](#date-range-breakdown), showing columns for

  - Channel
  - ROI
  - CPA
  - Revenue
  - Conversion goal
  - Spend

To close the interface, select **[!UICONTROL Close]**. 

To change how to view the ROI of your plan, select **[!UICONTROL X]** or **[!UICONTROL  %]** at **[!UICONTROL View ROI]**. 

## Forecasted paid channel spend and ROI

This visualization shows a scatterplot for the forecasted spend and return on investment on your paid channels, based on the model, date range and budget.

![Forecasted paid channel spend and ROI visualization](../assets/overview-plan-forecasted-paid-channel-send-roi.png)


## Forecasted revenue

This bar chart visualization shows the forecasted revenue for your channels based on the model, date range and budget.

![Forecasted revenue visualization](../assets/overview-plan-forecasted-revenue.png)


## Forecasted conversions

This bar chart visualization shows the forecasted conversions for your channels based on the model, date range and budget.

![Forecasted conversions visualization](../assets/overview-plan-forecasted-conversions.png)


## Marginal channel return

This line chart visualization shows a marginal return curve for the selected channel with indicators for the **[!UICONTROL Marginal break-even]** and **[!UICONTROL Return point]**. This visualization helps you to understand how the spend for a channel is from reaching a marginal break-even point. And whether you have room to increase spend in a channel or should spend less on a channel to improve the channel spend efficiency.

![Marginal channel return visualization](../assets/overview-plan-marginal-channel-return.png)

To select a specific channel for the visualization, select a channel from the **[!UICONTROL View]** dropdown menu.


## Date range breakdown

The [!UICONTROL Date range breakdown] table shows detailed granular data per channel for [!UICONTROL ROI], [!UICONTROL Revenue], [!UICONTROL CPA], [!UICONTROL Conversions] and [!UICONTROL Spend].

![Date range breakdown table](../assets/overview-plan-date-range-breakdown.png)

1. To download a CSV file containing the data of the Date range breakdown, select ![Download](/help/assets/icons/Download.svg) **[!UICONTROL Download CSV]**. From the context menu:

   - Select ![Download](/help/assets/icons/Download.svg) **[!UICONTROL Detailed CSV]** for detailed data in CSV format. 
   - Select ![Download](/help/assets/icons/Download.svg) **[!UICONTROL Summary CSV]** for summary data in CSV format. 

   Detailed data is granular data keyed by week. Summary data is data keyed by the model-provided date range.

1. To view the Date range breakdown by category of channels, select **[!UICONTROL All channels]**, **[!UICONTROL Paid channels]**, or **[!UICONTROL Non-paid channels]** from the **[!UICONTROL View]** selection.


## Edit plan

To edit your plan, select ![Edit](/help/assets/icons/Edit.svg) **[!UICONTROL Edit plan]**.
    
1. In the **[!UICONTROL Spend selection]** section, for each budget date range, use the ![Chevron](/help/assets/icons/ChevronRight.svg) to open the channel distribution view for that data range.

   You can use historical reference data if you want to use past marketing spend data and insights. Consider historical reference data to:

   - Improve budget allocation by highlighting high-performing channels and poorly performing channels.
   - Support trend analysis. 
   - Identify effective strategies and avoid mistakes while configuring plans. 
    
   If you select a historical reference period, you align to previous spend pattern preferences and Mix Modeler's planning functionality can generate plans that are within your expectations. These plans should ultimately enhance stakeholder confidence, ensure that marketing plans are strategic, efficient, and that these plans are grounded in proven performance data and business needs.

   ![Spend selection](/help/assets/plan-spend-selection.png)

   1. Select the **[!UICONTROL Spend pattern]**. 

       - The defaul option is **[!UICONTROL Automatic]**. 
       - Select **[!UICONTROL Historical reference]** and enter a **[!UICONTROL Start date]** to refer to past marketing spend data already available to Mix Modeler. The **[!UICONTROL End date]** is automatically determined based on the selected data range. The proposed start date is the first available past marketing spend data available. To indicate you have selected a non-existing historical reference period, you see a ![AlertRed](/help/assets/icons/AlertRed.svg).


   1. To modify the budgets for each channel, modify the values for **[!UICONTROL Min]** and **[!UICONTROL Max]** or use the sliders.

   1. To toggle between currency or percentage input, select **[!UICONTROL $]** or **[!UICONTROL %]** for **[!UICONTROL View spend by]**.

   1. To edit the details of your plan, select **[!UICONTROL Edit details]**:

      1. In the **[!UICONTROL Setup]** section:

         1. Enter a **[!UICONTROL Plan name]**, for example `Demo plan`. Enter a **[!UICONTROL Description]**, for example `Demo plan for Luma company`.
         1. Select a **[!UICONTROL Model]** from **[!UICONTROL _Select an option.._.]**

            ![Plan Setup](/help/assets/plan-setup.png)

      1. In the **[!UICONTROL Goal]** section, select the goal you want to optimize your plan towards. You can select between
         - **[!UICONTROL I have a budget to spend]**

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


         - **[!UICONTROL I have a target to achieve]** [!BADGE Beta]

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

         1. Select **[!UICONTROL Next]** to return to the **[!UICONTROL Spend selection]** section. 

1. In the **[!UICONTROL Advanced configuration]** section:

   ![Edit advanced configuration](../assets/edit-plan-advanced-configuration.png)

      - Your plan name , model, date range and total budget are summarized.

      - By default, Mix Modeler automatically calculates the average revenue per conversion using the latest historical seasonal data. In **[!UICONTROL Average Revenue per conversion]** you can define specific average revenue per conversion.

   1. For each date range in your budget:
      1. Select a date range from the **[!UICONTROL Date range]** dropdown menu.
      1. Enter an **[!UICONTROL Average revenue]** value.
   1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) Add custom average revenue per conversion unit to add a date range.
   1. Select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg) to remove a date range.

   >[!NOTE]
   >
   >If your model doesn't include historical revenue data, you must define an average revenue per conversion for each date range you specified for your budget.
   >

   - By default, Mix Modeler automatically calculates channel costs using the latest historical seasonal data. In **[!UICONTROL Channel costs]** you can define custom channel costs.

   1. For each channel in your model, define custom channel cost.
      1. Select a channel from the **[!UICONTROL Channel]** dropdown menu.
      1. For each date range in your budget:   
         1. Select a date range from the **[!UICONTROL Date range]** dropdown menu.
         1. Enter an **[!UICONTROL Average revenue]** value.
      1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom average revenue per conversion unit]** to add a date range.
      1. Select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg) to remove a date range.

   1. Select ![AddCircle](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add custom channel cost]** to add a channel.
   1. Select ![CrossSize400](/help/assets/icons/CrossSize400.svg) to remove a custom channel.


1. When you are finished editing your plan, select **[!UICONTROL Edit]**.

    In the **[!UICONTROL All changes are final]** dialog, select **[!UICONTROL OK]** to update the plan's current spend allocation and ROI and revenue forecasts. Select **[!UICONTROL Cancel]** to cancel the update of your plan.


- To cancel your plan updates at any time, select **[!UICONTROL Cancel]**. In the **[!UICONTROL No work will be saved]** dialog, select **[!UICONTROL Cancel]** to continue to work on your plan or select **[!UICONTROL OK]** to return back to the Plans interface.
- To go back in the wizard, select **[!UICONTROL Back]**.
