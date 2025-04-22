---
title: Audit logs
description: Learn how to access audit logs from Mix Modeler.
feature: Administration
exl-id: aa65aac5-bea4-43ff-b0d0-9e8a6a97d3ca
---
# Audit logs

To increase the transparency and visibility of activities performed in the system, user activity within the Mix Modeler workflow is captured in Experience Platform audit logs to understand any user-driven changes to Mix Modeler categories. These logs form an audit trail that can help with troubleshooting issues, and can help your business effectively comply with corporate data stewardship policies and regulatory requirements.  

<!-- DO WE HAVE TO ADD THIS
If you are subject to the Health Insurance Portability and Accountability Act (HIPAA) and create, receive, maintain, or transmit permitted sensitive personal data through Mix Modeler, you are responsible for executing a BAA with Adobe and licensing Healthcare Shield.
-->

Ann audit log informs who performed what action, and when. Each action recorded in a log contains metadata that indicates the action type, date and time, the email ID of the user who performed the action, and additional attributes relevant to the action type. It tracks the create, update, and delete actions taken by users in Mix Modeler.

To inspect the audit log, in the Mix Modeler interface:

1. Select ![Task List](/help/assets/icons/TaskList.svg) **[!UICONTROL Audits]** from **[!UICONTROL PRIVACY]**.

1. In **[!UICONTROL Audits]**, you can find the **[!UICONTROL Activity log]**. The Activity log shows entries for the following Mix Modeler categories, actions and status. 

   | Category | Action | Status |
   |---|---|---|
   | Mix Modeler Dataset Rule | Create | Allow or Deny |
   | Mix Modeler Dataset Rule | Update | Allow or Deny |
   | Mix Modeler Dataset Rule | Delete | Allow or Deny |
   | Mix Modeler Field | Create | Allow or Deny |
   | Mix Modeler Field | Update | Allow or Deny |
   | Mix Modeler Field | Delete | Allow or Deny |
   | Mix Modeler Marketing Touchpoint | Create | Allow or Deny |
   | Mix Modeler Marketing Touchpoint | Update | Allow or Deny |
   | Mix Modeler Marketing Touchpoint | Delete | Allow or Deny |
   | Mix Modeler Conversion | Create | Allow or Deny |
   | Mix Modeler Conversion | Update | Allow or Deny |
   | Mix Modeler Conversion | Delete | Allow or Deny |
   | Mix Modeler Model | Create | Allow or Deny |
   | Mix Modeler Model | Update | Allow or Deny |
   | Mix Modeler Model | Delete | Allow or Deny |
   | Mix Modeler Model | Rescore | Allow or Deny |
   | Mix Modeler Model | Clone | Allow or Deny |
   | Mix Modeler Model | Train / Retrain | Allow or Deny |
   | Mix Modeler Model | Download / Save metadata | Allow or Deny |
   | Mix Modeler Plan | Create | Allow or Deny |
   | Mix Modeler Plan | Update | Allow or Deny |
   | Mix Modeler Plan | Change associated model | Allow or Deny | 
   | Mix Modeler Data Harmonization |Trigger Sync | Allow or Deny | 


1. Select an entry in the Activity log to open a panel for more details.

   ![Mix Modeler Audit](/help/assets/mix-modeler-audit.png)

1. To filter on **[!UICONTROL Category]**, **[!UICONTROL Action]**, **[!UICONTROL Request ID]**, **[!UICONTROL User]**, **[!UICONTROL Status]** or **[!UICONTROL Date]** range, select ![Filter](/help/assets/icons/Filter.svg).

1. To modify the columns displayed in the Activity log, select ![Columns](/help/assets/icons/ColumnSetting.svg) and in the **[!UICONTROL Customize table]** dialog select the columns to show. Select **[!UICONTROL Apply]** to apply the selection, **[!UICONTROL Cancel]** to cancel the selection.

1. To download the audit log, select ![Download](/help/assets/icons/Download.svg) **[!UICONTROL Download log]**. In the **[!UICONTROL Download log]** dialog, select either **[!UICONTROL CSV]** or **[!UICONTROL JSON]** as the format and select **[!UICONTROL Download]**.

## Access to audit logs

When the feature is enabled for your organization, audit logs are automatically collected as activity occurs. You do not need to enable audit log collection manually.

To view and export audit logs, you must have been granted the Audit Logs Access access control permission. To learn how to manage individual permissions for Mix Modeler features, see the [access control documentation](https://experienceleague.adobe.com/en/docs/experience-platform/access-control/home).
