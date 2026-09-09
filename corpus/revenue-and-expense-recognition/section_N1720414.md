---
id: "section_N1720414"
type: "section"
title: "Allocating VSOE Revenue for a Bundle"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Allocating VSOE Revenue for a Bundle"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html"
anchors: ["bridgehead_N1720886", "bridgehead_N1720898", "procedure_N1720911"]
sha256: "e1db149eee7f8ab9f46ebf4886404ffafda7c28311536354a8247ee95077dad0"
---

As you sell bundles, it's the vendor-specific objective evidence (VSOE) value of the items, not the sale value, that is the revenue amount recognized for the sale. Allocation is the process used to determine the amount recognized for each item in a bundle. The total VSOE amount allocated always equals the sales amount of the transaction bundle (or the item group if you're using item groups for VSOE).

The VSOE allocation amount for a sale can be calculated automatically by checking the Auto-calculate VSOE box on a transaction. The VSOE price allocated to member items is determined by the VSOE settings on each item record and the delivery status of the item. Allocation amounts can also be calculated manually. See [Manual Calculation of VSOE Allocations](#bridgehead_N1720898). You can also allocate VSOE using custom code. See SuiteScript [Client Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158379074356.html#subsect_158473831107) for more information.

Important:

After a VSOE bundle is invoiced, the allocation amounts can't change. For example, you enter a sales order with three items. Only two of the items are marked delivered for VSOE and are eligible to have their allocated value recognized. After invoicing the sales order, you mark the third item delivered for VSOE. Marking the item delivered after invoicing doesn't impact the VSOE allocation. None of the VSOE settings impact the VSOE allocation after the order has been invoiced. Only the delivered flag can be checked after invoicing to start the revenue recognition process.

The VSOE value allocated to bundle member items is determined by the following:

-   Revenue recognition settings on each item record
    
-   VSOE settings on each item record
    
-   Delivery status of the items
    
-   Transaction-level and line-level discounts
    

For example, a VSOE transaction bundle includes the following:

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Installation Service 202 | $1500 | $1000 | $1000 | Yes | Defer Until Item Delivered |
| Software Product 101 | $1500 | $2000 | $2000 | Yes | Defer Until Item Delivered |
| Software Product 103 | $2500 | $2500 | $2500 | Yes | Defer Until Item Delivered |
| Total | $5500 | $5500 | $5500 |  |  |

NetSuite allocates the VSOE price of all items in this bundle based on their deferral settings and delivery status. All items in the bundle are set as Defer Until Item Delivered AND all items are marked as delivered.

Because the total invoice amount of the bundle items is equal to the total VSOE price, the VSOE allocation for each item is the VSOE price of each item. The total VSOE amount allocated for this sale is $5500.

For more examples of VSOE allocation, see [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html).

## VSOE Allocation and Currencies {#bridgehead_N1720886}

If you use NetSuite OneWorld and have enabled both the VSOE and Multiple Currencies features, when you enter a transaction using a currency other than the base currency, the VSOE price and allocation are calculated based on the foreign currency, not the base currency. The VSOE allocation is performed using the converted VSOE price or sales amount.

## Manual Calculation of VSOE Allocations {#bridgehead_N1720898}

You can set an accounting preference to calculate VSOE allocation manually.

#### To indicate that allocations should be calculated manually: {#procedure_N1720911}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  On the **General** subtab, scroll to the Revenue Recognition section, and clear the **Allow Users to Modify VSOE Values on Transactions** box.
    
3.  Click **Save**.
    

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Using VSOE on Sales Orders and Invoices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
