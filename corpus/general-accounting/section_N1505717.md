---
id: "section_N1505717"
type: "section"
title: "Importing a Budget"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Budgets > Budgets in NetSuite > Importing a Budget"
parent: "chapter_N1503165"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505717.html"
anchors: ["procedure_N1505774"]
sha256: "5844bd8fba09707de5b2858815a729dcaedbf6c5f4c1df6b94d1263caacb3751"
---

You can import external applications' budget data as CSV files to create NetSuite budget records.

If you have a budget already in NetSuite, you can copy that budget to a different year. For instructions, see [Copying a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505228.html).

You can use the Import Assistant to import budget data directly into the database. For information, see [Budget Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433988.html) and [Budget Template File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N433988.html#bridgehead_N434097).

Before you begin the import process, ensure that the values in the CSV file are properly formatted.

-   The account name in the CSV file must exactly match the account name in the chart of accounts.
    
-   If there is a subaccount, the account field must include the parent account name and subaccount name, separated by a colon (:). The format should be, Parent : Child Account. The format for subsidiaries should be the same as the format for subaccounts.
    
-   The account name shouldn't contain account numbers.
    
-   If multiple budgets are enabled, category is required.
    
-   The year format in the CSV file must match the year format of the Manage Accounting Periods page **exactly**. If you can't access the page at _Setup > Accounting > Manage G/L > Manage Accounting Periods_, ask your NetSuite administrator to provide the format.
    
-   Numbers for amounts must not contain the separator (,) or the Currency character ($).
    

Important:

Any field in the CSV file that doesn't contain a value appears in the created budget record as blank.

You need the Set Up Budget permission to import budget data. You don't need the Import CSV File permission. For questions about permissions, contact your administrator.

Warning:

Using a CSV file to update an existing budget record **overwrites** all existing budget data. The CSV file you use to update an existing budget **must** contain values in each field or your existing data will be lost.

#### To import a budget: {#procedure_N1505774}

1.  Go to Transactions > Financial > Set Up Budgets > Import.
    
2.  On the Import Assistant page, in the Scan & Upload CSV File section, select the type of character encoding for imported data.
    
    For information about available options, see [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).
    
3.  Click the **Budgets Template File** link to download a template file.
    
4.  Save the file to your system, and then populate the saved file with your budget data. Be aware of the following limitations for CSV file fields:
    
    -   **Year** - Year values should be for years with accounting periods set up at _Setup > Accounting > Manage Accounting Periods_.
        
    -   **Category** - If the Multiple Budgets feature is enabled, **Category** is a required field.
        
        Important:
        
        If the **Budget Category** field is not mapped during the import, its value defaults to the first budget category on the list. This list is ordered alphabetically.
        
        If you use NetSuite OneWorld with the Multiple Currencies feature, the budget category type determines the currency for the budget. Global categories use the root parent's base currency. Categories that are not global use the subsidiary's base currency. See [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html).
        
    -   **Account** - **Account** field values should be names. Don't use numbers even if the Use Account Numbers preference is checked. For subaccounts, values should be hierarchical, with the format `_parent account name_` : `_child account name_`. Be sure to include a space on both sides of the colon.
        
5.  Click **Select**, choose the budget data file you've populated, and then click **Next**.
    
6.  On the View Mapping / Start Import page, review the automappings of CSV file fields to NetSuite fields, and make any necessary changes or additions.
    
    -   Note that the **CSV file** field mapped to the required **Account** field should contain account names, not account numbers. If you have multiple accounts with the same name and different numbers, so that mapping by name doesn't work, use a workaround. For example, you could include a CSV file field containing internal ID values in addition to the **Account** field.
        
    -   For information about Import Assistant field mappings, see [CSV Field Mapping Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N348870.html) and [General CSV Field Mapping Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349148.html).
        
7.  Click **Run** to start the import.
    
    -   For information about the Import Assistant's error handling, see [CSV Import Error Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353446.html).
        
    -   For information about checking import status, see [Checking CSV Import Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350581.html).
        

After the import of budget data has successfully completed, you can review NetSuite budget records by going to the Budgets list page. To open this page, go to _Transactions > Financial > Set Up Budgets > List_. Then click a **View** or **Edit** link to open each budget record.

Note:

If you want to modify existing NetSuite budget data in an external application, you can export the data, make changes, then reimport the changed data. To export NetSuite budget data, create a budget search at _Transactions > Financial > Set Up Budgets > Search_, then click **Export** for the search. To export a budget with amounts by period, use the Budget Income Statement with Column set to Accounting Period in the footers.

### Related Topics

-   [Budgets in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1503165.html)
-   [Setting Up a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1503407.html)
-   [Copying a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1505228.html)
-   [Multiple Budgets and Budget Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506174.html)
-   [Budget-Related Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158801165026.html)
-   [Subsidiary Budgets in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506361.html)
-   [Budgets for Secondary Accounting Books](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1545224080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
