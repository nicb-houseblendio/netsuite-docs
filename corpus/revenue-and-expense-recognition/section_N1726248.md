---
id: "section_N1726248"
type: "section"
title: "Using VSOE with Discount Items"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Using VSOE with Discount Items"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html"
anchors: ["bridgehead_N1726345", "bridgehead_N1726424", "bridgehead_N1727923", "bridgehead_N1728995"]
sha256: "bbaf8814f6aff600f938017329e7c96ee95efb411df61afe70b40e3b9f3ce10c"
---

Discount items can affect vendor-specific objective evidence (VSOE) allocation when they're added to a transaction.

Important:

Use non-posting discount items to ensure that the net amount of each line and the transaction as a whole is amortized correctly.

For information about using VSOE with discount items, see:

-   [Rules for Discounts on VSOE Transactions](#bridgehead_N1726345)
    
-   [VSOE Discount Example](#bridgehead_N1726424)
    
-   [Implicit VSOE Discounts](#bridgehead_N1727923)
    
-   [Implicit Discounts and the Residual Method](#bridgehead_N1728995)
    

## Rules for Discounts on VSOE Transactions {#bridgehead_N1726345}

When a discount is included on a transaction, the discount is applied in a particular way for VSOE processing and affects the amount of revenue recognized by each item. Discount effects on VSOE prices can be different from discount effects on sales amounts.

The following rules apply for discounts on all VSOE transactions:

1.  Discounts are applied proportionately to lines based on their VSOE prices, except when the residual method is applied. See [Implicit Discounts and the Residual Method](#bridgehead_N1728995).
    
2.  A discount is applied to the entire bundle if the discount is added as a line item after an item group on a transaction.
    
3.  If the Permit Discount field on an item record is set to **Never**, then discounts aren't applied to the item, even when the residual method is used. This setting is typically used for specified upgrades.
    
    For more information about this field, read [Setting Up VSOE on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718972.html).
    
4.  If a discount is applied to an entire transaction, instead of a line item, then the transaction can contain a maximum of one bundle. The bundle can be either an item group bundle added as a line, or can be a transaction bundle. If multiple bundles are included on a discounted transaction, the VSOE allocation can't be calculated.
    

NetSuite uses the VSOE settings of items and discounts associated with the bundle to calculate the VSOE allocation for the bundle.

## VSOE Discount Example {#bridgehead_N1726424}

For example, when a transaction meets the following requirements, the **post-discount** sales amount is allocated proportionately to each item based on the VSOE amount for each item:

-   A discount has been applied to the entire bundle.
    
-   All of the items have an assigned VSOE price.
    
-   The total VSOE price of the bundle is greater than the total sales price.
    
-   All items have been delivered.
    

In this example, the sales order is marked Is VSOE Bundle and includes the following:

| Item | VSOE Price | Delivered? | VSOE % | Invoice price | Calculations | VSOE Allocation |
| --- | --- | --- | --- | --- | --- | --- |
| Installation Service 302 | $1,000 | Yes | 18.1817% | $0 | (3,300 x .181817) = 605.45 | $605.45 |
| Software Product 401 | 2,000 | Yes | 36.3637% | $2200 | (3,300 x .363637) =1210.91 | 1,210.91 |
| Software Product 501 | 2,500 | Yes | 45.4547% | 1,500 | (3,300 x .454547) = 1513.64 | 1,513.64 |
| **Subtotal** |  |  | 100.00% | 3,700 |  |  |
| 10% transaction discount |  |  |  | (370) |  |  |
| **Total** | $5,500 |  | 100.00% | $3,330 |  | $3,330.00 |

Note:

If a bundle includes a discount, but no member items permit a discount because they're not delivered or their permit discount setting is Never, then NetSuite doesn't calculate the VSOE allocation when Auto-allocate VSOE is set.

## Implicit VSOE Discounts {#bridgehead_N1727923}

VSOE bundle pricing can reflect a discount even if a transaction discount isn't set or a line item discount added. These implicit discounts occur in cases when the total list price of all elements is less than the total VSOE price for the bundle.

For example, you enter a sales order that shows the following bundle items and a line item discount:

| Item | Invoice price | VSOE Price |
| --- | --- | --- |
| Product 1 | $120 | $120 |
| Product 2 | $120 | $80 |
| Product 3 | $120 | $160 |
| Discount | ($60) |  |
| Total | $300 | $360 |

The $60 line item discount causes the invoice price to be less than the VSOE price, and the discount is allocated to eligible member items, as follows:

| Item | Invoice price | VSOE Price | VSOE Calculation | Allocation |
| --- | --- | --- | --- | --- |
| Product 1 | $100 | $120 | 120/360 x 300 | $100.00 |
| Product 2 | $100 | $80 | 80/360 x 300 | $66.67 |
| Product 3 | $100 | $160 | 120/360 x 300 | $133.33 |
| Discount | allocated to items |  |  |  |
| Total | $300 | $360 |  | $300.00 |

Next, you enter a sales order that shows the following bundle items, but the discount is implicit instead of added as a line item.

| Item | Invoice price | VSOE Price |
| --- | --- | --- |
| Product 1 | $100 | $120 |
| Product 2 | $100 | $80 |
| Product 3 | $100 | $160 |
| Total | $300 | $360 |

In this case, a discount isn't specified for the transaction or for a line, but a discount of $60 is implicit because the total VSOE price is $60 greater than the invoice price ($360 - 300 = 60). Implicit discounts are allocated in the same way that line-item and transaction discounts are allocated.

Unless the Residual Method is being used, the discount of $60 is allocated to each bundle member, except members set as Permit discount = Never. The $60 implicit discount is allocated in the same way as the line-item discount, as follows:

| Item | Invoice price | VSOE Price | VSOE Calculation | Allocation |
| --- | --- | --- | --- | --- |
| Product 1 | $100 | $120 | 120/360 x 300 | $100.00 |
| Product 2 | $100 | $80 | 80/360 x 300 | $66.67 |
| Product 3 | $100 | $160 | 120/360 x 300 | $133.33 |
| Total | $300 | $360 |  | $300.00 |

## Implicit Discounts and the Residual Method {#bridgehead_N1728995}

If the residual method is used, any discounts (implicit, transaction or line item) are applied only to items with a Delivered VSOE status.

For example, you enter a sales order that doesn't include a transaction or line-item discount. The difference between the VSOE price of the undelivered items ($240) and the total invoice price ($300) is allocated to the delivered item.

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered |
| --- | --- | --- | --- | --- |
| Product 1 | $100 | $? | 300 - 240 = $60.00 | Yes |
| Product 2 | $100 | $80 | $80.00 | No |
| Product 3 | $100 | $160 | $60.00 | No |
| Total | $300 |  |  |  |

For more information about the residual method, read [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html).

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
