---
id: "section_N1729793"
type: "section"
title: "Resolving Undetermined VSOE Allocation"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Resolving Undetermined VSOE Allocation"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html"
anchors: []
sha256: "ff614a397ab893eb8dd605f63858b03390613d60a02c6aa129f20d2a59f08710"
---

Allocation calculations usually occur at the time you enter the transaction and are based on the vendor-specific objective evidence (VSOE) settings at that time. However, in some cases, allocation can't be performed because VSOE information is unavailable for an item and the correct allocation amount can't be determined.

For example, VSOE allocation can't be performed when the correct VSOE allocation can't be determined for an item, such as under these conditions:

-   Items not marked Delivered don't have a VSOE price
    
-   The transaction isn't set to auto-calculate
    
-   The transaction is set to auto-calculate the VSOE allocation and any item in the bundle doesn't have a VSOE price (except when using the residual method)
    

If any of these conditions are met, NetSuite can't determine the VSOE allocation amount and doesn't allow the transaction to be saved.

For example, a VSOE transaction bundle on a sales order includes the following:

| Item | Invoice Price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Software Product 101 | $500 | unknown | not determined | No | Defer Until Item Delivered |
| Software Product 201 | 300 | unknown | not determined | No | Defer Until Item Delivered |
| Software Service | 800 | $500 | not determined | No | Defer Until Item Delivered |
| Total | $1600 |  |  |  |  |

The VSOE price is unknown for one or more undelivered items, and the VSOE allocation can't be determined.

When the two items without a VSOE price are marked Delivered, the VSOE allocation can be determined using the [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html), as shown below:

| Item | Invoice Price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Software Product 101 | $500 | unknown | $687.50 | Yes | Defer Until Item Delivered |
| Software Product 201 | 300 | unknown | 412.50 | Yes | Defer Until Item Delivered |
| Software Service | 800 | $500 | 500 | No | Defer Until Item Delivered |
| Total | $1600 |  | 1600 |  |  |

If you can't save a transaction because VSOE allocation can't be performed, you can do the following to resolve the problem:

-   Verify the VSOE settings of items on the transaction. When you save changes, NetSuite automatically recalculates the VSOE allocation.
    
-   Clear the Transaction is VSOE Bundle box to be able to save the transaction. Later, you must re-check the Transaction is VSOE Bundle box and enter the VSOE price for the auto-calculation to be performed.
    
-   Allocate VSOE manually.
    
    To enable manual allocation of VSOE, go to _Setup > Accounting > Accounting Preferences_. Click the **General** subtab and clear the **Allow Users to Modify VSOE Values on Transactions** box.
    
-   Allocate VSOE using custom code. For more information, see [Client Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158379074356.html#subsect_158473831107).
    

When the bundle is billed, the allocated value of the bundle is recognized according to the associated recognition schedule.

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
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
