---
id: "section_N2264208"
type: "section"
title: "Avoiding Underwater Inventory"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Inventory Sales and Fulfillment > Avoiding Underwater Inventory"
parent: "section_N2281204"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2264208.html"
anchors: ["procedure_N2264319", "procedure_N2264363", "procedure_N2264412"]
sha256: "4588d2e4e84193704bd1a0e4528d8ac41b4c2344c39eedf21cea0c92a9becb60"
---

Selling an item when the data shows that you do not have the item in stock is known as an 'underwater' sale. Inventory is in an underwater state when the on-hand quantity of the item is below zero. You should avoid entering an item on a sale transaction if the on hand count of the item is zero or a negative amount.

Problems can arise if you enter sale transactions over a period when an item is underwater. NetSuite has difficulty calculating the cost of the item on those sale transactions. These cost calculations from underwater sales can lead to skewed results for reports and inventory data.

When the on hand count is below zero, costing information at the time of the sale is shifted to another date. The estimated cost is calculated based on the last known cost when the item was in stock.

At a later date when more of the item is received into stock, the true cost can be calculated. Then, you can post an adjustment to correct for transaction lines entered when the item was underwater. However, because the adjustment posts with the item receipt, the correction does not post with the original estimated cost.

For example, consider the following scenario where inventory is sold underwater:

-   On March 30, an invoice is entered that sells 100 widgets and brings the on hand count of widgets to -100 widgets.
    
-   Based on historical costing, the cost of the widgets is estimated at $10 each. Therefore, the cost of goods sold for the 100 widgets = ($10 x 100) = $1000.
    
-   On April 2, a purchase is entered for 100 widgets at a cost of $12 each. The actual cost of the widgets is ($12 x 100) = $1200. An adjustment of $200 is entered to correct the purchase price of the widgets.
    

After you enter a purchase that brings an underwater item count back above zero, the costing adjustments entered balance totals across affected periods. However, when viewing reports by period, sales and purchases posting in different periods may still shift the cost results from one period to another.

Consider the balance for March and April **combined**. The total balances because the sale in March and the purchase in April (that includes the adjustment) are **both** included.

However, if you consider only sales in the month of March. The total is off by $200 because the adjustment that posted with the item receipt does not show in the totals. If you consider only purchases for the month of April. The total is off by $200 because the adjustment is included in the total without the sale.

If you do not enter purchases to bring the item count back above zero, the costing estimates remain in the system. For example, a costing estimate can be $0.00 if there is no purchase history. However, this can cause larger adjustments after you enter a purchase to bring the item count back above zero.

Important:

The time between the underwater item sale and the purchase that brings the count above zero, the more skewed your data and reports.

For example, an item is underwater only three days before you enter a purchase that brings it back above zero. Reports and data will be less skewed than if an item is underwater for three months.

## Why should I care about selling underwater inventory? {#procedure_N2264319}

-   **Data is less accurate** - When you have underwater items in your inventory, your inventory data is less accurate. Inaccurate inventory data can affect other aspects in NetSuite and can potentially skew data in your chart of accounts, reports, and other areas.
    
-   **Transactions are more confusing** - Purchases that include costing estimates are often confusing for users who are not familiar with the costing workflow for underwater sales. Sorting out transactions associated with underwater sales can be time consuming and counterproductive.
    
-   **Records are less fit for audits** - Transactions that include underwater items also include estimates and adjustments. These transactions are less likely to be well received by auditors.
    
    For more information, see [System Cost of Goods Sold Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2195087.html).
    

## How can I tell if I am selling underwater inventory? {#procedure_N2264363}

You can tell if you are selling underwater inventory by the following:

-   The sale transaction shows a negative on-hand count of the item
    
-   You receive a warning that the item is not in stock
    

It is best to focus concern on the point in your workflow at which items leave your inventory. For example, your workflow can include entering sales orders and then fulfilling them. Because items do not leave stock when you enter the sales order, your focus is not on that transaction. However, when you enter the fulfillment, items do leave stock and you need to be cautious that the fulfillment does not include underwater items.

## How can I avoid selling underwater inventory? {#procedure_N2264412}

You can avoid being in an underwater state with inventory items by following these tips:

-   Insist on prompt entry of item receipts.
    
-   Require item receipts to be entered with the date of receipt.
    
    Enter receipt date instead of the entry date if the receipt is not entered the same day it is received.
    
-   Always use sales orders to sell inventory.
    
-   Always fulfill orders from sales orders.
    
-   Set the **Fulfill Based on Commitment** preference to **Limit to Committed**.
    
    For more information about this preference, see [Order Management Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html).
    

-   Avoid entering standalone cash sales and invoices.
    
    Standalone transactions have no commitments or checks and balances to prevent you from selling out or going underwater.
    
-   Use the Inventory Level Warnings preference.
    
    This preference gives you instant feedback on each transaction about whether you have items in stock. For more information about this preference, read [Setting the Inventory Level Warnings Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2254698.html).
    

-   Perform a physical inventory count on a regular basis to assess whether your inventory data is consistent with the physical count of your stock.
    
    If the physical count is different from the quantity on hand based (item record), the count must be reconciled to match actual inventory levels.
    
-   Use the Review Negative Inventory page to identify inventory items that are underwater.
    
    To learn more, see [Reviewing Negative Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2268458.html).
    

### Related Topics

-   [Inventory Sales and Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2281204.html)
-   [Handling Backorders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263962.html)
-   [Basic Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2250682.html)
-   [Inventory Adjustments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2259648.html)
-   [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html)
-   [Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2285050.html)
-   [Multi-Location Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2303574.html)
-   [Inventory Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2353200.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
