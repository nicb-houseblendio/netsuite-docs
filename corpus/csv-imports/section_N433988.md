---
id: "section_N433988"
type: "section"
title: "Budget Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Simple Imports > Budget Import"
parent: "section_N433480"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433988.html"
anchors: ["bridgehead_N434097", "bridgehead_N434174"]
sha256: "57228318b1c28e6eaf6b758f61fd3b98768c18c07264278fadb825324d84c7bb"
---

The Budget Import lets you import your external budget data as NetSuite budget records. The interface and process for budget imports vary from those for other record type imports.

-   A simplified version of the Import Assistant is used for budget imports, with two pages to complete instead of five. This Assistant is available from _Transactions > Financial > Set Up Budgets > Import_ instead of the Setup menu.
    
-   NetSuite provides a CSV budget template file that you download and populate with your data before the import. For details, see [Budget Template File](#bridgehead_N434097) and [Budget Template File Tips](#bridgehead_N434174).
    
-   After you populate a file with your budget data and save it, you select this file in the Assistant. The Assistant automatically maps fields in your budget file to NetSuite budget fields and lets you view these mappings, and change them if necessary. Then click Run to import budget data directly into the database.
    

You can export your NetSuite budget data into an external application, make changes, and then reimport the changed data. To export NetSuite budget data, create a budget search at _Transactions > Financial > Set Up Budgets > Search_, then click Export for the search.

You need the Set Up Budgets permissions to import budget data. You don't need the Import CSV File permission. For questions about permissions, contact your administrator.

For more instructions for completing a budget import, see [Importing a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505717.html).

Note:

Account field values in budget import CSV files can be names, intern,al IDs or external IDs, but can't include account numbers, even if the Use Account Numbers preference is enabled. When using names, values for subaccounts should be hierarchical, with the format parent account name: child account name.

## Budget Template File {#bridgehead_N434097}

The budget template file is available for download at _Transactions > Financial > Set Up Budgets > Import_, when you click **BUDGETS template** in the Import Assistant.

The budget template file includes every field as columns, so that every row of data can store values for fields.

## Budget Template File Tips {#bridgehead_N434174}

Review the following tips for populating a budget CSV file from the template:

-   The year entered on the budget must match the name of the year at _Setup > Accounting > Manage Accounting Periods_.
    
-   Note that the CSV file field mapped to the required Account field should contain account names, internal IDs or external IDs, but not account numbers.
    
    When using names, be sure to only use the name that appears in the Name field on the Account record. If you're entering a line item for a subaccount, the Account field must include the parent account name and subaccount name separated by a colon, for example, **Checking : Purchases**. Use this format for the Account field even if the Use Account Numbers preference is enabled.
    
-   If you use the Multiple Budgets feature, Category is a required field. You can create new categories at _Setup > Accounting > Accounting Lists > New_, by clicking **Budget Category** and entering a budget category name.
    
    Important:
    
    If the Budget Category field isn't mapped during the import, its value defaults to the first budget category on the list. This list is ordered alphabetically.
    
    In OneWorld accounts, each budget category is classified as global or local to support subsidiary-level budgeting in local currencies. You don't have to modify your budget template file to include this global/local classification, because it's associated automatically with the imported budget category.
    

### Related Topics

-   [Simple Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433480.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
