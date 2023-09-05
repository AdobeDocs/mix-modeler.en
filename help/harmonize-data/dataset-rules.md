---
title: Dataset rules
description: Learn how to define dataset rules to use as part of harmonizing your data in Adobe Mix Modeler.
---

# Dataset rules

Dataset rules assist you in mapping your harmonized fields with fields from the data you ingested in Adobe Mix Modeler.

* For aggregate data that you ingested in Adobe Experience Platform, you map one or more of the available dataset fields to the appropriate harmonized fiels. 
* For event data, you can individually map one or more harmonized fields to fields from the dataset, directly or using conditions.


## Manage dataset rules and mappings

To see a list of the available dataset mappings, in the Adobe Mix Modeler UI:

1. Select ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** from the left rail.
   
1. Select **[!UICONTROL Dataset rules]** from the top bar. You will see a list of the dataset mappings.

In the list view, columns specify details about the dataset mappings

| Column name            | Details   |
| ---------------------- | ----------|
| Dataset                | The name of the the dataset.  |
| Source                 | The source of the dataset. Can be Adobe Analytics, Experience Event, Summary (aggregate) or Consumer Experience Event.   |
| Schema                 | The schema on which the dataset is based upon. You can quickly select the schema name to open the schema in a new tab in the schema editor in Adobe Mix Modeler - Schemas.  |
| Granularity            | The granularity of data in the dataset. Possible values are Daily, Weekly, Monthly or Yearly. |
| Start of the week      | Specifies which day of the week is considered the start of a new week for the specific dataset.  |
| Last modified          | Data and time of the last modification of the dataset maping. |

{style="table-layout:auto"}

### Create a dataset mapping

To create a dataset mapping, in the ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Dataset rules]** UI in Adobe Mix Modeler:

1. Select **[!UICONTROL Create Dataset Mapping]**.

1. In the **[!UICONTROL Create]** screen, 
 
   1. Select a dataset to begin configuration from the **[!UICONTROL Select dataset]** list.

   1. Select a day for Start of the week.

   1. Select Daily, Weekly, Monthly or Yearly for Granularity.

   1. When you have selected select a **[!UICONTROL Summary]** type of dataset:
   
      1. Map each of the **[!UICONTROL Available dataset fields]** to corresponding **[!UICONTROL Standard harmonized fields]**. Select a harmonized field from the list, or, if you do not want to map a dataset field to a harmonized field, explicitly select **[!UICONTROL -- None --]** from the list.

      1. If you need a new harmonized field, not available from the list, select **[!UICONTROL Create New]** to create a new harmonized field. You will see the dialog as outlined in [Add a new harmonized field](fields.md#add-a-harmonized-field) to quicly allow you to add a new harmonized field.

      1. When the mapping is complete for all fields, select **[!UICONTROL Save]**. Select **[!UICONTROL Cancel]** to cancel the mapping.
  
   1. When you have selected an event type of dataset, in the shaded box underneath **[!UICONTROL Map to harmonized fields]**:

      1. Select a harmonized field from the **[!UICONTROL Standard harmonized field]** list.
      1. When the selected harmonized field is of type metric:
         1. Select **[!UICONTROL Count]** or **[!UICONTROL Sum]** from the **[!UICONTROL Mapping type]** list.
         1. Select an **[!UICONTROL *AEP dataset field*]** from the list you want the harmonized field to map to by default.
      1. When the selected field is of type dimension:
         1. Select **[!UICONTROL Map Into]** or **[!UICONTROL Case]** from the **[!UICONTROL Mapping type]** list.
         1. When you have selected **[!UICONTROL Map Into]**, select **[!UICONTROL Field]** and **[!UICONTROL *AEP dataset field*]** or **[!UICONTROL Value]**  and a default value to map the harmonized field by default to the dataset field or entered value.
         1. When you have select **[!UICONTROL Case]**, select **[!UICONTROL Field]** and **[!UICONTROL *AEP dataset field*]** or **[!UICONTROL Value]**  and a default value to map the harmonized field by default to the dataset field or entered value. 
            1. Additionally, you define one or more cases, consisting of one or more conditions to explicity set values. Each condition can check for a specific **[!UICONTROL *AEP dataset field*]** whether it **[!UICONTROL Exists]** or **[!UICONTROL Not Exists]** or whether it **[!UICONTROL Contains]**, **[!UICONTROL Not Contains]**, **[!UICONTROL Equals]**, **[!UICONTROL Not Equals]**, **[!UICONTROL Starts With]**, or **[!UICONTROL Ends With]** a value entered at **[!UICONTROL *Enter input value*]**.
            1. To add another case, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add case]**, to add another condition, select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add condition]**.
            1. To delete a case or condition, select ![Close](../assets/icons/Close.svg) in the corresponding container.
            1. To select any of all of the conditions for a case, select **[!UICONTROL All of]** or **[!UICONTROL Any of]**.
            1. To explicitly set the value for a case, enter that value at **[!UICONTROL Then]**.
  
   1. Select ![Add](../assets/icons/AddCircle.svg) **[!UICONTROL Add field]** to define additional fields.
   1. When finished, select **[!UICONTROL Save]** to save the mapping, or select **[!UICONTROL Cancel]** to cancel the mapping.






