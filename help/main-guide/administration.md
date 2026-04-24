---
title: Administration
description: Learn how to administer Mix Modeler.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
TQID: https://experienceleague.adobe.com/0MxMv6Due-i9-8JxKTb3vk2NDZ5mc6Pj4yEe-liCszg
product_v2:
  - id: b88c80e3-31df-4609-989d-d4dac0e6d973
    internal-label: Mix Modeler
feature_v2:
  - id: e0abf868-dae2-4c1c-83e9-b21799232845
    internal-label: Datasets
  - id: f40f1683-8300-4054-aab8-77da06ad63ff
    internal-label: Models
  - id: fe2edbb1-46f9-4347-a27c-577cab3640cb
    internal-label: Administration
subfeature_v2:
  - id: a567f0f7-0057-4079-8ded-5b24cc25af15
    internal-label: Harmonized Data
  - id: d822825b-9821-40d5-9b0d-42a9e3f317c5
    internal-label: Plans
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: b23e006f-0a29-4f1d-8fd0-77aa56f3d12b
    internal-label: Data modeling
  - id: ebde5b41-29c9-4f5e-9ef6-1197e85409e3
    internal-label: Data management
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
  - id: f4e6943a-c91a-4134-a2c7-f4f20cfff2f0
    internal-label: Privacy
---
# Administration

Use the [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html) to manage Mix Modeler products and users.

For Mix Modeler to function properly, you must set the correct permissions.

In the Adobe Experience Cloud UI: 

1. Select **[!UICONTROL Permissions]** from the left rail, underneath **[!UICONTROL ADMINISTRATION]**.

1. Select ![User](/help/assets/icons/User.svg) **[!UICONTROL Roles]** from the left panel.

1. Select an existing role, or create a role using **[!UICONTROL Create role]** (for example, **Mix Modeler**). If you select an existing role, select ![Edit](/help/assets/icons/Edit.svg) **[!UICONTROL Edit]** to edit the permissions for the role. See [Manage Roles](https://helpx.adobe.com/enterprise/using/admin-console.html) for more information.

1. Ensure you have selected one or more sandboxes for the role.
   
1. Add the **Adobe Mix Modeler** resource to the list of resources for the role.

1. Ensure you select the correct **[!UICONTROL Adobe Mix Modeler]** permissions for the role you are configuring. You can select one or more of the following roles:

    - **[!UICONTROL View Adobe Mix Modeler Harmonized Data]**
    - **[!UICONTROL Manage Adobe Mix Modeler Harmonized Data]**
    - **[!UICONTROL View Adobe Mix Modeler Models Configuration]**
    - **[!UICONTROL Manage Adobe Mix Modeler Models Configuration]**
    - **[!UICONTROL View Adobe Mix Modeler Plans Configuration]**
    - **[!UICONTROL Manage Adobe Mix Modeler Plans Configuration]**

      ![Mix Modeler RBAC](/help/assets/mix-modeler-rbac.png)


1. Ensure you select additional permissions for the role. For example, to view or manage datasets and schemas, you would select:

    - **[!UICONTROL Data Management]**: select the relevant options: **[!UICONTROL View Datasets]** or **[!UICONTROL Manage Datasets]**.

    - **[!UICONTROL Data Modeling]**: select the relevant options: **[!UICONTROL Manage Schemas]** or **[!UICONTROL View Schemas]**.

    <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    --> 

    <!--![Permissions](assets/permissions-including-privacy.png)-->

    Select **[!UICONTROL Save]** to save the permissions.

1. In **[!UICONTROL Details]** within **[!UICONTROL Role]**, add the appropriate **[!UICONTROL Users]** or **[!UICONTROL User groups]** to provide users access to Mix Modeler.
