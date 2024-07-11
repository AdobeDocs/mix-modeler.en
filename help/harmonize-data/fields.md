---
title: Harmonized fields
description: Learn how to define fields to use as part of harmonizing your data in Mix Modeler.
feature: Harmonized Data, Harmonized Fields
exl-id: f051279a-1ae9-49bd-a946-abfc34c90413
---
# Harmonized fields

Harmonized fields allow you to define fields for conceptually the same data, originating from different sources, each with their own definition of that data. For example, a clicks metric can be defined and named differently depending on the source of data. A clicks harmonized field allows you to define a common nomenclature for a clicks metric based on those different sources of clicks data.

Harmonized fields let you define the fields you want to use as part of the harmonize data workflow. The fields you define can be used in defining dataset rules, marketing touchpoints and conversions.

## Global harmonization fields

The default available global harmonization fields in Mix Modeler are: 


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
| event_date             | Date                   | Dimension | Date time  |           |
| gross_demand           | Gross Demand           | Metric    | Currency  |           |
| impressions            | Impessions             | Metric    | Number    |           |
| last_updated_date      | Last Updated Date      | Dimension | Date time  |           |
| linkvisits             | Link Visits            | Metric    | Number    |           |
| mediatype              | Media Type             | Dimension | String    |           |
| net_sales              | Net Sales              | Metric    | Currency  |           |
| orders                 | Orders                 | Metric    | Number    |           |
| sourcetype             | Source Type            | Dimension | String    |           |
| spend                  | Spend                  | Metric    | Currency  |           |
| trafficsource          | Traffic Source        | Dimension | String    |           |

{style="table-layout:auto"}

You can add, edit, or delete your own harmonized fields on top of these global harmonized fields.

## Manage harmonized fields

To see a table of the available harmonized fields, in the Mix Modeler interface:

1. Select ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** from the left rail.
   
1. Select **[!UICONTROL Fields]** from the top bar. You see a table of the harmonized fields. If more pages are available, use ![Arrow left](/help/assets//icons/ChevronLeft.svg) or ![Arrow Right](/help/assets//icons/ChevronRight.svg) at **[!UICONTROL Page _x_ of _x_]** to move between pages of the table.

   The table columns specify details about the harmonized fields

   | Column name            | Details   |
   | ---------------------- | ----------|
   | Field name             | The name of the harmonized field.  |
   | Display name           | The display name of the harmonized field. This display name is used when defining dataset rules, marketing touchpoint, and conversion definitions.   |
   | Category               | Specifies whether a harmonized data field is a [!UICONTROL Dimension], a [!UICONTROL Metric] or [!UICONTROL Derived]. A derived category is a harmonized field using a metrics-based formula definition. |
   | Data type              | Specifies the data type ([!UICONTROL Number], [!UICONTROL String], [!UICONTROL Currency], [!UICONTROL Date time]).  |
   | Creation date      | Date and time of the creation of the harmonized field. |
   | Owner                  | Indicates whether a harmonized field is a default one ([!UICONTROL Global]), or is defined by you ([!UICONTROL Client]). |
   | Last modified date | Data and time of the last modification of the harmonized field. |
   | Formula                | Specifies the formula for a harmonized field based on a derived category. |

   {style="table-layout:auto"}

1. To search for a specific harmonized field, use ![Search](/help/assets//icons/Search.svg) **[!UICONTROL *Search harmonized field*]**.


### Add a harmonized field

To add a harmonized field, in the ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in the Mix Modeler:

1. Select ![Add](/help/assets//icons/AddCircle.svg) **[!UICONTROL Add field]**.

1. In the **[!UICONTROL Create]** dialog:

    1. Enter a **[!UICONTROL Field name]**, for example `region`.
    1. Enter a **[!UICONTROL Display name]**, for example `Region`.
    1. Select a **[!UICONTROL Category]**: **[!UICONTROL Dimension]**, **[!UICONTROL Metric]** or **[!UICONTROL Derived]**.

       When you select **[!UICONTROL Derived]**, specify a **[!UICONTROL Formula]**. To build a valid arithmetic expression, combine one or more metrics from **[!UICONTROL Insert Metric]** with one or more operators **[!UICONTROL + - * / ( )]** . For example, `[orders]/[impressions]`

    1. Select a **[!UICONTROL Data type]**.
       
       - **[!UICONTROL String]** or **[!UICONTROL Date time]**, when Category selected is Dimension.  
       - **[!UICONTROL Number]** or **[!UICONTROL Currency]** when Category selected is Metric or Derived.

    1. Select **[!UICONTROL Submit]** to add the harmonized field. Select **[!UICONTROL Close]** to close the dialog without adding the harmonized field.

       ![Create a field](/help/assets//create-field.png)


### Edit a harmonized field

You can only edit harmonized fields you created earlier (owner is client). You cannot edit a global harmonized field.

To edit a harmonized field, in the ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in the Mix Modeler:

1. Select the harmonized field that you want to edit. For example, **[!UICONTROL Region]**.

1. In the **[!UICONTROL Edit harmonization values]** pane, modify values for **[!UICONTROL Display name]**, **[!UICONTROL Category]**, and **[!UICONTROL Data type]**. See [Add a harmonized field](#add-a-harmonized-field) for more information.

1. Select **[!UICONTROL Submit]** to apply the changes to the harmonized field.

   ![Edit a field](/help/assets//edit-field.png)

### Delete a harmonized field

You can only delete harmonized fields you created earlier (owner is client). You cannot delete a global harmonized field.

To delete a harmonized field, in the ![DataSearch](/help/assets//icons/DataCheck.svg) **[!UICONTROL Harmonized data]** > **[!UICONTROL Fields]** interface in the Mix Modeler:

1. Select the harmonized field that you want to delete, for example **[!UICONTROL Region]**.

1. Select ![Delete](/help/assets//icons/Delete.svg) **[!UICONTROL Delete]** from the **[!UICONTROL Edit harmonization values]** left pane.

   >[!WARNING]
   >
   >   The field will be deleted immediately.

