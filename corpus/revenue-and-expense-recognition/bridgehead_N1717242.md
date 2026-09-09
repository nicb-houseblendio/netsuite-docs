---
id: "bridgehead_N1717242"
type: "bridgehead"
title: "Revenue Reclassification Summary Report"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Revenue Reclassification Reports > Revenue Reclassification Summary Report"
parent: "section_N1717186"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1717242.html"
anchors: ["procedure_N1717346"]
sha256: "2a28468c3d35b14f3dca73593755e50208ca5e9ad958ba0226c2f13eb5ebd119"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

Note:

This report applies only if line level deferred revenue reclassification is disabled for your account. This report isn't available with the Advanced Revenue Management (Essentials) and Advanced Revenue Management (Revenue Allocation) features.

Use this report to provide an audit trail at month end of the revenue reclassification and foreign currency adjustment journal entries that occurred for a time period. The report shows the accumulated billing and revenue recognition amount for each transaction line on a sales order. These transaction events are the source of revenue reclassification and currency adjustment journal entries created. Use this report to see how the journal entries were created based on the accumulated revenue recognition and billing amounts.

The report includes the following columns:

-   Sales Order - grouped by customer and transaction lines for each order
    
-   Transaction Type
    
-   Transaction Currency
    
-   Transaction Date
    
-   Billing (Trans Currency) - the accumulated billing amount as of the date selected for the report
    
-   Billing (Base Currency)
    
-   Rev Rec (Transaction Currency) - the accumulated revenue amount as of the date selected for the report
    
-   Rev Rec (Base Currency)
    
-   Unbilled Receivables Amount (Base Currency)
    
-   Deferred Revenue Amount (Base Currency
    
-   Revenue Posting Amount (Base Currency)
    

You can customize the report to include additional columns such as Total Committed Amount Base Currency, Total Committed Amount Transaction Currency, Deferred Revenue Account, and Revenue Reclassification Account.

This report doesn't support reporting by period, even if the Report by Period preference is set to All Reports. The Report by Period preference can be configured at _Home > Set Preferences_, the Analytics subtab.

#### To view the Revenue Reclassification Summary {#procedure_N1717346}

1.  Go to _Reports > Revenue >Revenue Reclassification_.
    
2.  Select **More** to expand the footer.
    
    -   For the **Date, From,** and **To** fields, select a date range that includes the sales order date. This is the date the sales order was created. For example, to view revenue reclassification activity for a sales ordered dated 6/15/2025, enter a date range that includes 6/15/2025.
        
    -   For the **As of** date, select the ending period date to run the report for. The report returns the revenue reclassification activity through this date. For example, if you select **As of** 06/30/2025, the report shows revenue reclassification activity for the selected sales orders through 6/30/2025. If you enter 7/31/2025, the report shows activity from the sales order date through 7/31/2025.
        
    -   Select a subsidiary in the **Subsidiary Context** field.
        
3.  Click **Refresh**.
    

### Related Reports

-   [Deferred Revenue Reclassification Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3742786017.html)
-   [Deferred Revenue Reclassification Activity Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3742806547.html)
-   [Revenue Reclassification Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1717454.html)

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
