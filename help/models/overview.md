---
title: Models
description: Learn how to configure and use models in Adobe Mix Modeler.
---

# Models

The model functionality in Adobe Mix Modeler allows you to configure, trains and score AI/ML models specific to your business objectives and supported by AI-driven transfer learning between multitouch attribution and marketing mix modeling. 

The models are based on the harmonized data view you create as part of the Adobe Mix Modeler application workflow.

## Manage models

To view a list of your current models, in the Adobe Mix Modeler UI:

1. Select ![](../assets/icons/FileData.svg) **[!UICONTROL Models]** from the left rail.
   
1. You see a list of the current models.

    In the list view, columns specify details about the model.

    | Column name | Details |
    |---|---|
    | Name | Name of the model |
    | Description | Description of the model |
    | Conversion Events | The conversion you have selected for the model. |
    | Dataset | The dataset the model will use to train and score. This is by default the harmonized view. |
    | Run frequency | The run frequency of training the model. |
    | Last run | The date and time of the last training of the model. |
    | Last run status | The status of the last run of the training of the model |

1. To change the columns displayed for the list, select ![Column settings](../assets/icons/ColumnSetting.svg) and toggle columns on or off.
1. To delete a model:
   1. Select the name of the model you want to delete.
   1. From the context menu, select **[!UICONTROL Delete]** to delete the model. 
1. To view more details of a model:
   1. Select the name of the model you want to view more details of.
   1. From the context menu, select **[!UICONTROL More]**. In the right pane, you see details of your selected model.


## Create a model

To create a model, in the ![Models](../assets/icons/FileData.svg) **[!UICONTROL Models]** UI in Adobe Mix Modeler, select **[!UICONTROL Guide me]**.

To build your custom AI-powered models to measure and optimize your paid, owned, and earned marketing investments holistically using the power of Adobe Sensei, the UI provides a step-by-step guided model configuration flow.

   1. In the **[!UICONTROL Setup]** step:
      1. Enter your model name and enter a description.
      1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Cancel]** to cancel the model configuration.
   1. In the **[!UICONTROL Configure]** step:
      1. In the **[!UICONTROL Conversion goal]** section, within the container:
         1. Enter a name for the conversion.
         1. Select a conversion from the **[!UICONTROL *Select harmonized field*]** list. 
         1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new conversion]** to create a new conversion directly from within the model configuration.
      1. In the **[!UICONTROL Marketing touchpoints]** section, you see a list of marketing touchpoint containers, corresponding to the marketing touchpoints defined as part of your harmonized data view. 
         * For each container
           1. You can modify the name 
           1. Select a marketing touchpoint from the list.
           1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]** to create a new marketing touchpoint directly from within the model configuration.
         * To add a marketing touchpoint container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**.
         * To remove a marketing touchpoint container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

      1. By default, a score will be generated for all the data in your harmonized view. To only score a subset of the population, define one or more filters using containers in the **[!UICONTROL Eligible data population]** section. 
         * For each container, define one or more events.
           1. For each event: 
              1. Select a metric or dimension from the **[!UICONTROL _Select harmonized field_]** list.
              1. Select the appropriate operator from the **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]**, **[!UICONTROL is not in]** list.
              1. Enter of select a value.
           1. To add an additional event in the container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add event]**.
           1. To remove an event from the container, select ![Close](../assets/icons/Close.svg).
           1. To filter using all or any of multiple events defined in the container, select **[!UICONTROL Any of]** or **[!UICONTROL All of]**. The label will correspondingly change from **[!UICONTROL Include Or]** to **[!UICONTROL Include And]**.
         
         * To add an eligible data population container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.
         * To remove an eligibile data population container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

      1. To add datasets containing external factors to your model, use one or more containers in the **[!UICONTROL External factors dataset]** section. 
         * For each container:
           1. Enter a name.
           1. Select a dataset from the **[!UICONTROL _Select a dataset_]** list.
         * To add an additional external factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**.
         * To remove an external factors dataset container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

      1. To add datasets containing internal factors to your model, use one or more containers in the **[!UICONTROL Internal factors dataset]** section. 
         * For each container:
           1. Enter a name.
           1. Select a dataset from the **[!UICONTROL _Select a dataset_]** list.
         * To add an additional internal factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**.
         * To remove an additional internal factors dataset container, within the container, select ![More](../assets/icons/More.svg) and **[!UICONTROL Remove container]** from the context menu.

      1. To define the lookback window for the model, enter a value between `1` and `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**.
      1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Back]** to go back to the previous step. Select **[!UICONTROL Cancel]** to cancel the model configuration.
   1. In the **[!UICONTROL Advanced]** step:
      1. In the **[!UICONTROL Define training window]** section, select between 
         * **[!UICONTROL Have Adobe Mix Modele select a helpful training window]** and 
         * **[!UICONTROL Manually input a training window]** and define the number of years in **[!UICONTROL Include events the following years prior to a conversion]**.
      1. In the **[!UICONTROL Spend share]** section:
         * To allow spend share, activate **[!UICONTROL Allow spend share]** . Spend share will utilize historical marketing investment ratios to inform the model when marketing data is sparse.
      1. In the **[!UICONTROL Prior knowledge]** section:
         1. Select the **[!UICONTROL Rule type]**.
         1. Distribute percentages for each of the channels listed under **[!UICONTROL Name]**, using the **[!UICONTROL Contribution proportion]** column. Ensure total distribution of percentages add up to 100%. 
         1. Additionally you can add for each channel a percentage for **[!UICONTROL Level of confidence]**.

         * Use **[!UICONTROL Clear all]** to clear all input values for the **[!UICONTROL Contribution proportion]** and **[!UICONTROL Level of confidence]** columns.
      1. Select **[!UICONTROL Finish]** to finish you model configuration. Select **[!UICONTROL Back]** to go back to the previous step. Select **[!UICONTROL Cancel]** to cancel the model configuration.







