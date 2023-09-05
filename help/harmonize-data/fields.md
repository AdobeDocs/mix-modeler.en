---
title: Harmonized fields
description: Learn how to define fields to use as part of harmonizing your data in Adobe Mix Modeler.
---

# Harmonized fields

Harmonized fields let you define the fields you want to use as part of the harmonize data workflow. The fields you define can be used in defining dataset rules, marketing touchpoints and conversion.

## Global harmonization fields

The global harmonization fields, available by default, in Adobe Mix Modeler are: 


| Field name             | Display name           | Category  | Data Type | Comment   |
| ---------------------- | ---------------------- | --------- | --------- | --------- |
| brand                  | Brand                  | Dimension | String    |           |
| campaign               | Campaign               | Dimension | String    |           |
| channel                | Channel                | Dimension | String    |           |
| channel_id             | Channel ID             | Dimension | String    |           |
| channel_type_at_source | Channel Type At Source | Dimension | String    |           |
| channel                | Channel                | Dimension | String    |           |
| clicks                 | Clicks                 | Metric    | Number    |           |
| conversiontype         | Conversion Type        | Dimension | String    |           |
| cost                   | Cost                   | Metric    | Currency  |           |
| dataset                | Dataset                | Dimension | String    |           |
| date_type              | Date Type              | Dimension | String    | day, week |
| emailssent             | Emails Sent            | Metric    | Number    |           |
| event_date             | Date                   | Dimension | DateTime  |           |
| gross_demand           | Gross Demand           | Metric    | Currency  |           |
| impressions            | Impessions             | Metric    | Number    |           |
| last_updated_date      | Last Updated Date      | Dimension | DateTime  |           |
| linkvisits             | Link Visits            | Metric    | Number    |           |
| mediatype              | Media Type             | Dimension | String    |           |
| net_sales              | Net Sales              | Metric    | Currency  |           |
| orders                 | Orders                 | Metric    | Number    |           |
| sourcetype             | Source Type            | Dimension | String    |           |
| spend                  | Spend                  | Metric    | Currency  |           |
| trafficsource          | Traffice Source        | Dimension | String    |           |

{style="table-layout:auto"}

You can add, edit or delete your own harmonized fields on top of these global harmonized fields.

## Manage harmonized fields

To see a list of the available harmonized fields, in the Adobe Mix Modeler UI:

1. Select ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** from the left rail.
   
1. Select **[!UICONTROL Fields]** from the top bar. You will see a list of the harmonized fields.

1. To search for a specific harmonized field, use ![Search](../assets/icons/Search.svg) **[!UICONTROL *Search harmonized field*]**.

In the list view, columns specify details about the harmonized fields

| Column name            | Details   |
| ---------------------- | ----------|
| Field name             | The name of the harmonized field.  |
| Display name           | The display name of the harmonized field. This display name is used when defining dataset rule, marketing touchpoint and conversion definitions.   |
| Category               | Specifies whether a harmonized data field is a [!UICONTROL Dimension], a [!UICONTROL Metric] or [!UICONTROL Derived]. A derived category is a harmonized field using a metrics based formula definition. |
| Owner                  | Indicates whether a harmonized field is a default one ([!UICONTROL Global]), or is defined by you ([!UICONTROL Client]). |
| Data type              | Specifies the data type ([!UICONTROL Number], [!UICONTROL String], [!UICONTROL Currency], [!UICONTROL DateTime]).  |
| Creation datatime      | Date and time of the creation of the harmonized field. |
| Last modified datetime | Data and time of the last modification of the harmonized field. |
| Formula                | Shows the formula for a harmonized field based on a derived category. |

{style="table-layout:auto"}


### Add a harmonized field

To add a harmonized field, in the ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** UI in the Adobe Mix Modeler:

1. Select ![Add](../assets/icons/AddCircle.svg)Add field.

1. In the **[!UICONTROL Create]** dialog:

    1. Enter a **[!UICONTROL Field name]**, for example `region`.
    1. Enter a **[!UICONTROL Display name]**, for example `Region`.
    1. Select a **[!UICONTROL Category]** from the list: **[!UICONTROL Dimension]**, **[!UICONTROL Metric]** or **[!UICONTROL Derived]**.

       When you select **[!UICONTROL Derived]**, specify a **[!UICONTROL Formula]**:

       Combine one or more metrics from the the **[!UICONTROL Insert Metric]** list with one or more operators **[!UICONTROL + - * / ( )]** to compose a valid arithmetic expression. For example `[orders]/[impressions]`

    1. Select a **[!UICONTROL Data type]**.
       
       - **[!UICONTROL String]** or **[!UICONTROL DateTime]**, when Category selected is Dimension.  
       - **[!UICONTROL Number]** or **[!UICONTROL Currency]** when Categoy selected is Metric or Derived.

    1. Select **[!UICONTROL Submit]** to add the harmonized field. Select Close to close the dialog without adding the harmonized field.


### Edit a harmonized field

You can only edit harmonized fields you created earlier. You cannot edit a global harmonized field.

To edit a harmonized field, in the ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** UI in the Adobe Mix Modeler:

1. Select the harmonized field you want to edit, for example **[!UICONTROL Region]**.

1. In the **[!UICONTROL Edit harmonization values]** pane, modify values for **[!UICONTROL Display name]**, **[!UICONTROL Category]** and **[!UICONTROL Data type]**.

1. Select **[!UICONTROL Submit]** to apply the changes to the harmonized field.

### Delete a harmonized field

You can only delete harmonized fields you created earlier. You cannot delete a global harmonized field.

To delete a harmonized field, in the ![DataSearch](../assets/icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** UI in the Adobe Mix Modeler:

1. Select the harmonized field you want to delete, for example **[!UICONTROL Region]**.

1. Select ![Delete](../assets/icons/Delete.svg) **[!UICONTROL Delete]** from the **[!UICONTROL Edit harmonization values]** left pane.


