---
title: Create a model
description: Learn how to create a model in Mix Modeler.
feature: Models
exl-id: e1093c09-1e23-460b-92de-cfb0061112fd
---
# Create a model

To create a model, in the ![Models](/help/assets/icons/FileData.svg) **[!UICONTROL Models]** interface in Mix Modeler, select **[!UICONTROL Open model canvas]**.

To build your custom AI-powered models, the interface provides a step-by-step guided model configuration flow.

1. In the **[!UICONTROL Setup]** step:

   1. Enter your model **[!UICONTROL Name]**, for example `Demo model`. Enter a **[!UICONTROL Description]**, for example `Demo model to explore AI featues of Mix Modeler`.

       ![Model name and description](/help/assets/model-name-description.png)

   1. Select **[!UICONTROL Next]** to continue to the next step. Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Configure]** step:

   1. In the **[!UICONTROL Conversion goal]** section:

       ![Model - conversion step](/help/assets/model-conversion-step.png)

       1. Select a conversion from the **[!UICONTROL Conversion]** dropdown menu. The available conversions are the conversion that you defined as part of [Conversions](../harmonize-data/conversions.md) in [!UICONTROL Harmonized datasets]. For example, **[!UICONTROL Online Conversion]**. 

       1. You can select ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a conversion]** to create a conversion directly from within the model configuration.



   1. In the **[!UICONTROL Marketing touchpoints]** section, you can select one or more marketing touchpoints, corresponding to the marketing touchpoints you defined as part of [Marketing touchpoints](../harmonize-data/marketing-touchpoints.md) in [!UICONTROL Harmonized datasets]. 


      ![Model - marketing touchpoint step](/help/assets/model-marketing-touchpoint-step.png)

      1. Select one or more marketing touchpoint from the **[!UICONTROL Touchpoint include]** dropdown menu.

         * You can use ![CrossSize75](/help/assets/icons/CrossSize75.svg) to remove a touchpoint.
         * You can use **[!UICONTROL Clear all]** to remove all touchpoints.

      1. You can select ![LinkOutLight](/help/assets/icons/LinkOutLight.svg) **[!UICONTROL Create a touchpoint]** to create a marketing touchpoint directly from within the model configuration.

      >[!NOTE]
      >
      >You cannot set up the model with touchpoints that have overlapping data and there must be at least one touchpoint with spend.

   1. By default, a score is generated for all the data in your harmonized view. To only score a subset of the population, define one or more filters using containers in the **[!UICONTROL Eligible data population]** section. 

      ![Model - Eligible data population](/help/assets/model-eligible-data-population-step.png)

       * For each container, define one or more events.

         1. For each event: 

             1. Select a metric or dimension from **[!UICONTROL _Select harmonized field_]**.

             1. Select the appropriate operator: **[!UICONTROL equals]**, **[!UICONTROL not equals]**, **[!UICONTROL less than]**, **[!UICONTROL greater than]**, **[!UICONTROL starts with]**, **[!UICONTROL doesn't start with]**, **[!UICONTROL ends with]**, **[!UICONTROL doesn't end with]**, **[!UICONTROL contains]**, **[!UICONTROL doesn't contain]**, **[!UICONTROL is in]**, or **[!UICONTROL is not in]**.

             1. Enter or select a value at **[!UICONTROL _Enter or select value_]**.

         1. To add an additional event in the container, select ![Add](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add event]**.

         1. To remove an event from the container, select ![Close](/help/assets/icons/CrossSize75.svg).

         1. To filter using all or any of multiple events defined in the container, select **[!UICONTROL Any of]** or **[!UICONTROL All of]**. The label correspondingly changes from **[!UICONTROL Include ... Or ...]** to **[!UICONTROL Include ... And ...]**.
       
       * To add an eligible data population container, select ![Add](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add eligible population]**.

       * To remove an eligible data population container, within the container, select ![More](/help/assets/icons/More.svg), and select **[!UICONTROL Remove marketing touchpoint]** from the context menu.

         

   1. To add datasets containing external factors to your model, use one or more containers in the **[!UICONTROL External factors dataset]** section. An example of external factors are S&P indices. 

      ![Model - External factors dataset](/help/assets/model-external-factors-dataset-step.png)

       * For each container:

         1. Enter a **[!UICONTROL External factor name]**, for example `External Factors`.

         1. Select a dataset from the **[!UICONTROL Dataset]** dropdown menu. You can select ![Data](/help/assets/icons/Data.svg) to manage datasets. See [Datasets](../ingest-data/datasets.md) for more information.

         1. Select an option from the **[!UICONTROL Impact on conversion]** dropdown menu: **[!UICONTROL Auto select]**, **[!UICONTROL Positive]** or **[!UICONTROL Negative]**.

       * To add an additional external factors dataset container, select ![Add](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add external factor]**.

       * To remove an external factors dataset container, select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg).

         


   1. To add datasets containing internal factors to your model, use one or more containers in the **[!UICONTROL Internal factors dataset]** section. An example of internal factors are email marketing data.

      ![Model - Internal factors dataset](/help/assets/model-internal-factors-dataset-step.png)

       * For each container:

         1. Enter a **[!UICONTROL Internal factor name]**, for example `Email Marketing Data`.

         1. Select a dataset from **[!UICONTROL _Select a dataset_]**. You can select ![Data](/help/assets/icons/Data.svg) to manage datasets. See [Datasets](../ingest-data/datasets.md) for more information.

         1. Select an option from the **[!UICONTROL Impact on conversion]** dropdown menu: **[!UICONTROL Auto select]**, **[!UICONTROL Positive]** or **[!UICONTROL Negative]**.

       * To add an additional internal factors dataset container, select ![Add](/help/assets/icons/AddCircle.svg) **[!UICONTROL Add internal factor]**.

       * To remove an internal factors dataset container, select ![RemoveCircle](/help/assets/icons/RemoveCircle.svg).

         

   1. To define the lookback window for the model, enter a value between `1` and `52` in **[!UICONTROL Give contribution credit to touchpoints occurring within]** ... **[!UICONTROL weeks prior to the conversion]**.

   1. Select **[!UICONTROL Next]** to continue to the next step. If more configuration is needed, a red outline and text explains what additional configuration is required. <br/>Select **[!UICONTROL Back]** to go back to the previous step. <br/>Select **[!UICONTROL Cancel]** to cancel the model configuration.

