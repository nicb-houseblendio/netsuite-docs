---
id: "section_N1502183"
type: "section"
title: "Intercompany Reconciliation Report"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Working with Elimination Reports > Intercompany Reconciliation Report"
parent: "section_N1502129"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502183.html"
anchors: ["procedure_N1502342"]
sha256: "ea1b27ac0ea315ad01f8b50f73c8067d8a0b30b5a77913aa61493c418c30082a"
---

Use the Intercompany Reconciliation report to identify unmatched or incorrectly matched intercompany transactions. This includes intercompany transactions that have not been paired with a corresponding transaction in another subsidiary, and paired transactions that have different amounts or currencies. To produce this report, NetSuite scans all transactions submitted for intercompany customers and vendors including:

-   purchase orders and sales orders
    
-   item fulfillments and item receipts
    
-   vendor bills and invoices
    
-   vendor return authorizations and return authorizations
    
-   vendor credits and credit memos
    
-   customer payments and vendor payments
    

If you use the Multi-Book Accounting feature, you can run the Intercompany Reconciliation report for any accounting book enabled for consolidation.

The Automated Intercompany Management feature automatically generates intercompany elimination journal entries during the period close process. If you use this feature, the intercompany journal form includes an Eliminate box to identify lines to be eliminated. For more information, see [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html).

Before you run elimination for the period, run this report as part of your period end process to identify any problems associated with intercompany transactions. You can then correct the discrepancies to synchronize sales and billing information across subsidiaries before you run intercompany elimination. You can also drill down from the report to edit the source sales and billing transactions, as needed.

Best practices is to run the report periodically to catch problems with transactions before the month end process.

Important:

Run the Intercompany Reconciliation report before you run intercompany elimination. Set the filter for the report for the dates or period you are about to close. Review the transactions listed in each section of the report and determine if you need to make any corrections before running elimination. You can drill down to view the transaction records from the report.

The Intercompany Reconciliation report has five sections and lists the mismatched intercompany transactions for:

1.  **Unlinked Orders and Returns** - intercompany transactions not paired with a corresponding intercompany transaction in another subsidiary
    
    This section includes purchase orders, sales orders, return authorizations and vendor return authorizations.
    
2.  **Mismatched Amount** - paired intercompany transactions with amounts that do not match
    
    This section includes purchase orders, sales orders, return authorizations, and vendor return authorizations.
    
3.  **Mismatched Inventory Item Quantities** - paired intercompany transactions with item quantities that do not match
    
    This section includes only item quantities that do not match. Item rates on paired intercompany inventory orders are always the same.
    
    The **Inventory Item Quantity** columns identify the differences in quantities per item for the following:
    
    -   **Item Fulfillment and Sales Invoice** - the item quantity fulfilled on a sales order is different from the quantity billed on the sales invoice
        
        NetSuite creates the sales invoice from the sales order.
        
    -   **Item Receipt and Vendor Bill** - the item quantity received on a purchase order is different from the quantity on the vendor bill
        
        NetSuite creates the vendor bill from the purchase order.
        
    -   **Item Receipt and Item Fulfillment** - the item quantity fulfilled on a sales order is different from the quantity received for the paired purchase order
        
    
    Note:
    
    The **Inventory Item: Display Name** column displays the **Item's Display Name** for any item that appears in the **Mismatched Inventory Item Quantities** section. If the **Item's Display Name** is blank, the column doesn't display anything.
    
4.  **Mismatched Billing** - paired intercompany transactions with billed amounts that do not match
    
    The amount billed (vendor bill) for the purchase order doesn't match the amount billed (invoice) for a sales order.
    
5.  **Standalone Transactions** - billing and payment transactions that are not associated with a sales order or purchase order
    
    This section includes vendor bills, invoices, credit memos, vendor credits, customer payments, and vendor payments.
    

## To view the Intercompany Reconciliation Report: {#procedure_N1502342}

Go to _Reports > Financial > Intercompany Reconciliation_.

The following filters are available in the report footer:

-   **Date Range** - view results for transactions in a date range
    
    For paired transactions, the results are based on the posting period or date of the purchase order. For unmatched orders, (sales orders not linked to a purchase order), results are based on the sales order date. For stand-alone bills, (bills without referenced purchase order or sales order), the results are based on the date of the invoice, bill, or payment.
    
    Note:
    
    The Period filter is not available for this report because it can include nonposting transactions. To run this report, set your Report by Period preference to Financials Only or Never. See, [Analytics Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html).
    
-   **Subsidiary Context** - view results for all subsidiaries or one subsidiary
    

A message appears indicating that your report is loading. The status bar in the footer of the report indicates the progress as your report loads. You can click Cancel Report next to the status bar to stop the report from loading.

The Intercompany Reconciliation report displays the following columns:

-   Purchasing Subsidiary
    
-   Vendor
    
-   Purchasing Trans - transaction number with drill down to source record
    
-   Purchasing Trans Type - purchase order, return authorization, vendor bill, vendor credit
    
-   Purchasing Trans Date
    
-   Purchasing Trans Currency
    
-   Purchasing Amount - amount is negative for reversed transactions such as return authorizations, credit memos, and refunds
    
-   Purchasing Billed Amount
    
-   Sales Subsidiary
    
-   Customer
    
-   Sales Trans - transaction number with drill down to transaction record
    
-   Sales Trans Type - sales order, invoice, vendor return authorization, credit memo
    
-   Sales Trans Date
    
-   Sales Trans Currency
    
-   Sales Amount - amount is negative for reversed transactions such as vendor return authorizations, bill credit
    
-   Sales Amount Billed
    

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

-   [Intercompany Elimination Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502692.html)
-   [Working with Elimination Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1502129.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
