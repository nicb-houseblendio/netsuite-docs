---
id: "section_N1481077"
type: "section"
title: "GL Impact Page"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > General Ledger Impact of Transactions > GL Impact Page"
parent: "chapter_N1459499"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1481077.html"
anchors: []
sha256: "8a5a1d3d7452f2e67a2e802486789083f7587504ba81b570160369341633462e"
---

You can access the GL Impact page from most transaction records by clicking GL Impact in the Actions list. Most posting transactions also include a GL Impact subtab.

Note:

If you are using NetSuite Next, the GL impact page opens in a tabbed drawer. You can access the GL impact page by clicking general ledger icon ![GLImpactIcon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/GeneralAccounting/GLImpactIcon.png) at the top right corner of the transaction.

If a custom GL plug-in execution is scheduled or in progress, a message is displayed at the top of the GL Impact page to indicate that the GL impact might change.

Note:

For advanced intercompany journal entries, the permissions set for your user role determine what you're able to view and edit. If you don't have access to all the subsidiaries on a record, you can only view data for the subsidiaries to which you have access. In addition, you can't edit or copy the record.

The GL Impact page lists the general ledger or journal impact of lines on the originating transaction. For each transaction line, the following details are displayed, as applicable:

-   Accounting Book (when the Multi-Book Accounting feature is enabled)
    
-   Account affected
    
-   Debited amount
    
-   Credited amount
    
-   Whether the amount posts to the account
    
-   Memo text
    
-   Name of related entity (for example, employee, customer, or vendor)
    
-   (OneWorld only) Hierarchical name of the subsidiary affected by the transaction
    
-   Department
    
-   Class
    
-   Location
    
-   Custom segment
    

For example, the GL Impact page for an invoice could show a debit amount posting to an Accounts Receivable account and a credit amount posting to a merchandise sales account.

Non-posting transactions list debits to the related non-posting registers. Opportunity records do include the GL Impact link.

To return to the source transaction, click the crosslink at the top of the page, for example, Go to Sales Order #SORD1001.

Click the Export button to export GL impact details to a CSV or Excel file.

If the Advanced PDF/HTML Templates feature is enabled, click the **Print** button to create a PDF file containing the GL Impact for the transaction. This PDF can be saved or printed. For more information, see [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html).

For intercompany journal entries, the GL Impact page always uses the class, department, and location used by the subsidiary at the last transaction line that has tax. For information about enabling line-level selection for class, department, and location, see [Using Per-Line Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html).

Note:

For automated intercompany adjustments in a OneWorld account, this page displays amounts debited and credited to accounts in both the originating subsidiary (employee's subsidiary) and the related subsidiary (customer's subsidiary). General ledger impact to the originating subsidiary is in its base currency, the same currency recorded for the adjustment. General ledger impact to the related subsidiary is translated from the originating subsidiary base currency to the related subsidiary base currency, using the exchange rate indicated on the adjustment record. This rate is based on the last day of the period when the adjustment occurred.

SuiteGL features support customization of general ledger processes to meet your specific business needs. With these features, you can modify line-level general ledger impact of transactions, design specialized transaction types with unique GL capabilities, and create customized classifications that improve reporting and analytics. For details, see [SuiteGL Features Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4326823275.html).

### Related Topics

-   [General Ledger Impact of Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1459499.html)
-   [Sales Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1459773.html)
-   [Customer Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1460914.html)
-   [Vendor/Purchase Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1461991.html)
-   [Cost of Goods Sold (COGS) GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1464868.html)
-   [Bank Transaction GL Impact](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1465926.html)
-   [General Ledger Tracking in Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556628.html)
-   [Printing the GL Impact for a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_156215822877.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
