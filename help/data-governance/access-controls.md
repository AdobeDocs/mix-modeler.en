---
title: Access controls
description: Learn how to configure access controls in Mix Modeler.
feature: Administration
exl-id: c9ec97d9-b9a2-41f5-8626-1cf967d5d7fe
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
