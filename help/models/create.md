---
title: Create a model
description: Learn how to create a model in Adobe Mix Modeler.
---

# Create a model

To create a model, in the ![Models](../assets/icons/FileData.svg) **[!UICONTROL Models]** UI in Adobe Mix Modeler, select **[!UICONTROL Guide me]**.

To build your custom AI-powered models to measure and optimize your paid, owned, and earned marketing investments holistically using the power of Adobe Sensei, the UI provides a step-by-step guided model configuration flow.

1. In the **[!UICONTROL Setup]** step:

   1. Enter your model **[!UICONTROL Name]**, for example `Demo model`. Enter a **[!UICONTROL Description]**, for example `Demo model to explore AI featues of Adobe Mix Modeler`.

       ![Model name and description](../assets/model-name-description.png)

   1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Configure]** step:

   1. In the **[!UICONTROL Conversion goal]** section, within the container:

       1. Enter a **[!UICONTROL Conversion name]** for the conversion, for example `Conversion`

       1. Select a conversion from the **[!UICONTROL *Select harmonized field*]** list, containing the available conversions you as part of [Conversions](../harmonize-data/conversions.md) in [!UICONTROL Harmonized datasets]. For example **[!UICONTROL Online Conversion]**. 

       1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new conversion]** to create a new conversion directly from within the model configuration.

            ![Model - conversion step](../assets/model-conversion-step.png)

   1. In the **[!UICONTROL Marketing touchpoints]** section, you see a list of marketing touchpoint containers, corresponding to the marketing touchpoints defined as part [Marketing touchpoints](../harmonize-data/marketing-touchpoints.md) in [!UICONTROL Harmonized datasets]. 

       * For each container

         1. You can modify the name 

         1. Select a marketing touchpoint from the list.

         1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]** to create a new marketing touchpoint directly from within the model configuration.

       * To add a marketing touchpoint container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**.

       * To remove a marketing touchpoint container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

            ![Model - marketing touchpoints-step](../assets/model-marketing-touchpoint-step.png)

   1. By default, a score will be generated for all the data in your harmonized view. To only score a subset of the population, define one or more filters using containers in the **[!UICONTROL Eligible data population]** section. 

       * For each container, define one or more events.

         1. For each event: 

             1. Select a metric or dimension from the **[!UICONTROL _Select harmonized field_]** list.

             1. Select the appropriate operator from the **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]**, **[!UICONTROL is not in]** list.

             1. Enter or select a value.

         1. To add an additional event in the container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add event]**.

         1. To remove an event from the container, select ![Close](../assets/icons/Close.svg).

         1. To filter using all or any of multiple events defined in the container, select **[!UICONTROL Any of]** or **[!UICONTROL All of]**. The label will correspondingly change from **[!UICONTROL Include ... Or ...]** to **[!UICONTROL Include ... And ...]**.
       
       * To add an eligible data population container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.

       * To remove an eligibile data population container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

         ![Model - Eligible data population](../assets/model-eligible-data-population-step.png)

   1. To add datasets containing external factors to your model, use one or more containers in the **[!UICONTROL External factors dataset]** section. 

       * For each container:

         1. Enter a name.

         1. Select a dataset from the **[!UICONTROL _Select a dataset_]** list.

       * To add an additional external factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**.

       * To remove an external factors dataset container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

         ![Model - External factors dataset](../assets/model-external-factors-dataset-step.png)


   1. To add datasets containing internal factors to your model, use one or more containers in the **[!UICONTROL Internal factors dataset]** section. 

       * For each container:

         1. Enter a name.

         1. Select a dataset from the **[!UICONTROL _Select a dataset_]** list.

       * To add an additional internal factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**.

       * To remove an additional internal factors dataset container, within the container, select ![More](../assets/icons/More.svg) and **[!UICONTROL Remove container]** from the context menu.

         ![Model - Internal factors dataset](../assets/model-internal-factors-dataset-step.png)

   1. To define the lookback window for the model, enter a value between `1` and `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**.

   1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Back]** to go back to the previous step. Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Advanced]** step:

   1. In the **[!UICONTROL Define training window]** section, select between 

       * **[!UICONTROL Have Adobe Mix Modele select a helpful training window]** and 

       * **[!UICONTROL Manually input a training window]** and define the number of years in **[!UICONTROL Include events the following years prior to a conversion]**.

         ![Model - Define training window](../assets/model-define-training-window.png)

   1. In the **[!UICONTROL Spend share]** section:

       * To allow spend share, activate **[!UICONTROL Allow spend share]** . Spend share will utilize historical marketing investment ratios to inform the model when marketing data is sparse.

   1. In the **[!UICONTROL Prior knowledge]** section:

       1. Select the **[!UICONTROL Rule type]**.

       1. Distribute percentages for each of the channels listed under **[!UICONTROL Name]**, using the **[!UICONTROL Contribution proportion]** column. Ensure total distribution of percentages add up to 100%. 

       1. Additionally you can add for each channel a percentage for **[!UICONTROL Level of confidence]**.

       1. When needed, use **[!UICONTROL Clear all]** to clear all input values for the **[!UICONTROL Contribution proportion]** and **[!UICONTROL Level of confidence]** columns.

            ![Model - Prior knowledge](../assets/model-prior-knowledge-step.png)

1. Select **[!UICONTROL Finish]** to finish you model configuration. Select **[!UICONTROL Back]** to go back to the previous step. Select **[!UICONTROL Cancel]** to cancel the model configuration.

