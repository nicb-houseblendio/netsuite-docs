---
id: "bridgehead_N1717454"
type: "bridgehead"
title: "Revenue Reclassification Detail Report"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Revenue Reclassification Reports > Revenue Reclassification Detail Report"
parent: "section_N1717186"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1717454.html"
anchors: ["procedure_N1717596"]
sha256: "37c879890bcf321b991a0e4b95d9e2d8b7655fe41900125ead9771262de7a6ef"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

Note:

This report applies only if line level deferred revenue reclassification is disabled for your account. This report isn't available with the Advanced Revenue Management (Essentials) and Advanced Revenue Management (Revenue Allocation) features.

The Revenue Reclassification Detail report shows the detailed history of all related transactions for a sales order including the:

-   period-end revenue recognition journal entries
    
-   billing transactions
    
-   revenue reclassification journal entries
    
-   foreign currency adjustment journal entries
    

The report shows the G/L impact to Revenue, Deferred Revenue, and Unbilled Receivable accounts for each of these transactions. You can aggregate the G/L impact amounts to reconcile to the current balance sheet and income statement balances.

The report shows the following columns:

-   Sales Order - grouped by customer and transaction lines for each order
    
-   Transaction Type
    
-   Line Number
    
-   Transaction Currency
    
-   Base Currency
    
-   Transaction Date
    
-   Billing (Trans Currency)
    
-   Billing (Base Currency)
    
-   Rev Rec (Trans Currency)
    
-   Rev Rec (Base Currency)
    
-   Unbilled Receivables Amount (Base Currency)
    
-   Deferred Revenue Amount (Base Currency)
    

This report doesn't support reporting by period, even if the Report by Period preference is set to All Reports. The Report by Period preference can be configured at _Home > Set Preferences_, the Analytics subtab.

#### To view the Revenue Reclassification Detail: {#procedure_N1717596}

1.  Go to _Reports > Revenue >Revenue Reclassification_.
    
2.  Select **More** to expand the footer.
    
    -   For the **Date, From,** and **To** fields, select a date range that includes the date of the sale order or sales orders you want to run the report for. This is the date the sales order was created. For example, to view revenue reclassification activity for a sales ordered dated 6/15/2012, you must enter a date range that includes 6/15/2012.
        
    -   For the **As of** date, select the ending period date to run the report for. The report returns the revenue reclassification activity through this date. For example, if you select **As of** 06/30/2012, the report shows revenue reclassification activity for the selected sales orders through 6/30/2012. If you enter 10/31/2012, the report shows activity from the sales order date through 10/31/2012.
        
    -   Select a subsidiary in the **Subsidiary Context** field.
        
3.  Click **Refresh**.
    

### Related Reports

-   [Deferred Revenue Reclassification Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3742786017.html)
-   [Deferred Revenue Reclassification Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3742786017.html)
-   [Revenue Reclassification Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1717242.html)

### Related Topics

-   [Revenue Reclassification Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1717186.html)
-   [Drilling Down to Records or Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719130.html)
-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Enhancing Deferred Revenue Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3884444530.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
