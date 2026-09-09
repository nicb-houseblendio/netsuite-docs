---
id: "section_N1733002"
type: "section"
title: "Using the Residual Method of Revenue Recognition"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Using the Residual Method of Revenue Recognition"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html"
anchors: ["bridgehead_N1733118", "bridgehead_N1733823", "bridgehead_N1733860"]
sha256: "594f74e0ed117e6dfb801e3ff51a6d0d19faedbd98cef17a8b27d970e13728c3"
---

When a transaction includes an item with a vendor-specific objective evidence (VSOE) price that differs from its sales amount, VSOE prices are allocated to all items in the bundle. The allocation process uses the total sales amount of the transaction to assign a VSOE price to the bundle. The VSOE price allocated is the amount that is eventually recognized based on VSOE rules.

When VSOE prices aren't known for one or more items in a bundle, the VSOE allocation may be determined if the bundle qualifies for the Residual Method of revenue recognition using SOP 98-9. SOP 98-9 amends part of SOP 97-2 and requires the recognition of revenue using the residual method in some circumstances.

The Residual Method can be used to determine the VSOE allocation for items if a bundle meets these conditions:

-   All **undelivered** items **have** a VSOE price.
    
-   One or more **delivered** items **don't have** a VSOE price.
    
-   The total VSOE amount for undelivered bundle items is less than the total sales amount of the bundle.
    

For more information about using the residual method, see:

-   [Residual Method Calculation](#bridgehead_N1733118)
    
-   [Discounts and the Residual Method](#bridgehead_N1733823)
    
-   [Residual Method Examples](#bridgehead_N1733860)
    

## Residual Method Calculation {#bridgehead_N1733118}

Using the residual method, the vendor-specific objective evidence (VSOE) allocation is calculated based on the fact that the total sales price of an item group must always equal the total VSOE allocation.

The formula used to calculate VSOE Allocation using the Residual Method is:

(total invoice amount of bundle - VSOE prices of **undelivered** items)

\= amount to apply to delivered items lacking a VSOE Price in proportion to their invoice prices

When the total VSOE amount of a sale is known, NetSuite can calculate the VSOE value for qualifying individual items.

For example, you sell the following VSOE bundle:

| Bundle Members | Invoice price | VSOE price | VSOE Allocation | Delivered |
| --- | --- | --- | --- | --- |
| Software Product 099 | $10,000 | unknown | unknown | Yes |
| Professional Services (100 hours) | 8,000 | $10,000 | unknown | No |
| Maintenance, 1 year | 2,000 | 2000 | unknown | No |
| Total | $20,000 | unknown | $20,000 |  |

The total sales amount of this transaction equals $20,000. Therefore, using the residual method, the VSOE allocation must equal $20,000 also.

When you apply the formula above, VSOE is calculated as follows:

total invoice amount of bundle ($20,000) - VSOE prices of **undelivered** items ($12,000)

\= amount to apply ($8000)

Undelivered items have the same VSOE allocation as their VSOE price and the remaining amount of $8,000 becomes the VSOE allocation for the delivered software product, as follows:

| Bundle Members | Invoice price | VSOE price | VSOE Allocation | Delivered |
| --- | --- | --- | --- | --- |
| Software Product 099 | $10,000 | unknown | $8000 | Yes |
| Professional Services (100 hours) | 8,000 | $10,000 | 10,000 | No |
| Maintenance, 1 year | 2,000 | 2000 | 2,000 | No |
| Total | $20,000 | unknown | $20,000 |  |

If the bundle contains multiple items marked Delivered, the remainder is allocated proportionately to those items based on their sales prices.

## Discounts and the Residual Method {#bridgehead_N1733823}

When a discount is applied to a bundle, the discount may only be allocated to the delivered items in that bundle. Each delivered item must have an invoice price to determine the allocation of the discount.

The Never flag can be used to prevent the allocation of discount to delivered items in the case of a specified upgrade. If the Permit Discount field on an item record is set to **Never**, then discounts aren't applied to the item. For more information, read [Setting Up VSOE on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718972.html).

Note:

If a bundle includes both undelivered and delivered items and all delivered items have a **Permit Discount** setting of **Never**, the auto-calculation of VSOE allocation isn't performed.

## Residual Method Examples {#bridgehead_N1733860}

The following examples illustrate the use of the residual method of revenue recognition to determine the vendor-specific objective evidence (VSOE) allocation.

In the example below, the VSOE allocation is deferred for all items until the specified item is delivered. The items that are undelivered have a VSOE allocation equal to their VSOE price. The residual amount of $2000 becomes the VSOE allocation for the delivered product.

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered | Deferral |
| --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000 | No | Defer Bundle Until Delivered |
| Software Product 101 | 1500 | 2000 | 2000 | Yes | Defer Until Item Delivered |
| Software Product 103 | 2500 | not assigned | 2500 | Yes | Defer Until Item Delivered |
| Total | $5500 |  | $5500 |  |  |

NetSuite doesn't allocate the VSOE price to any items, pending the delivery of the Installation Service 202 item, which is marked Defer Bundle Until Delivered. When Installation Service 202 is delivered, VSOE prices are allocated based on residual method calculations.

In the next example, a residual amount is allocated between more than one delivered item:

| Item | Invoice price | VSOE Price | VSOE Allocation | Calculation | Delivered | Deferral |
| --- | --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000.00 | VSOE price =VSOE allocation | Yes | Defer Until Item Delivered |
| Software Product 101 | 1500 | not assigned | 1687.50 | 4500 x (1500/4000) = 1687.50 | Yes | Defer Until Item Delivered |
| Software Product 103 | 2500 | not assigned | 2812.50 | 4500 x (2500/4000) = 2812.50 | Yes | Defer Until Item Delivered |
| Total | $5500 |  | $5500 |  |  | Defer Until Item Delivered |

In the next example, the residual amount is allocated between multiple delivered items for a bundle discounted 10%. None of the discount is applied to the undelivered item.

| Item | Invoice price | VSOE Price | VSOE Allocation | Calculation | Delivered | Deferral |
| --- | --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000.00 | VSOE price =VSOE allocation | No | Defer Until Item Delivered |
| Software Product 101 | 1500 | not assigned | 1481.25 | \=1500/(1500+2500) x (4950-1000) | Yes | Defer Until Item Delivered |
| Software Product 103 | 2500 | not assigned | 2468.75 | \=2500/(1500+2500) x (4950-1000) | Yes | Defer Until Item Delivered |
| Subtotal | $5500 |  |  |  |  |  |
| 10% Discount | (550) |  |  |  |  |  |
| Total | $4950 |  | $4950 |  |  |  |

In the next example, the residual amount is allocated between multiple delivered items. The bundle includes a 10% discount and one of the delivered items has a Permit Discount setting of Never.

| Item | Invoice price | VSOE Price | VSOE Allocation | Calculation | Del. | Permit Discount | Deferral |
| --- | --- | --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000.00 | VSOE price =VSOE allocation | No | As Allowed | Defer Until Item Delivered |
| Software Product 101 | 1500 | not assigned | 1137.50 | 1500 / (1500 + 2500) x 4500 - 550 | Yes | As Allowed | Defer Until Item Delivered |
| Software Product 103 | 2500 | not assigned | 2812.50 | 2500 / (1500+ 2500) x 4500 | Yes | Never | Defer Until Item Delivered |
| Subtotal | $5500 |  |  |  |  |  |  |
| 10% Discount | (550) |  |  |  |  |  |  |
| Total | $4950 |  | $4950 |  |  |  |  |

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
