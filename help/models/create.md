---
title: Create a model
description: Learn how to create a model in Adobe Mix Modeler.
---

# Create a model

To create a model, in the ![Models](../assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Adobe Mix Modeler, select **[!UICONTROL Guide me]**.

To build your custom AI-powered models, the interface provides a step-by-step guided model configuration flow.

1. In the **[!UICONTROL Setup]** step:

   1. Enter your model **[!UICONTROL Name]**, for example `Demo model`. Enter a **[!UICONTROL Description]**, for example `Demo model to explore AI featues of Adobe Mix Modeler`.

       ![Model name and description](../assets/model-name-description.png)

   1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Configure]** step:

   1. In the **[!UICONTROL Conversion goal]** section, within the container:

       1. Enter a **[!UICONTROL Conversion name]** for the conversion, for example `Conversion`

       1. Select a conversion from the **[!UICONTROL *Select harmonized field*]** list, containing the available conversions you defined as part of [Conversions](../harmonize-data/conversions.md) in [!UICONTROL Harmonized datasets]. For example, **[!UICONTROL Online Conversion]**. 

       1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new conversion]** to create a conversion directly from within the model configuration.

            ![Model - conversion step](../assets/model-conversion-step.png)

   1. In the **[!UICONTROL Marketing touchpoints]** section, you see a list of marketing touchpoint containers, corresponding to the marketing touchpoints you defined as part of [Marketing touchpoints](../harmonize-data/marketing-touchpoints.md) in [!UICONTROL Harmonized datasets]. 

       * For each container:

         1. You can modify the **[!UICONTROL Marketing touchpoint name]**. 

         1. Select a marketing touchpoint from **[!UICONTROL _Select marketing touchpoint_]**.

         1. You can select ![Reply](../assets/icons/Reply.svg) **[!UICONTROL Create new marketing touchpoint]** to create a marketing touchpoint directly from within the model configuration.

       * To add a marketing touchpoint container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add marketing touchpoint]**.

       * To remove a marketing touchpoint container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

            ![Model - marketing touchpoints-step](../assets/model-marketing-touchpoint-step.png)

   1. By default, a score is generated for all the data in your harmonized view. To only score a subset of the population, define one or more filters using containers in the **[!UICONTROL Eligible data population]** section. 

       * For each container, define one or more events.

         1. For each event: 

             1. Select a metric or dimension from **[!UICONTROL _Select harmonized field_]**.

             1. Select the appropriate operator: **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]**, or **[!UICONTROL is not in]**.

             1. Enter or select a value at **[!UICONTROL _Enter or select value_]**.

         1. To add an additional event in the container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add event]**.

         1. To remove an event from the container, select ![Close](../assets/icons/Close.svg).

         1. To filter using all or any of multiple events defined in the container, select **[!UICONTROL Any of]** or **[!UICONTROL All of]**. The label correspondingly changes from **[!UICONTROL Include ... Or ...]** to **[!UICONTROL Include ... And ...]**.
       
       * To add an eligible data population container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.

       * To remove an eligible data population container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

         ![Model - Eligible data population](../assets/model-eligible-data-population-step.png)

   1. To add datasets containing external factors to your model, use one or more containers in the **[!UICONTROL External factors dataset]** section. 

       * For each container:

         1. Enter a **[!UICONTROL Factor name]** at **[!UICONTROL _Enter factor_]**.

         1. Select a dataset from **[!UICONTROL _Select a dataset_]**. You can select ![Data](../assets/icons/Data.svg) to manage datasets. See [Datasets](../ingest-data/datasets.md) for more information.

       * To add an additional external factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**.

       * To remove an external factors dataset container, within the container, select ![More](../assets/icons/More.svg) and select **[!UICONTROL Remove container]** from the context menu.

         ![Model - External factors dataset](../assets/model-external-factors-dataset-step.png)


   1. To add datasets containing internal factors to your model, use one or more containers in the **[!UICONTROL Internal factors dataset]** section. 

       * For each container:

         1. Enter a **[!UICONTROL Factor name]** at **[!UICONTROL _Enter factor_]**.

         1. Select a dataset from the **[!UICONTROL _Select a dataset_]** list. You can select ![Data](../assets/icons/Data.svg) to manage datasets. See [Datasets](../ingest-data/datasets.md) for more information.

       * To add an additional internal factors dataset container, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**.

       * To remove an additional internal factors dataset container, within the container, select ![More](../assets/icons/More.svg) and **[!UICONTROL Remove container]** from the context menu.

         ![Model - Internal factors dataset](../assets/model-internal-factors-dataset-step.png)

   1. To define the lookback window for the model, enter a value between `1` and `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**.

   1. Select **[!UICONTROL Next]** to continue to the next step. If more configuration is needed, a red outline and text explains what additional configuration is required. <br/>Select **[!UICONTROL Back]** to go back to the previous step. <br/>Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Advanced]** step:

   1. In the **[!UICONTROL Define training window]** section, select between 

       * **[!UICONTROL Have Adobe Mix Modeler select a helpful training window]** and 

       * **[!UICONTROL Manually input a training window]**. When selected, define the number of years in **[!UICONTROL Include events the following years prior to a conversion]**.

         ![Model - Define training window](../assets/model-define-training-window.png)

   1. In the **[!UICONTROL Spend share]** section:

       * To use historical marketing investment ratios to inform the model when marketing data is sparse,  activate **[!UICONTROL Allow spend share]**.

   1. In the **[!UICONTROL Prior knowledge]** section:

       1. Select the **[!UICONTROL Rule type]**.

       1. Distribute percentages for each of the channels listed under **[!UICONTROL Name]**, using the **[!UICONTROL Contribution proportion]** column. Ensure that the total distribution of percentages adds up to 100%. 

       1. You can add for each channel a **[!UICONTROL Level of confidence]** percentage.

       1. When needed, use **[!UICONTROL Clear all]** to clear all input values for the **[!UICONTROL Contribution proportion]** and **[!UICONTROL Level of confidence]** columns.

          ![Model - Prior knowledge](../assets/model-prior-knowledge-step.png)

1. Select **[!UICONTROL Finish]** to finish you model configuration. 
   
   * In the **[!UICONTROL Create instance?]** dialog, select **[!UICONTROL Ok]** to trigger the first set of training and scoring runs immediately. Your model is listed with status <span style="color:orange">●</span> **[!UICONTROL Awaiting training]**.
   
     Select **[!UICONTROL Cancel]** to cancel. 
  
   * If more configuration is needed, a red outline and text explains what additional configuration is required. 
   
   Select **[!UICONTROL Back]** to go back to the previous step. 
   
   Select **[!UICONTROL Cancel]** to cancel the model configuration.

