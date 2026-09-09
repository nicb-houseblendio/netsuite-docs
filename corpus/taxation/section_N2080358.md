---
id: "section_N2080358"
type: "section"
title: "Creating or Customizing Roles to Use Withholding Tax Features"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Withholding Tax > Creating or Customizing Roles to Use Withholding Tax Features"
parent: "chapter_N2078886"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2080358.html"
anchors: ["bridgehead_N2080500", "bridgehead_N2082475"]
sha256: "3994f2c62163bd8796e3ba53cbbf7f2ceb44c59683d2070841cb6da65426b1cb"
---

Important:

The topics here cover withholding tax for NetSuite accounts without the SuiteTax feature enabled. If you're using an account with SuiteTax enabled, go to [Withholding Taxes in SuiteTax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159646451288.html).

Withholding tax isn't getting new features and reports in accounts without SuiteTax. Updates to the Withholding Tax SuiteApp now include only fixes for reported issues.

By default, the NetSuite withholding tax features are accessible to the following standard roles:

-   Accountant
    
-   Accountant (Reviewer)
    
-   Administrator
    
-   CFO
    

In addition, the Withholding Tax SuiteApp provides the following roles that have already been set up with all the required permissions:

-   Withholding Tax Accountant
    
-   Withholding Tax Accountant (Reviewer)
    
-   Withholding Tax Bookkeeper
    
-   Withholding Tax CFO
    

You can assign these Withholding Tax roles to users for access to withholding tax features, or use them as templates when you create your own customized roles. If you're already using custom roles and want to add permissions to those roles to use the withholding tax features, use the following permission tables for guidance.

Set permissions for a role on the Permissions subtab of the Role record. Permissions are divided into four different types on the Transactions, Reports, Lists, Setup, and Custom Record subtabs.

-   To add a permission, click a line in a list, click **Insert**, and select a permission. You can also click the blank line at the bottom of a list, select a permission, and click **Add**.
    
-   To remove a permission, click it in the list and click **Remove**.
    
-   To set access levels for a permission, click a line in a list and select from the Level column. For information about these levels, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).
    

## To be able to enter withholding tax in transactions {#bridgehead_N2080500}

| Subtab | Permission | Level |
| --- | --- | --- |
| Transactions | Bill | Full |
| Transactions | Cash Sale | Full |
| Transactions | Check | Full |
| Transactions | Credit Memo | Full |
| Transactions | Customer Payment | Full |
| Transactions | Enter Vendor Credits | Full |
| Transactions | Invoice | Full |
| Transactions | Make Journal Entry | Full |
| Transactions | Pay Bills | Full |
| Transactions | Purchase Order | Full |
| Transactions | Sales Order | Full |
| Lists | Accounts | View |
| Lists | Customers | Full |
| Lists | Items | Full |
| Lists | Subsidiaries | View |
| Lists | Tax Records | View |
| Lists | Vendors | Full |
| Lists | Perform Search | View |
| Setup | Accounting Lists | View |
| Setup | Manage Accounting Periods | View |
| Custom Record | Grouped Withholding Tax Code | View |
| Custom Record | Withholding Tax Code | View |
| Custom Record | Withholding Tax Setup | View |
| Custom Record | Withholding Tax Type | View |
| Custom Record | WTax Job | Full |

## To be able to view withholding tax reports (including country-specific reports) {#bridgehead_N2082475}

| Subtab | Permission | Level |
| --- | --- | --- |
| Transactions | Bill | View or Full |
| Transactions | Cash Sale | View or Full |
| Transactions | Check | View or Full |
| Transactions | Credit Memo | View or Full |
| Transactions | Customer Payment | View or Full |
| Transactions | Enter Vendor Credits | View or Full |
| Transactions | Invoice | View or Full |
| Transactions | Make Journal Entry | View or Full |
| Transactions | Pay Bills | View or Full |
| Transactions | Purchase Order | View or Full |
| Transactions | Sales Order | View or Full |
| Lists | Accounts | View |
| Lists | Currency | View |
| Lists | Customers | View |
| Lists | Documents and Files | View |
| Lists | Fiscal Calendars (if your account has the Multiple Calendars feature enabled) | View |
| Lists | Items | View |
| Lists | Subsidiaries | View |
| Lists | Tax Records | View |
| Lists | Vendors | View |
| Setup | Accounting Lists | View |
| Setup | Manage Tax Reporting Periods | Full |
| Setup | Set Up Company | Full |
| Custom Record | Company Information Loader | Full |
| Custom Record | Grouped Withholding Tax Code | View |
| Custom Record | Withholding Tax Code | View |
| Custom Record | Withholding Tax Setup | View |
| Custom Record | Withholding Tax Type | View |
| Custom Record | WTax Journal Type | Full |
| Custom Record | WTax Cache | Full |

### Additional Information

-   [NetSuite Users & Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N284861.html)
-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)
-   [NetSuite Permissions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N325094.html)

### Related Topics

-   [Withholding Tax Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079416.html)
-   [Setting Up Withholding Tax](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2079716.html)
-   [Setting Default Withholding Tax Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085546.html)
-   [Applying Withholding Taxes on Transactions as a Buyer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2085924.html)
-   [Recording Withholding Taxes on Transactions as a Seller](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2087219.html)
-   [Importing Withholding Tax Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4606135691.html)
-   [Withholding Tax Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2088848.html)
-   [Withholding Tax Troubleshooting Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4485199528.html)
-   [Known Limitations of the Withholding Tax SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160458601048.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
