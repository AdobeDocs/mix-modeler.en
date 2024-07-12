---
title: Administration
description: Learn how to administer Mix Modeler.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
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
