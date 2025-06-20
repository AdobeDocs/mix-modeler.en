---
title: Plans overview
description: Learn how to view, select, and action on plans in Mix Modeler.
feature: Plans
exl-id: 45a8dc30-3259-493d-8ea5-1899903733a6
---
# Plans overview

Plans in Mix Modeler allow you to allocate budgets by business unit and channel. The planning functionality is integrated with the outcomes of the trained models based on your harmonized data.

A plan outlines the discretionary investments (for example budgets) a business intends to spend on marketing-related projects over the course of a given timeframe. These investments are in service of common KPIs (for example orders, revenue). Plans can inclusd expenses from channels such as paid advertising, sponsored web content, events.

A plan requires:

- a model,
- a data range,
- a budget.

A plan can optionally include:

- a configured recognition window,
- multiple flight dates with each having a target budget,
- minimum and maximum budget constraints by channel and flight date.

If a model that you have used for your plan is scored on new data, you need to create a new plan to take into account the re-scored data.


## Build plans

To build a plan, use the Mix Modeler plan creation wizard. See [Build plans](build.md) for more details.


## Manage plans

To view a table of your current plans, in the Mix Modeler interface:

1. Select ![](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** from the left rail.

1. You see a table of the current plans and their status.

    The table columns specify details about the plans.

    | Column name | Details |
    |---|---|
    | Name | Name of the plan |
    | Model | The model used as the base for the plan. |
    | Date range | The full date range for a plan. |
    | Budget | The total budget for a plan. |
    | Plan target | The target metric defined for a target based plan. |
    | Forecasted return | The [forecasted return](/help/main-guide/glossary.md) for a plan |
    | Forecasted ROI | The [forecasted ROI](/help/main-guide/glossary.md) for a plan. |
    | Forecasted conversion | The [forecasted conversion](/help/main-guide/glossary.md) for a plan |
    | Forecasted CPA | The [forecasted CPA](/help/main-guide/glossary.md)for a plan |
    | Status | The status of a plan: <p><span style="color:red">●</span> Failed, <p><span style="color:blue">●</span> Processing, or <p><span style="color:green">●</span> Complete. |

    {style="table-layout:auto"}

    You can use ![ColumnSetting](/help/assets/icons/ColumnSetting.svg) to select ![Checkmark](/help/assets/icons/Checkmark.svg) the columns to display in the table. 

1. Use ![Search](/help/assets/icons/Search.svg) to search and filter the table for one or more specific plans.

### Plan insights

To view the insights of a plan and to edit a plan:

   1. Select ![PLan](/help/assets/icons/FileChart.svg) **[!UICONTROL Plans]** from the left rail.

   1. Select the plan name. 
   
   You are redirected to [Plan insights](insights.md).  


### Duplicate a plan

To duplicate a plan:

- Select ![More](/help/assets/icons/More.svg) for a plan. From from the context menu, select **[!UICONTROL Duplicate]**.
- Alternatively, select a plan in the table ![SelectBox](/help/assets/icons/SelectBox.svg) and select ![Copy](/help/assets/icons/Copy.svg) **[!UICONTROL Duplicate]** from the blue action bar.

A new plan, with a name composed of the original plan's name appended with **[!UICONTROL (Copy)] (_n_)**, is created. You are automatically redirected to [Plan creation](build.md) to provide updated details for the copied plan. 

- Details (like Description, Budget, and more) from the original plan are copied over. 
- Budget constraints from the original plan are copied over to the newly created plan.
- You have the option to select another model as the base for the copied plan.
  - For touchpoints or channels that do exist in the copied plan, but do not exist in the newly selected model, any constraints for these touchpoints or channels are removed from the plan.
  - For touchpoints or channels that do not exist in the copied plan, but do exist in the newly selected model, the constraints are set to:
    - a minimum value of `0`, 
    - a maximum value in line with the plan flight range budget. 



### Compare plans

To compare plans:

1. Select two plans from the table.
1. Select ![Compare](/help/assets/icons/Compare.svg) **[!UICONTROL Compare]** from the blue action bar. You see the **[!UICONTROL Compare plans]** UI. 


### Delete plans

To delete a plan:

   1. Select ![More](/help/assets/icons/More.svg) for a plan. From the context menu, select **[!UICONTROL Delete]**. <br/>Alternatively, select a plan in the table ![SelectBox](/help/assets/icons/SelectBox.svg) and select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** from the blue action bar.
   1. Select **[!UICONTROL Delete]** in the **[!UICONTROL Delete plan]** confirmation dialog to delete the plan. Select **[!UICONTROL Cancel]** to cancel.

To delete multiple plans:

   1. Select multiple plans.
   1. From the blue action bar, select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** to delete the plans. 
   1. Select **[!UICONTROL Delete]** in the **[!UICONTROL Delete *x* plans]** confirmation dialog to delete the plans. Select **[!UICONTROL Cancel]** to cancel.


