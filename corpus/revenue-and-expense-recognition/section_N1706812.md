---
id: "section_N1706812"
type: "section"
title: "Billing Additional Items on Orders with Revenue Commitments"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Advanced Revenue Commitments Overview > Billing Additional Items on Orders with Revenue Commitments"
parent: "section_N1703735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1706812.html"
anchors: ["procedure_N1706871"]
sha256: "ec36ffdbce7038f52eb85c25d092c2dfd3fb1f80305389461aa9652a71857873"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

You can add items to an invoice when billing a sales order that has a revenue commitment. This type of billing activity usually occurs for overages on service contracts or other types of billing that need to include charges not covered by the original sales order. All items added directly to an invoice are considered one-time, independent revenue events.

When you add items to an invoice when billing a sales order with a revenue commitment, the revenue for the added items is recognized immediately upon posting the invoice. It's not included with the revenue commitment generated for the items on the invoice that came from the original sales order and doesn't follow a revenue recognition schedule.

On the invoice record, the **Processed by Rev Commit** column identifies which items follow the revenue recognition schedule. All item lines on the invoice that originate from a sales order with a revenue commitment are set to Yes. When you add an additional line to the invoice on the Items subtab, the Processed by Rev Commit column is blank. This indicates that a revenue recognition schedule doesn't apply and that the revenue for this line is booked immediately.

![Screenshot of invoice record, Items subtab, with values in the Processed by Rev Commit column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/revcommitvariant.png)

Items that you enter on the Billable Items, Billable Expense, and Billable Time subtabs of an invoice aren't sourced from a sales order. These items can have a revenue recognition schedule but the Processed by Rev Commit. column will always be blank. These items aren't included in revenue commitments and revenue reclassification.

In addition, if you edit a line on an invoice for a sales order with a revenue commitment and change it to an item not included in the original sales order, the income for the line is recognized immediately upon saving the order. The Processed by Rev Commit. column is left blank.

You can delete all of the line items on an invoice created from a sales order with Rev Rec on Rev Commit. box checked. If you do so, the box, which is read-only on invoices, is automatically cleared by the system.

For a use case example, see [Revenue Commitment with One-Time Revenue Item Example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1712809.html).

The following procedure provides information about how to add an item when billing a sales order with revenue commitment only. For information about creating invoices, see [Billing and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1232486.html).

#### To bill an item not on a sales order with revenue commitment: {#procedure_N1706871}

1.  On a sales order with a revenue commitment that is ready for invoicing, click **Next Bill**.
    
2.  Verify the information in Primary Information is correct or make changes as needed.
    
3.  On the **Items** subtab, enter a new line for the billable item you want to add to the invoice, and click **Add**.
    
4.  Complete the **Billable Items**, **Billable Expenses**, and **Billable Time** subtabs as needed. For more information, see [Deferring Revenue When Billing Costs to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1693662.html).
    
    To generate deferred revenue for billable time, you must manually select revenue recognition schedules on the **Billable Time** subtab.
    
5.  Click **Save**.
    

### Related Topics

-   [Advanced Revenue Commitments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703735.html)
-   [Life Cycle for Sales Order with Revenue Commitment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1703982.html)
-   [Calculating Foreign Currency Adjustment for Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1704597.html)
-   [Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752066884.html)
-   [Adopting Line Level Deferred Revenue Reclassification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3758129615.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