1. In the **[!UICONTROL Advanced]** step:

   1. In the **[!UICONTROL Define training window]** section, select between 

       * **[!UICONTROL Have Mix Modeler select a helpful training window]** and 

       * **[!UICONTROL Manually input a training window]**. When selected, define the number of years in **[!UICONTROL Include events the following years prior to a conversion]**.

         ![Model - Define training window](/help/assets/model-define-training-window.png)

   1. In the **[!UICONTROL Spend share]** section:

       * To use historical marketing investment ratios to inform the model when marketing data is sparse, activate **[!UICONTROL Allow spend share]**.

   1. In the **[!UICONTROL MTA enabled]** section:

       * To enable MTA features for the created mode, active **[!UICONTROL MTA enabled]**. Once enabled, 

   1. In the **[!UICONTROL Prior knowledge]** section:

      ![Model - Prior knowledge](/help/assets/model-prior-knowledge-step.png)

       1. Select the **[!UICONTROL Rule type]**, which is by default **[!UICONTROL Absolute values]**.

       1. Specify contribution percentages for any of the channels listed under **[!UICONTROL Name]**, using the **[!UICONTROL Contribution proportion]** column. 

       1. Where appropriate, you can add for each channel a **[!UICONTROL Level of confidence]** percentage.

       1. When needed, use **[!UICONTROL Clear all]** to clear all input values for the **[!UICONTROL Contribution proportion]** and **[!UICONTROL Level of confidence]** columns.

          

1. Select **[!UICONTROL Finish]** to finish your model configuration. 
   
   * In the **[!UICONTROL Create instance?]** dialog, select **[!UICONTROL Ok]** to trigger the first set of training and scoring runs immediately. Your model is listed with status ![StatusOrange](/help/assets/icons/StatusOrange.svg) **[!UICONTROL Awaiting training]**.
   
     Select **[!UICONTROL Cancel]** to cancel. 
  
   * If more configuration is needed, a red outline and text explains what additional configuration is required. 
   
   Select **[!UICONTROL Back]** to go back to the previous step. 
   
   Select **[!UICONTROL Cancel]** to cancel the model configuration.
