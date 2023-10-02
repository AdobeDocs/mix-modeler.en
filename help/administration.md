---
title: Administration
description: Learn how to administer Mix Modeler.
feature: Administration
exl-id: 76d6d15d-a838-4ee2-9929-e55ea8946b80
---
# Administration

Use the [Adobe Admin Console](https://helpx.adobe.com/enterprise/using/admin-console.html) to manage Mix Modeler products and users.

For Mix Modeler to function properly, you must set the correct permissions.

In the Adobe Experience Cloud UI, 

1. Select **[!UICONTROL Permissions]** from the left rail, underneath **[!UICONTROL ADMINISTRATION]**.

1. Select ![Person](assets/icons/User.svg) **[!UICONTROL Roles]** from the left panel.

1. Select an existing role, or create a role using **[!UICONTROL Create role]**. If you select an existing role, select ![Edit](assets/icons/Edit.svg) **[!UICONTROL Edit]** to edit the permissions for the role. See [Manage Roles](https://helpx.adobe.com/enterprise/using/admin-console.html) for more information.

1. Ensure you select the following permissions for the role:

    * **[!UICONTROL Sandboxes]**: Select at least one sandbox.

    * **[!UICONTROL Data Management]**: ensure you select the options **[!UICONTROL View Datasets]** and **[!UICONTROL Manage Datasets]**.

    * **[!UICONTROL Data Modeling]**: ensure you select the options **[!UICONTROL Manage Schemas]** and **[!UICONTROL View Schemas]**.

    * **[!UICONTROL Destinations]**: ensure you select **[!UICONTROL Manage and Activate Dataset Destination]**, **[!UICONTROL Destination Authoring]**, **[!UICONTROL Activate Destinations]** and **[!UICONTROL View Destinations]**.

    * **[!UICONTROL Data Ingestion]**: ensure you select **[!UICONTROL View Sources]** and **[!UICONTROL Manage Sources]**.

    <!--
    * **[!UICONTROL Data Governance]**: ensure you select **[!UICONTROL View User Activity Log]** and **[!UICONTROL View Data Usage Policies]**.
    --> 

    The permissions set up for the role should look like:

    ![Permissions](assets/permissions.png)

    <!--![Permissions](assets/permissions-including-privacy.png)-->

    Select **[!UICONTROL Save]** to save the permissions.

1. In **[!UICONTROL Details]** within **[!UICONTROL Role]**, add the appropriate **[!UICONTROL Users]** and/or **[!UICONTROL User groups]** to provide users access to Mix Modeler.
