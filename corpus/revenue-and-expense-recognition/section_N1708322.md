---
id: "section_N1708322"
type: "section"
title: "Understanding Revenue Commitment Fields"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Commitments > Creating Revenue Commitments > Understanding Revenue Commitment Fields"
parent: "section_N1707026"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1708322.html"
anchors: ["bridgehead_N1708496", "bridgehead_N1708516", "bridgehead_N1708574", "bridgehead_N1708967", "bridgehead_N1708980", "bridgehead_N1709002"]
sha256: "39c67532d1dc9c4c89095eb907c8c45909e698621a86286ae36318b057955480"
---

Important:

The functions discussed in this topic require the Revenue Commitments feature to be enabled.

By default, one field related to revenue commitment displays in the Revenue section of the Accounting subtab, the Rev Rec on Rev Commit. box. After you select this option, other fields become available. NetSuite displays the Accounting subtab on the following transaction forms:

-   Cash Sale
    
-   Credit Memo
    
-   Invoice
    
-   Refund
    
-   Revenue Commitment
    
-   Revenue Commitment Reversal
    
-   Sales Order
    

The following fields may be available under Revenue on the Accounting subtab:

-   [Rev Rec on Rev Commit.](#bridgehead_N1708496)
    
-   [Revenue Status](#bridgehead_N1708516)
    
-   [Rev. Commit. Status](#bridgehead_N1708574)
    
-   [Recognized Revenue](#bridgehead_N1708967)
    
-   [Deferred Revenue](#bridgehead_N1708980)
    
-   [Discounts and Subtotals](#bridgehead_N1709002)
    
-   Transaction is VSOE Bundle - For information about this field, see [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html).
    

## Rev Rec on Rev Commit. {#bridgehead_N1708496}

This field displays Yes or No to indicate whether revenue on this transaction is recognized using a revenue commitment or an invoice. When creating a sales order, this item on the Accounting subtab initially appears as an unchecked box. You can use form customization to set the default value.

If it's an intercompany transaction and Rev Rec on Rev Commit. box is checked, the deferred revenue account for all items must support intercompany elimination. To support intercompany elimination, make sure the Eliminate Intercompany Transactions box on the account is checked.

## Revenue Status {#bridgehead_N1708516}

The Revenue Status field can display the following values:

-   **Pending** - No revenue recognition has occurred, therefore all revenue remains deferred.
    
-   **In Progress** - Some revenue recognition has occurred.
    
-   **Completed** - All revenue recognition has occurred, leaving no deferred revenue.
    

If you cancel or manually close a sales order before recognizing revenue for all items on the order, the status would be based on the status of the transaction at the time. For example, if you had a sales order with an amount of $100, but closed it after only recognizing $80, then the status would be In Progress. In this case, you should use a return authorization and revenue commitment reversal to offset the full amount of the sales order and the revenue commitment.

NetSuite displays this field if the Revenue Recognition feature is enabled. The field doesn't require the Revenue Commitments feature to be enabled.

## Rev. Commit. Status {#bridgehead_N1708574}

The Rev. Commit. Status field can display the following values:

-   **Pending Commitment** - No revenue commitments created.
    
-   **Partially Committed** - Some revenue commitments created.
    
-   **Committed** - All revenue commitments created.
    

Important:

The status NetSuite displays depends on the status of invoices, as well as revenue commitments. If the **Rec Rev on Rev Commit** box on a sales order isn't checked, the **Rev. Commit. Status** is based on the partial or fully completed status of the invoices for the sales order. In this situation, the invoice becomes the revenue commitment document.

## Recognized Revenue {#bridgehead_N1708967}

The cumulative dollar amount of the revenue recognized with either invoices or revenue commitments. NetSuite displays this field if the Revenue Recognition feature is enabled. The field doesn't require the Revenue Commitments feature to be enabled.

## Deferred Revenue {#bridgehead_N1708980}

The cumulative dollar amount of the revenue deferred with either invoices or revenue commitments. Revenue is deferred by using revenue recognition schedules. For more information, refer to [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html).

## Discounts and Subtotals {#bridgehead_N1709002}

Discounts and subtotals on revenue commitments work like they do on invoices with the **Convert Absolute Discounts to Percentage** preference enabled (Setup > Accounting Preferences > Order Management > Invoicing). NetSuite automatically converts absolute discounts to percentages when it copies lines from a sales order or return authorization to a revenue commitment or revenue commitment reversal. This means that if you partially commit, the discount will be proportionately applied. It also means that in certain cases the number may change slightly due to rounding.

For example, consider a sales order with the following lines:

| Line | Item | Amount |
| --- | --- | --- |
| 1 | 19' Monitor | $250 |
| 2 | Discount | $(50) |
|  | Sub-total | $200 |

| Line | Item | Amount |
| --- | --- | --- |
| 1 | 19' Monitor | $250 |
| 2 | Discount | 20% |
|  | Sub-total | $200 |

**Shipping, Handling, Payments, and Tax Items**

Revenue commitments don't display these items, which only appear on invoices.

### Related Topics

-   [Creating Revenue Commitments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707026.html)
-   [Creating a Revenue Commitment from a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707177.html)
-   [Using the Generate Revenue Commitment Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1707431.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
