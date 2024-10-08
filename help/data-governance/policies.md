---
title: Policies
description: Learn how to access policies from Mix Modeler.
feature: Administration
exl-id: 4dba7c30-ad1e-4213-a2b0-afc55f2448a3
---
# Policies

Once you go through the workflow to create a model and submit the model's configuration, [policy enforcement](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/enforcement/overview#automatic-enforcement) checks to see if there are any violations. If a policy violation occurs, a popover appears indicating that one or more policies have been violated. This check is to ensure that your data operations and marketing actions within Experience Platform are compliant with data usage policies.

By default, Mix Modeler checks for violations of Adobe defined policies associated with the following labels and marketing actions:

| Policy name | Associated label | Associated marketing action |
|---|---|---|
| Restrict usage analytics and user based measurement | C8 | Analytics |
| Restrict data science | C9 | Data Science |
| Restrict data export | C12 | Data Export |

Violations are also checked for the policies that you have defined yourself, and that do contain any marketing actions listed in the table above.

When violating a policy while building a dataset rule, you see a popover that displays information about the policy violation.

For example:

- you have enabled the [!UICONTROL Restrict data science] policy with associated label [!UICONTROL C9] and associated marketing action [!UICONTROL Data Science],
- you have applied the [!UICONTROL C9] - [!UICONTROL No data science] label to the `totalCost` field in your Conversion Data schema,
- you want to set up a dataset rule that, amongst others, maps the `totalCost` field of the Conversion Data schema to the harmonized field with name `spend` (and display name `Spend`).

When you want to save the dataset rule, you see a **[!UICONTROL Data governance policy violation detected]** popup, displaying a list of polices violated. When you select the policy name, in the [!UICONTROL Violation summary], you see a list of the [!UICONTROL Active data governance labels], containing [!UICONTROL Entity], [!UICONTROL Type], [!UICONTROL Field] and [!UICONTROL Government labels] applied.

<!-- pending screenshot -->

When applying a data usage label to a schema field that is already used in harmonized data, you see a popover that displays information about the policy violation.

For example:

- you have set up dataset rule that, amongst others, maps the `totalCost` field of your Conversion Data schema to the harmonized field with name `spend` (and display name `Spend`).
- you have synced the harmonized data successfully at least once (see [Dataset rules - Sync data](/help/harmonize-data/dataset-rules.md#sync-data)).
- you enable the [!UICONTROL Restrict data science] policy with associated label [!UICONTROL C9] and associated marketing action [!UICONTROL Data Science],
- you want to apply the [!UICONTROL C9] - [!UICONTROL No data science] label to the `totalCost` field in your Conversion Data schema. 

When you want to save your schema update, you see a **[!UICONTROL Data governance policy violation detected]** popup, displaying a list of polices violated. Select the policy name in the [!UICONTROL Violation summary] to find more details in the [!UICONTROL Data Lineage] list.

<!-- pending screenshot -->

## Violation detected popovers

The data governance policy violation detected popovers provide specific information about the violation. You can resolve these violations through policy settings and other measures that aren't directly related to the configuration workflow. For example, you could change the labels so that certain fields are allowed to use for data science purposes. Alternatively, you could also modify the model configuration itself, so that the model doesn't use an object with a data usage label.

The ![Privacy](/help/assets/icons/Privacy.svg) **[!UICONTROL Policies]** selection in the left rail provides access to the [!UICONTROL Policies] interface of Experience Platform, allowing to manage your policies, labels and marketing actions.

<!--
Currently,  Mix Modeler does not support all of the data governance functionality offered by Experience Platform. Field level access control is supported. See [Field level access control](../harmonize-data/dataset-rules.md#field-level-access-control)
-->

>[!MORELIKETHIS]
>
>[Data usage policies overview](https://experienceleague.adobe.com/en/docs/experience-platform/data-governance/policies/overview)
>
>

