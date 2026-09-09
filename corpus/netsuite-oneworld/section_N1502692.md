---
id: "section_N1502692"
type: "section"
title: "Intercompany Elimination Report"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Working with Elimination Reports > Intercompany Elimination Report"
parent: "section_N1502129"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502692.html"
anchors: ["procedure_N1502716"]
sha256: "8d7f7c532bc26e025a8e8a6578be49bee635b68d153e5396e82c52ce2931e557"
---

The Intercompany Elimination report provides an audit trail of intercompany eliminations for a period. Run this report after posting intercompany elimination for a period. This report provides the source transactions marked for elimination, and the generated elimination journal entries.

If you use the Multi-Book Accounting feature, you can run the Intercompany Elimination report for any accounting book enabled for consolidation.

## To view the Intercompany Elimination Report: {#procedure_N1502716}

Go to _Reports > Financial > Intercompany Elimination_.

The following filters are available in the report footer:

-   **Date Range** - view results for transactions in a date range or period range
    
-   **Subsidiary Context** - view results for all subsidiaries or one subsidiary
    
    To filter the report by subsidiary, select an elimination subsidiary with posted elimination journal entries.
    

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

The Intercompany Elimination report displays source transactions and elimination lines. It groups the data by elimination subsidiary, then by sales order and purchase order pair. Source transactions include sales invoice, vendor bill, credit memo, vendor credit, journal entry, advanced intercompany journal entry. Transactions from the same paired transaction are grouped. For example, all invoices and vendor bills that originate from the same sales order, purchase order pair are grouped together.

The Intercompany Elimination report displays the following columns:

-   Source Trans Type
    
-   Subsidiary - the subsidiary where the transaction is created:
    
    -   the selling subsidiary for a sales invoice
        
    -   the purchasing subsidiary for a vendor bill
        
    -   the From subsidiary for an advance intercompany journal entry (AICJE)
        
-   Paired Subsidiary - the subsidiary the transaction targets
    
    the Other subsidiary for AICJE
    
-   Source Trans Date
    
-   Source Trans Account - the account on the source transaction marked for intercompany elimination
    
-   Source Trans Amount (Trans Currency) - source transaction line amount in transaction currency. Shows as positive for a debit, negative for a credit. For A/R and A/P accounts, this is the open balance after month-end revaluation.
    
-   Source Trans Currency
    
-   Source Trans Amount (Base Currency) - source transaction line amount in base currency. Shows as positive for a debit, negative for a credit. For A/R and A/P accounts, this is the open balance after month-end revaluation.
    
-   Subsidiary Base Currency
    
-   Consolidated Exchange Rate - the consolidated exchange rate used to translate the source subsidiary base currency to elimination subsidiary base currency
    
-   Elimination JE - links to the elimination journal entry
    
-   Elimination JE Date
    
-   Elimination JE Amount
    
-   Elimination Subsidiary Currency
    

Important:

On the Intercompany Elimination Report, the Source Trans Amount (Trans Currency) doesn't zero-out.

You can also see the Intercompany Elimination dataset that provides a detailed visibility into intercompany elimination journal entries. For more information, see [Intercompany Elimination Dataset in SuiteAnalytics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1209050543.html).

### Additional Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html)
-   [Graphing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734603.html)
-   [Printing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734828.html)
-   [Emailing a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N734970.html)
-   [Scheduling a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N735311.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html)
-   [Reporting Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N698474.html)

### Related Topics

-   [Intercompany Reconciliation Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502183.html)
-   [Working with Elimination Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502129.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
