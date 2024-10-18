---
title: Models
description: Learn how to configure and use models in Mix Modeler.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
---
# Models

The model functionality in Mix Modeler allows you to configure, train, and score models specific to your business objectives. The training and scoring supports AI-driven transfer learning between multitouch attribution and marketing mix modeling. 

The models are based on the harmonized data that you create as part of the Mix Modeler application workflow.

A model in Mix Modeler is a machine learning model employed to measure and predict a specified outcome based on a marketer's investments. Marketing touchpoints and summary-level data can be used as an input. Mix Modeler allows you to create variants of models based on different sets of variables, dimensions, and outcomes, such as revenues, units sold, leads.

A model requires:

* One conversion.
* One or more marketing touchpoints (channels) comprised of summary-level data, marketing touchpoint data (event data) or both.
* A configurable lookback window.
* A configurable training window.

A model can optionally include:

* External factors.
* Internal factors.
* Prior knowledge of marketing contributions from other sources such as past stakeholder experience, incrementally testing, other models.
* Spend share, which uses relative spend share as a proxy when marketing data is sparse.


## Create a model

To create a model, use the Mix Modeler step-by-step guided model configuration flow available when you select **[!UICONTROL Open model canvas]**. See [Create a model](create.md) for more details.

## Manage models

To view a table of your current models, in the Mix Modeler interface:

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   
1. You see a table of the current models.

    The table columns specify details about the model.

    | Column name | Details |
    |---|---|
    | Name | Name of the model |
    | Description | Description of the model |
    | Conversion event | The conversion you have selected for the model. |
    | Run frequency | The running frequency of training the model. |
    | Last run | The date and time of the last training of the model. |
    | Status | The status of the last run of the training of the model. <br/>![StatusGreen](/help/assets/icons/StatusGreen.svg) Success<br/>![StatusOrange](/help/assets/icons/StatusOrange.svg) Training issue<br/> ![StatusOrange](/help/assets/icons/StatusOrange.svg) Awaiting training <br/>![StatusRed](/help/assets/icons/StatusRed.svg) Failed <br/>![StatusGreen](/help/assets/icons/StatusGray.svg) _ (when a last run is in progress) |

    {style="table-layout:auto"}

1. To change the columns displayed for the list, select ![Column settings](/help/assets/icons/ColumnSetting.svg) and toggle columns on ![Check](/help/assets/icons/Checkmark.svg) or off.

You can take the following actions on a specific model.

### View details

To view more details of a model:

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   
1. Select ![Info](/help/assets/icons/Info.svg) for a model to show a pop-up with details.



### Duplicate

You can quickly duplicate a model.

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Duplicate]**.
   

### Model insights

The model insights functionality is only available on successfully trained and scored models.

To view the insights of a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select the model name. 

You are redirected to [Model Insights](insights.md).  
   

### Re-train


Re-train a model is only available on successfully trained models. 

Consider to re-train a model when you want to:

* Include new incremental marketing and factor data. For example, over the last quarter, market dynamics have changed or your marketing data distribution has changed significantly.

To re-train a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Train]**. Alternatively, select ![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Train]** from the blue action bar.

      In the **[!UICONTROL Train model]** dialog, select the option to: 

      * **[!UICONTROL Train model with last 2 years of marketing data]**, or 
      * **[!UICONTROL Train model using specific date range of data]**. 
        Specify the date range. You can use the ![Calendar](/help/assets/icons/Calendar.svg) to select a date range. You have to select a data range with a minimum of one year.

      ![Re-train a model](../assets/re-train-model.png)

   1. Select **[!UICONTROL Train]** to re-train the model.


### Score or re-score


You can incrementally score a model based on new marketing data or re-score a model for a specific date range. 

Consider to re-score a model when you want to:

* Correct incorrect marketing data. For example, the recent paid search data you included in the training and scoring of the model missed a week of data.
* Use new incremental marketing data that has become available through updates in the datasets you have configured as part of your harmonized data.

To score or re-score a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Score]**. Alternatively, select ![DataRefresh](/help/assets/icons/DataRefresh.svg) **[!UICONTROL Score]** from the blue action bar.

      In the **[!UICONTROL Score marketing data]** dialog, select the option to: 

      * **[!UICONTROL Score new marketing data from *mm/dd/yyyy*]**, to score your model incrementally using new marketing data, or 
      * **[!UICONTROL Score specific date range of marketing data]** to re-score for a specific date range. 
        Specify the date range. You can use the ![Calendar](/help/assets/icons/Calendar.svg) to select a date range. 

      ![Re-train a model](../assets/re-score-model.png)

   1. Select **[!UICONTROL Score]**. When re-scoring a model using a specific data range, you see an **[!UICONTROL Existing model is replaced]** dialog, prompting you to confirm to replace the model with new scores for the selected date range. Select **[!UICONTROL Replace model]** to confirm.

### Edit

 1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

    1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Edit]**.

      In the **[!UICONTROL Edit model]** dialog, select the option to rename the model.

      * Enter a new name and description.

      * To enable scheduling, enable Status. 

        

      ![Re-train a model](../assets/model-edit.png)

    1. Select **[!UICONTROL Score]**. When re-scoring a model using a specific data range, you see an **[!UICONTROL Existing model is replaced]** dialog, prompting you to confirm to replace the model with new scores for the selected date range. Select **[!UICONTROL Replace model]** to confirm.



### Delete a model

To delete a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Delete]**. Alternatively, select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** from the blue action bar.

To delete multiple models:

   1. Select multiple models.

   1. From the blue action bar, select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** to delete the models. 

      >[!WARNING]
      >
      >The model is deleted immediately.


