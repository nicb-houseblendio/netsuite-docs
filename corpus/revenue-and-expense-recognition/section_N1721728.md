---
id: "section_N1721728"
type: "section"
title: "Using VSOE on Sales Orders and Invoices"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Recognizing Revenue for VSOE Bundles > Using VSOE on Sales Orders and Invoices"
parent: "section_N1720104"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721728.html"
anchors: ["procedure_N1724938"]
sha256: "dc6b8e88a6d48d6bf2eb27f741dfc1242d897216385cb53788a00dda04e93955"
---

Vendor-specific objective evidence (VSOE) can be used on individual invoices or used together with sales orders. VSOE settings entered on sales orders can also affect invoices created from them.

If the revenue for an item on a sales order must be recognized using a revenue recognition schedule and the sales order will be billed on an invoice for a bundle, the **Transaction Is VSOE Bundle** box on the Accounting subtab must be checked. This setting ensures that NetSuite generates a revenue recognition schedule so that the revenue on the Sales Order is correctly billed on the bundle invoice.

For example, you enter the following sales order:

| Item | Invoice price | VSOE Price | VSOE Allocation | Delivered? | Deferral |
| --- | --- | --- | --- | --- | --- |
| Software Product 201 | $500 | $400 | $400 | Yes | Defer Until Item Delivered |
| Support | $300 | $200 | $200 | No | Defer Until Item Delivered |
| Software Product 301 | $800 | $1000 | $800 | Yes | Defer Until Item Delivered |
| Total | $1600 | $1600 | $1600 |  |  |

When you invoice this order, a revenue recognition schedule isn't created for the undelivered support item. The revenue of $200 is deferred indefinitely. After an invoice is created from a sales order, changes to the sales order can affect the VSOE settings and revenue recognition of the billed amount, even without any changes on the invoice.

When you make either of these changes to a sales order, the changes also affect the invoice:

-   Changing the delivery status
    
-   Changing the VSOE allocation
    

For example, in the order shown above, if you change the status of the support item to Delivered on the sales order, a revenue recognition schedule is created for the item, even though the invoice was not changed. This change is implemented either by saving changes to lines of the sales order or by clicking the Update VSOE button.

Note that the following changes **don't** affect the invoice:

-   Removing or adding an item
    
-   Changing the delivery status for an item to Not Delivered after revenue has already posted from the related revenue recognition schedule for that line
    

#### To enter VSOE information on a sales order: {#procedure_N1724938}

1.  Go to _Transactions > Sales > Enter Sales Orders_.
    
2.  For a line item, click the field in the **VSOE** column. The VSOE fields display.
    
    1.  Enter information in the following fields as needed:
        
        -   **VSOE Price**
            
            Enter the VSOE price for this item if it's known.
            
        -   **VSOE Amount**
            
            As you sell bundles, it's the VSOE value of the items, not the sale value, that is the revenue amount recognized for the sale. Allocation is the process to determine the amount to be recognized for each item in a bundle. The total VSOE amount allocated always equals the sales amount of the bundle.
            
            Enter a manually calculated allocation amount, if needed.
            
            The VSOE allocation amount for a sale can be calculated automatically by checking the Auto-calculate VSOE box on a transaction.
            
        -   **VSOE Allocation**
            
            This field holds the revenue value of the item. It may be automatically populated by selecting the Auto-calculate VSOE box on a transaction or manually entered. If you manually enter this value, the total VSOE amount allocated must equal the total sales amount of the bundle. Furthermore, no VSOE allocation can be negative.
            
        -   **Deferral**
            
            Choose how to handle deferment when this item is sold as part of a bundle:
            
            **Defer Bundle Until Delivered** - Until this item is marked delivered, the revenue recognition of all items in the bundle is deferred. A typical use for this option is to identify items whose revenue recognition depends on the delivery of the item itself, in addition to the delivery of a separate service. For example, a specified upgrade would typically be marked Defer Bundle Until Delivered.
            
            **Defer Until Item Delivered** - Until this item is marked delivered, the revenue recognition of this item is deferred. This setting is the default for this field.
            
        -   **Permit Discount**
            
            In the Permit Discount field, choose from the following to determine how discounts are handled for this item.
            
            **As Allowed** - Allows a portion of an applicable discount to be applied against this item if its status is Delivered when the VSOE allocation is performed. This is the default value for this field.
            
            **Never** - Doesn't allow a discount to be applied against this item when the VSOE allocation is performed. This selection would be common for a Specified Upgrade.
            
        -   **Delivered**
            
            The VSOE delivery status is used to determine how the sales amount of the bundle is allocated to individual members based on their VSOE settings, and to specify that revenue recognition for the item can begin when the order has been billed.
            
            Check this box to mark the item as delivered. Clear this box to mark the item as not yet delivered.
            
    2.  Click **Add**.
        
3.  Repeat step 2 to add other VSOE items.
    
4.  Complete other sales order fields as needed.
    
5.  Click **Save**.
    

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Recognizing Revenue for VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720104.html)
-   [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html)
-   [Updating VSOE Allocations and Delivery Status on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1721160.html)
-   [Updating the VSOE Delivery Status on Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725322.html)
-   [Billing a VSOE Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1725637.html)
-   [Using VSOE with Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1726248.html)
-   [Using VSOE with Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729547.html)
-   [Resolving Undetermined VSOE Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1729793.html)
-   [Posting VSOE Revenue to the General Ledger](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1732506.html)
-   [Using the Residual Method of Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1733002.html)
-   [VSOE Revenue Recognition Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1736679.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
