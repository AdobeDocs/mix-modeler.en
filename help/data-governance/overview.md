---
title: Data governance
description: Learn how to use the services and tools from Experience Platform that allow you to control your collected experience data. So, you comply with your business practices, legal obligations, and development process.
feature: Administration
exl-id: 87407c29-e158-48bf-bde9-b3c16a16107e
---
# Data governance

The integration between Mix Modeler and Experience Platform provides Mix Modeler with the capabilities to leverage the intrinsic data governance features of Experience Platform. This section of the documentation details the specifics of the data governance features available in Mix Modeler.

Experience Platform Data Governance gives you the ability to control and comprehend your data throughout the journey that data takes through Experience Platform. This journey involves maintaining data quality, data lineage, data cataloging, and much more.

Data usage labels and policies that are created on datasets consumed by Experience Platform surface in the Mix Modeler where appropriate. For example, these labels stop or warn users when deleting datasets that are part of a dataset rule in the harmonized data. Or hide schema fields that are restricted for users when creating a dataset rule.

The data governance integration allows you to manage compliance more efficiently. Data stewards in your organization can set policies to restrict usage. As a result, you can use data that complies with policies defined by data stewards. Read the documentation on [Labels and Policies](https://experienceleague.adobe.com/en/docs/analytics-platform/using/cja-dataviews/data-governance) to learn more.

The following data governance features are available:

| Feature | Details |
|---|---|
| Access controls | Role-based access control and attribute-based (field-level) access control are supported. See [Access controls](access-controls.md) for more information. |
| Audit logs | When users create, update or delete specific Mix Modeler categories, Experience Platform Audit functionality records the activity in the audit logs. See [Audit logs](audit-logs.md) for more information. |
| Policies | As part of the harmonized data workflow, Experience Platform defined policies are enforced. Any violation of data usage labels is reported and displayed to the user. See [Policies](policies.md) for more information. |
| Encryption | All datasets used for input and output of models follow the Experience Platform guidelines. Experience Platform data encryption applies for data at-rest and in-transit. |
| Data hygiene | All datasets used for input and out of models follow the Experience Platform guidelines. Experience Platform provides a set of tools to manage the customer data lifecycle, including the support of different types of data expiration. When you delete a source dataset from Experience Platform, which is used as part of your harmonized data, you are notified. See [Dataset rules](/help/harmonize-data/dataset-rules.md) for more information. |
| Customer Managed Keys | When you have licensed Mix Modeler with the Privacy Security Shield or Healthcare Shield add-on, you can use the Customer Managed Keys capability to leverage Azure Key Vault to bring your own keys via APIs. You have complete management of data being processed within models in Mix Modeler. |
