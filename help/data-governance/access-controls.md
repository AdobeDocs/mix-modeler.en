---
title: Access controls
description: Learn how to configure access controls in Mix Modeler.
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
TQID: https://experienceleague.adobe.com/EoiF5ui2Bqq0Oxuv-s5E5pQclj9gnjoKgZ1bOzRK-vY
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Mix Modeler
feature_v2:
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized Data
  - id: ba4fd72c-282e-4fb6-abc1-08e6fb87b2ad
    internal-label: Dataset Rules
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
    internal-label: Metadata
  - id: c7d04a2c-412a-4c9d-9d7a-4456eaa5adeb
    internal-label: Governance
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
---
# Access controls

Access control for Mix Modeler is provided through Experience Platform in the [Adobe Admin Console](https://adminconsole.adobe.com/) and through [Permissions](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home#platform-permissions) in Experience Platform. This functionality leverages product profiles in the Admin Console, which link users with permissions and sandboxes.

For more information on access control, see [Access control overview](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home).

## Role-based access control

See [Administration](../main-guide/administration.md) on how to configure role-based access permissions for Mix Modeler users and user groups in Experience Platform.

## Attribute-based access control

[Attribute-based access control](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) is a capability of Experience Platform that enables administrators to control access to specific objects and/or capabilities based on attributes. Attributes can be metadata added to an object, such as a label added to a schema field or segment. An administrator defines access policies that include attributes to manage user access permissions.

This functionality allows you to label Experience Data Model (XDM) schema fields with labels that define organizational or data usage scopes. In parallel, administrators can use the user and role administration interface to define access policies on XDM schema fields. And better manage the access given to users or groups of users (internal, external, or third-party users). Additionally, attribute-based access control allows administrators to manage access to specific segments.

Through attribute-based access control, administrators can control users' access to both sensitive personal data (SPD) and personally identifiable information (PII) across all Platform workflows and resources. Administrators can define user roles that have access only to specific fields and data that corresponds to those fields.

When configuring dataset rules for harmonized datasets, Experience Platform's [attribute based access control](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/abac/overview) is enforced on a field-level. A field is restricted when a label is attached to a schema field. And an active policy is enabled that denies access for you to that field. As a result:

* you do not see the schema fields that are restricted for you when you create a dataset rule, 
* you are not able to view or edit the mapping of one or more schema fields that are restricted for you. When you edit or view a dataset rule containing such restricted fields, you see the following screen.
  ![Action not permitted](/help/assets/action-not-permitted.png)
