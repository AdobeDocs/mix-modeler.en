---
title: Models overview
description: Learn how to build and use models in Mix Modeler.
feature: Models
exl-id: c43d9bc9-4429-45c2-9247-bd24510a24be
---
# Models overview

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

When a model is first created, the creation immediately kicks off the training and scoring process. After the completion of the initial training and scoring run, model insights are available for review. A model may subsequently be re-trained. Also, data may be added to the model which requires you to rescore the model manually. Re-trainng and re-scoring are an iterative process as new findings and information emerge and adjustments are needed to obtain a model fit that is most appropriate for your business objectives. 


## Build models

To build a model, use the Mix Modeler step-by-step guided model configuration flow available when you select **[!UICONTROL Open model canvas]**. See [Build models](build.md) for more details.

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
   | Status | The status of the model. |

   {style="table-layout:auto"}

   The reported status of the model is dependent on where a model is within its lifecycle. For example, whether a model is created, (re-)trained successfully or not, or (re-)scored successfully or not. 
   
   In the table below:

   * ![Checkmark](/help/assets/icons/Checkmark.svg) - indicates a successful execution of a step in the model lifecycle.
   * ![Clock](/help/assets/icons/Clock.svg) - indicates a current ongoing execution of a step in the model lifecycle.
   * ![Close](/help/assets/icons/Close.svg) - indicates a failed execution of a step in the model lifecycle.
  
   | Status | [Build](/help/models/build.md) | [Train](/help/models/train-score.md#train) | [Score](/help/models/train-score.md#score) | [Retrain](/help/models/train-score.md#train) | [Rescore](/help/models/train-score.md#score) |
   |---|:---:|:---:|:---:|:---:|:---:|
   | In progress | ![Checkmark](/help/assets/icons/Checkmark.svg) | | | | |
   | In progress | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Clock](/help/assets/icons/Clock.svg) | | | |
   | In progress | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Clock](/help/assets/icons/Clock.svg) | | |
   | In progress | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Clock](/help/assets/icons/Clock.svg) | | 
   | In progress | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) |  ![Clock](/help/assets/icons/Clock.svg) |
   | Training failed | ![Checkmark](/help/assets/icons/Checkmark.svg)  | ![Close](/help/assets/icons/Close.svg) | | | | 
   | Training failed | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Close](/help/assets/icons/Close.svg) | |
   | Training successful | ![Checkmark](/help/assets/icons/Checkmark.svg)  | ![Checkmark](/help/assets/icons/Checkmark.svg) | | | | 
   | Training successful | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | |
   | Scoring failed | ![Checkmark](/help/assets/icons/Checkmark.svg)  | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Close](/help/assets/icons/Close.svg) | | | 
   | Scoring failed | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Close](/help/assets/icons/Close.svg)|
   | Scoring successful | ![Checkmark](/help/assets/icons/Checkmark.svg)  | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | | | 
   | Scoring successful | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg) | ![Checkmark](/help/assets/icons/Checkmark.svg)|

   {style="table-layout:fixed"}

1. To change the columns displayed for the list, select ![Column settings](/help/assets/icons/ColumnSetting.svg) and toggle columns on ![Check](/help/assets/icons/Checkmark.svg) or off.

You can take the following actions on a specific model.

### Model insights

The model insights functionality is only available on successfully trained and scored models.

To view the insights of a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

   1. Select the model name. 

You are redirected to [Model Insights](insights.md).  
   

### View details

To view more details of a model:

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   
1. Select ![Info](/help/assets/icons/Info.svg) for a model to show a pop-up with details.


### Duplicate

You can quickly duplicate a model.

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Duplicate]**.

You are redirected to the steps to create a new model, with a proposed name composed of the original model's name appended with **[!UICONTROL (Copy)] (_n_)**.

### Edit

You can edit the name, description and the scheduling of training and scoring of a model.

1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.

1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Edit]**.

   In the **[!UICONTROL Edit model]** dialog:

   * Enter a new **[!UICONTROL Name]** and **[!UICONTROL Description]**.

   * To enable scheduling, enable **[!UICONTROL Status]**. You can only enable scheduling for models that are trained and scored.

      1. Select a **[!UICONTROL Scoring frequency]**:

         * **[!UICONTROL Daily]**: Enter a valid time (for example `05:22 pm`) or use ![Clock](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Weekly]**: Select a day of the week and enter a valid time (for example `05:22 pm`) or use ![Clock](/help/assets/icons/Clock.svg).
         * **[!UICONTROL Monthly]**: Select a day of the month from the Run on every dropdown menu and enter a valid time (for example `05:22 pm`) or use ![Clock](/help/assets/icons/Clock.svg).

      1. Select a **[!UICONTROL Training frequency]** from the dropdown menu: **[!UICONTROL Monthly]**, **[!UICONTROL Quarterly]**, **[!UICONTROL Yearly]**, or **[!UICONTROL None]**. 

      ![Edit a model](../assets/model-edit.png)

1. Select **[!UICONTROL Save]**.
   


### Train

Consider to retrain a model when you want to include new incremental marketing and factor data. See [Train and score models](train-score.md#train) for more information.


### Score

You can incrementally score a model based on new marketing data or rescore a model for a specific date range. See [Train and score models](train-score.md#score) for more information.


### Delete models

To delete a model:

   1. Select ![](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   1. Select ![More](/help/assets/icons/More.svg) for a model, and from the context menu select **[!UICONTROL Delete]**. Alternatively, select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** from the blue action bar.
   1. Select **[!UICONTROL Delete]** in the **[!UICONTROL Delete model]** confirmation dialog to delete the model. Select **[!UICONTROL Cancel]** to cancel.

To delete multiple models:

   1. Select multiple models.
   1. From the blue action bar, select ![Delete](/help/assets/icons/Delete.svg) **[!UICONTROL Delete]** to delete the models. 
   1. Select **[!UICONTROL Delete]** in the **[!UICONTROL Delete *x* models]** confirmation dialog to delete the models. Select **[!UICONTROL Cancel]** to cancel.

