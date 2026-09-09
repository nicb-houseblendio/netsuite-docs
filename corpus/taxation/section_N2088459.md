---
id: "section_N2088459"
type: "section"
title: "Importing Withholding Tax Transactions Using CSV Import"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Importing Withholding Tax Transactions > Importing Withholding Tax Transactions Using CSV Import"
parent: "section_4606135691"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088459.html"
anchors: ["procedure_N2088536"]
sha256: "1c33b32f537d17aa65dd547a849455cb5705f165f3ad2e65ff5647f505d4666e"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

You can use the CSV import feature in NetSuite to add or update transactions that have withholding tax. For more information about importing withholding tax transactions in NetSuite, see [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html). When a withholding tax transaction is created or updated using CSV import or by a scheduled script, the transaction's withholding tax is applied on individual line items.

Note:

Before you start the CSV import, you must make sure that withholding tax codes are already set up in NetSuite. For more information, see [Setting Up Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2084484.html). To post withholding tax on payments, you must use the user interface.

#### To add or update transactions with withholding tax: {#procedure_N2088536}

1.  Go to Setup > Import/Export > CSV Import Preferences.
    
2.  Check the box to enable Run Server SuiteScript and Trigger Workflows.
    
3.  Go to Setup > Import/Export > Import CSV Records and follow the steps in the Import Assistant.
    
4.  In Step 1 (Scan & Upload CSV File):
    
    1.  In the **Import Type** field, select **Transactions**.
        
    2.  In the **Record Type** field, select an accrual record type (Vendor Bill or Invoice).
        
    3.  Make sure the appropriate character encoding format is selected.
        
    4.  Choose one file or multiple files to upload.
        
    5.  Select the file or files to upload.
        
    6.  Click **Next**.
        
5.  In Step 2 (Import Options), choose the appropriate data handling option and click **Next**.
    
6.  If you're importing multiple files, complete Step 3 (File Mapping) and click **Next**. If you're importing only one file, the system directs you to Step 4.
    
7.  In Step 4 (Field Mapping):
    
    1.  Provide field mappings for the following fields in the Expense and Item sublists of transactions:
        
        Note:
        
        Withholding Tax columns for the Item sublist are hidden by default. You need to unhide these custom columns so they can be mapped during CSV import. To show the custom columns, go to Customization > Lists, Records, & Fields > Transaction Column Fields. Edit the following Item sublist fields for Withholding Tax. On the **Display** subtab, select **Normal** in the **Display Type** field.
        
        -   Item sublist
            
            -   Withholding Tax Code (by Internal ID)
                
            -   Withholding Tax Rate
                
            -   Withholding Tax Base Amount
                
            -   Withholding Tax Amount
                
        -   Expenses sublist
            
            -   Withholding Tax Code - Expense (by Internal ID)
                
            -   Withholding Tax Rate - Expense
                
            -   Withholding Tax Base Amount - Expense
                
            -   Withholding Tax Amount - Expense
                
        -   Expenses sublist
            
            -   Withholding Tax Code
                
            -   Withholding Tax Rate
                
            -   Withholding Tax Base Amount
                
            -   Withholding Tax Amount
                
    2.  Click **Next**.
        
8.  In Step 5, you can save your settings and run the import.
    

When the withholding tax is posted for sales and purchase transactions, note the values of the amounts displayed in the **Withholding Tax Base** and **Withholding Tax Amount** columns. The values displayed will have a positive or negative numeric value to indicate the withholding tax deductions.

For purchase transactions, the **Withholding Tax Amount** column displays a negative numeric value.

Note:

This applies to both expense and item sublists.

For example, ABC LTD rented an office space for $1000.00. This is subject to 5% withholding tax. When you add the purchase transaction, the values for the withholding tax amounts will be displayed in the CSV template as follows:

| Amount | Withholding Tax Rate | Withholding Tax Base | Withholding Tax Amount |
| --- | --- | --- | --- |
| 1000.00 | 5% | 1000.00 | \-50.00 |

For sales transactions, the **Withholding Tax Base** column displays a negative numeric value.

Note:

This applies only to item sublists.

For example, XYZ INC billed their customer for services rendered. The professional fee is $5000.00 and is subject to 10% withholding tax. When the sales transaction is entered, the values for the withholding tax amounts will be displayed in the CSV template as follows:

| Amount | Withholding Tax Rate | Withholding Tax Base | Withholding Tax Amount |
| --- | --- | --- | --- |
| 5000.00 | 10% | \-5000.00 | 500.00 |

For more information about importing CSV files, read the following topics:

-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
    
-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)
    
-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
    

### Related Topics

-   [Importing Withholding Tax Transactions Using SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4582915835.html)
-   [Withholding Tax Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4605306566.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Creating or Customizing Roles to Use Withholding Tax Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
