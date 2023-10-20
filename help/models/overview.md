---
title: Models
description: Learn how to configure and use models in Mix Modeler.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
---
# Models

The model functionality in Mix Modeler allows you to configure, train, and score AI/ML models specific to your business objectives and supported by AI-driven transfer learning between multitouch attribution and marketing mix modeling. 

The models are based on the harmonized data that you create as part of the Mix Modeler application workflow.

A model in Mix Modeler is a machine learning model employed to measure and / or predict a specified outcome based on a marketer's investments. Marketing touchpoints and summary-level data can be used as an input. Mix Modeler allows you to create variants of models based on different sets of variables, dimensions, and outcomes, such as revenues, units sold, leads.

A model requires:

* one conversion,
* one or more marketing touchpoints (channels) comprised of summary-level data, marketing touchpoint data (event data) or both,
* a configurable lookback window for
* a configurable training window.

A model can optionally include:

* external factors,
* internal factors,
* so-called 'priors' (probability distribution representing knowledge or uncertainty of data prior or before observing that data), which indexes prior conversions by channel,
* spend share, which uses relative spend share as a proxy when marketing data is sparse.


## Create a model

To create a model, use the Mix Modeler step-by-step guided model configuration flow available when you select **[!UICONTROL Guide me]**. See [Create a model](create.md) for more details.

## Manage models

To view a table of your current models, in the Mix Modeler interface:

1. Select ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   
1. You see a table of the current models.

    The table columns specify details about the model.

    | Column name | Details |
    |---|---|
    | Name | Name of the model |
    | Description | Description of the model |
    | Conversion Events | The conversion you have selected for the model. |
    | Dataset | The dataset that the model uses to train and score. This is by default the harmonized dataset. |
    | Run frequency | The running frequency of training the model. |
    | Last run | The date and time of the last training of the model. |
    | Last run status | The status of the last run of the training of the model. <br/><span style="color:green">●</span> Success<br/><span style="color:orange">●</span> Training issue<br/> <span style="color:orange">●</span> Awaiting training <br/><span style="color:red">●</span> Failed|

    {style="table-layout:auto"}

1. To change the columns displayed for the list, select ![Column settings](../assets/icons/ColumnSetting.svg) and toggle columns on ![Check](../assets/icons/Checkmark.svg) or off.

### Delete a model

To delete a model:

   1. Select the name of the model that you want to delete.

   1. From the context menu, select **[!UICONTROL Delete]** to delete the model. 

### View details of a model

To view more details of a model:

   1. Select the name of the model that you want to view more details of.

   1. From the context menu, select **[!UICONTROL More]**. You see details of the selected model in the right pane.



### Model insights

>[!NOTE]
>
>This selection is only available on successfully trained models.
>

To view insights of a model, in the Mix Modeler interface:

   1. Select ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select the name of a model with a **[!UICONTROL Last run status]** of <span style="color:green">●</span> **[!UICONTROL Success]** from the **[!UICONTROL Models]** table.

   1. From the context menu, select **[!UICONTROL Model Insights]**. You are redirected to [Model Insights](insights.md).
