---
title: Model Insights
description: Learn how to get details about your model, like historical overview, model insights, and model quality in Mix Modeler.
feature: Models
exl-id: d99852f9-ba0d-4a2e-b5f3-ca0efe6002fd
---
# Model Insights

To view model insights, in the ![Models](./help/assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler:

1. From the **[!UICONTROL Models]** table, select the name of a model that has a **[!UICONTROL Last run status]** of <span style="color:green">●</span> **[!UICONTROL Success]**.
   
1. From the context menu, select **[!UICONTROL Model Insights]**.

![Model insights tab bar](./help/assets/model-insights-tabbar.png)

You see when the specified model is last refreshed and widgets are displayed using four tabs: [Model insights](#model-insights), [Attribution](#attribution), [Diagnostics](#diagnostics), and [Historical overview](#historical-overview).

You can change the date period on which the widgets on each of the tabs are based on. Enter a date period or select ![Calendar](./help/assets/icons/Calendar.svg) to select a date period.

## [!UICONTROL Model insights]

The Model insights tab shows widgets for:

* Contribution by date and base media. The stacked graph is ordered: Base at the bottom, Non-spend channels in the middle, and Spend channels on top.

* Contribution by channel.

* Marketing performance summary.

* Marginal response curves. 
  <br/>Select a channel from the **[!UICONTROL Channel]** dropdown list to update the widget for a specific channel.

![Model - Model insights](./help/assets/model-insights-insights.png)

You can hover over individual chart elements in each widget to display a popover with more details.

To download a CSV file containing the data for the widget, select ![Download](./help/assets/icons/Download.svg).

To download full model insights data in Microsoft&reg; Excel format, select ![Download](./help/assets/icons/Download.svg) **[!UICONTROL Download data]**. 

## [!UICONTROL Attribution]

Using the [!UICONTROL Attribution] tab, you can understand the effectiveness of touchpoints and marketing campaigns that have event level data. The following attribution models are supported:

* Based on the selected model in Mix Modeler:
  * Algorithmic - Influenced
  * Algorithmic - Incremental
* Rule based:
  * Decay units
  * First touch
  * Last touch
  * Linear
  * Ushape

See [Multi-touch attribution](../get-started/about.md#multi-touch-attribution) for an introduction on the multi-touch attribution capability in Mix Modeler.

Select one or more attribution models from the **[!UICONTROL Attribution Model]** dropdown list. The selected attribution models apply to all widgets in the Attribution tab.

![Attribution](./help/assets/model-insights-attribution.png)

The Mix Modeler multi-touch attribution granular event scores align to the overall Mix Modeler scores and ROIs. These scores are also made available as datasets in Experience Platform.

The Attribution tab consists of the following widgets:

### [!UICONTROL Overview]

The [!UICONTROL Overview] widget shows, for the selected attribution models, the conversions totals and percentages. Selecting more models adds additional circles to the visualization, each with its own color corresponding to the legend.

To see a popup with details for an attribution model, hover over any of the circles in the visualization.

### [!UICONTROL Trends]

The [!UICONTROL Daily trends], [!UICONTROL Weekly trends], or [!UICONTROL Monthly trends] widget shows, for the selected attribution models, the daily, weekly, or monthly conversion trends.

To choose the period, select **[!UICONTROL Daily trends]**, **[!UICONTROL Weekly trends]** or **[!UICONTROL Monthly trends]** from ![More](./help/assets/icons/More.svg).

To see details, hover over the data line of a specific attribution model to display a popover that shows the total number of conversions for that data. 

### [!UICONTROL Breakdown]

The [!UICONTROL Breakdown] widget is a breakdown by channel or touchpoint of the conversions for each of the selected attribution models. This widget can be helpful to make decisions on the effectiveness of each channel or touchpoint.

To choose the breakdown type, select **[!UICONTROL Breakdown by channel]** or **[!UICONTROL Breakdown by touchpoint]** from ![More](./help/assets/icons/More.svg).

To see details, hover over any of the chart elements.

### [!UICONTROL Top campaigns]

The Top campaigns widget shows a table of the top campaigns with columns for Campaign name, Channel, Media type and Incremental conversions. This widget can help inform your team of the effectiveness of a specific campaign for a given channel and provide insights on what campaigns you should further invest into.

To sort the table in ascending &uarr; or descending order &darr; for Channel, Media type or Incremental conversions, select the column header and toggle the sort.

To expand the table in a separate dialog, select **[!UICONTROL Expand]** from ![More](./help/assets/icons/More.svg).

The expanded Top campaigns dialog shows the same table with addition columns for 

* Incremental conversions 
* Influenced conversions
* First touch conversions
* Last touch conversions
 
  You can select each of the additional column headers to sort the table in ascending or descending order.
  
To close the expanded Top campaigns dialog, select **[!UICONTROL Close]**.


### [!UICONTROL Breakdown by touchpoint position]

The [!UICONTROL Breakdown by touchpoint position] visualization is a breakdown of attributed conversions by position of the touchpoint and touchpoint across all the conversion paths. This chart helps you to compare if a touchpoint contributes better at a position than remaining positions and other touchpoints at any position. 

>[!NOTE]
>
>The sum of percentage contribution for an attribution model across all touchpoints and positions should be equal to 100. 


The positions [!UICONTROL Starter], [!UICONTROL Player] and [!UICONTROL Closer] are defined as follows:

| Position | Description |
|---|---|
| [!UICONTROL Starter] | This position indicates whether the touchpoint is the first touch in a conversion path. |
| [!UICONTROL Player] | This position indicates whether the touchpoint is not the first or the last touch leading to conversion. |
| [!UICONTROL Closer] | This position indicates whether the touchpoint is the last touch before conversion.| 


### [!UICONTROL Top conversion paths]

The [!UICONTROL Top conversion paths] visualization shows the top 5 conversion paths based on the selected attribution models. 

For each conversion path, you see:

* the number of channels that do have an impact, 
* the total attributed paths, 
* the percentage of attributed paths for this conversion path vs. total attributed paths,
* for each channel, the attribution model contribution percentage, and
* the sum of these channel attribution model contribution percentages.


## [!UICONTROL Diagnostics]

The Diagnostics tab shows widgets for:

* [!UICONTROL Model Assessment] visualization, which you can break down on Actual vs. Predicted or Residual conversions.

  To break down the visualization, select **[!UICONTROL Actual vs. Predicted]** or **[!UICONTROL Residuals]** from the **[!UICONTROL Breakdown]** list.

* [!UICONTROL Model fitting metrics] table, showing the following columns for each conversion metric:
  
  * Actual Conversion
    
  * Modeled Conversion
    
  * Residual Conversion (difference between actual and modeled conversion)
    
  * Model quality score values:

      * R2 (R-squared), which tells how well the data fits the regression model (the goodness of fit).

      * MAPE (Mean Absolute Percentage Error), which is one of the most commonly used KPIs to measure forecast accuracy and expresses the forecast error as a percentage of the actual value.

      * RMSE (Root Mean Square Error): which shows the average error, weighted according to the square of the error.

  To download a CSV file containing the data for the table, select ![Download](./help/assets/icons/Download.svg).

* [!UICONTROL Touchpoint effectiveness] table, representing the outcome of the Attribution AI algorithmic model. The data for this table is only generated for specific periods of time. Select **[!UICONTROL As of *xx/xx/xx, xx:xx TZ*]**  ![Info](./help/assets/icons/InfoOutline.svg) for more details.  
  
  The visualization shows, in descending order of [!UICONTROL Efficiency measure] ![Descending Order](./help/assets/icons/SortOrderDown.svg), for each touchpoint:

  * [!UICONTROL Paths touched]: visualizes the percentage of paths achieving conversion and percentage of paths not achieving conversion. For a touchpoint, you see more attributed conversions when the attribution conversion ratio is high. This ratio compares the percentage of paths that lead to conversion versus the percentage of paths that do *not* lead to conversion.
  * [!UICONTROL Efficiency measure]: generated by the algorithmic attribution model, the efficiency measure indicates the relative importance of a touchpoint toward conversion, independent of touchpoint volume. The efficiency is measured on a scale of 1 to 5. Note that higher touchpoint volume does not guarantee higher efficiency measure.
  * [!UICONTROL Total volume]: The aggregate number of times a user touches a touchpoint. The number is inclusive of touchpoints that appear on a path achieving conversion as well as paths *not* resulting in conversion.

![Diagnostics](./help/assets/model-insights-diagnostics.png)


## [!UICONTROL Historical overview]

The Historical overview tab shows widgets for:

* Conversion and Spend by Fiscal Qtr and Product.
  
* Spend by Channel.

* Touchpoint Spend.

  You can select an alternative spend-based channel to display for this widget. Select a channel from **[!UICONTROL Channels]**.

* Touchpoint Volume.

    You can select an alternative volume-based channel to display for this widget. Select a channel from **[!UICONTROL Channels]**.

![Model - Historical overview](./help/assets/model-insights-historical-overview.png)
