---
id: "section_N2172688"
type: "section"
title: "Account Information about Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Using Item Records > Creating Item Records > Account Information about Items"
parent: "section_N2166469"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2172688.html"
anchors: []
sha256: "0c0c2bea49ac96d3b43f7e62130af36aca173f208ec3fd685873151fe899a288"
---

The following fields are used to set up your preferred handling of accounts for each item. The fields and subtabs that appear depend on the features you have enabled and the type of record you view.

Important:

when selecting accounts. Problems can occur when you try to change an account on an item record after an item transaction has been entered. Contact your NetSuite account representative to update an account on an item.

**COGS Account** - Select a Cost of Goods Sold (COGS) account to track the cost of this item. Don't duplicate this account. This field appears only on Inventory and Assembly items.

**Asset Account** - Select an asset account to track the value of stock on hand. Don't duplicate this account. This field appears only on Inventory and Assembly items.

**Income Account** - Select an income account to track item sales revenue. Don't duplicate this account.

This field appears only on the following items:

-   Assembly
    
-   Download
    
-   Gift Certificate
    
-   Inventory
    
-   Kit/Package
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale or resale
    
-   Service for sale or resale
    

**Update COGS and Asset accounts on existing transactions when accounts are changed** - Check this box to update COGS and Asset Accounts when you update an item record account. The box is cleared after saving the item record. This field appears on Inventory and Assembly items and is enabled when COGS or Asset accounts are updated. Additionally, the **Do Not Update COGS and Asset Accounts on Existing Transactions When Accounts Are Changed** preference must be enabled at Setup > Accounting > Accounting Preferences > Items/Transactions > Accounts.

**Deferred Revenue Account** - When this item is sold and revenue recognition or advanced revenue management (essentials) is enabled, the revenue from the sale is deferred. The sale amount is posted to a deferred revenue account, as opposed to a standard income account. For more information, see [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html) or [Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4328435538.html).

This field appears only on the following items:

-   Assembly
    
-   Download
    
-   Inventory
    
-   Kit/Package
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale or resale
    
-   Service for sale or resale
    

**Intercompany Deferred Revenue Account** - This account records deferred revenue when you sell this item between subsidiaries. This account is used by the Revenue Recognition or Advanced Revenue Management (Essentials) features. The Automated Intercompany Management feature must also be enabled to eliminate intercompany transactions correctly. Therefore, you must select an account that has the Eliminate Intercompany Transactions box checked. This field appears only on inventory type items and the following resale item types: Non-inventory, Other Charge, and Service. For more information, see [Automated Intercompany Management Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486393.html).

**Gain/Loss Account** - Use this account if you don't use the **Use Item Cost as Transfer Cost** preference. The transfer price on a transfer order is used as the item cost on the item receipt. Any difference between the cost and the transfer price posts to a Gain/Loss account when the item is shipped. For information about setting the Use Item Cost as Transfer Cost preference, see [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

Select the Gain/Loss account you prefer to use to post transfer cost discrepancies. The account you select must be different from the Cost of Goods Sold (COGS) and asset account for the item. You can also choose the Use Income Account setting to use the income account as the Gain/Loss account.

If you leave this field blank or select Use Income Account, the income account for the item is used.

If you use the **Expand Account Lists** preference, you can choose any account in this field.

**Price Variance Account** - Select the account to post to for variances in billing prices associated with this item. Variances occur when the item price appearing on the purchase order is different from the item price appearing on the bill.

Note:

After you select a variance account, you can change the another, if necessary. Account changes are noted on the System Notes subtab of the History subtab of item records.

**Quantity Variance Account** - Select the account to post to for variances in billing quantities associated with this item. Variances show up when the item quantity on the receipt doesn't match the quantity on the bill.

Note:

After you select a variance account, you can change the account, if necessary. Account changes are noted on the System Information subtab of item records.

**Exchange Rate Variance** - Select the account to post to for variances in exchange rates associated with this item. Variances occur when exchange rates differ between the receipt and the bill for an item.

Note:

After you select a variance account, you can change the account, if necessary. Account changes are noted on the System Information subtab of item records.

**Customer Return Variance Account** - Select the account you want to post amounts to for cost variances of items returned by customers. The Customer Return Variance Account takes the place of using the Cost of Goods Sold (COGS) account for the entire cost of the item. This account should not be duplicated.

You can set a specific COGS account to use for returns of this item to track costing separately for returns and sales. For example, a return authorization (RMA) might have a value of $5 for the item. But after the RMA is received, the costing value received is now $4. This generates a difference of $1.

-   If you select a Customer Return Variance Account, the $1 posts to the account you choose in this field.
    
-   If you **do not** select a Customer Return Variance Account, the $1 posts to the account chosen in the COGS Account field. This is the same field that sales COGS amounts post to.
    

This field appears only when you use the Return Authorizations feature.

**Vendor Return Variance Account** - Select the account you want to post amounts to for cost variances of items returned to vendors. This account should not be duplicated.

You can set a specific Cost of Goods Sold (COGS) account for returns of this item to track costing separately for returns and purchases. If you don't select a Vendor Return Variance Account, any variances post to the account chosen in the COGS Account field.

**Production Quantity Variance Account** - Variances post to this account when the assembly cost is higher or lower than expected due. This can be due to the number of items used in the assembly build. For example, a variance is created if a build costs more because you use 10 widgets, when you normally use eight.

**Production Price Variance Account** - Variances post to this when the assembly cost is higher or lower than expected. This can be due to the expense of items used in the assembly build. For example, a variance is created if a build costs more because you use widgets that cost $30 each, when you normally pay $20.

**Unbuild Variance Account** - Select the account to post a variance to when an unbuild transaction calculates a cost variance. This account should not be duplicated.

**Purchase Price Variance Account** - Select the account to post a variance to when a purchase transaction calculates a cost variance.

**WIP Cost Variance Account** - This is an expense account for cost or average cost assemblies. This is true when the reconciliation amount can't be returned to the asset account because the amount has been shipped. This account is required if WIP is checked for any locations. This field appears only on Assembly items using WIP.

**Scrap Account** - This is an expense account for scrapping that occurs during the work order completion. This account is required if WIP is checked for any locations. This field appears only on Assembly items using WIP.

**WIP Account** - This is an asset account used when a work order component issue is entered. This account is required if WIP is checked for any locations. This field appears only on Assembly items using WIP.

**Account** - Select the account where this discount, markup, or payment should post. This field appears only on Discount, Markup, and Payment items.

**Expense Account** - Select an expense account to associate with this item.

This field appears only on the following items:

-   Non-inventory for purchase or resale
    
-   Other Charge for purchase or resale
    
-   Service for purchase or resale
    

**Group with Undeposited Funds** - Select Group with Undeposited Funds process these payments as any other undeposited funds. If these are to be deposited immediately into an account, select Account.

**Liability Account** - Select a liability account for gift certificate sales. This field appears only on Gift Certificate items.

**Non-posting** - Select Non-posting if you don't want discount or markup amounts to post to an account. This field appears only on Discount and Markup items.

### Related Topics

-   [Item Record Header Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161918187368.html)
-   [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html)
-   [Sales and Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2171993.html)
-   [Revenue Recognition and Amortization Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173064.html)
-   [Tax and Tariff Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173187.html)
-   [Entering Preferences on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173412.html)
-   [Copying and Importing Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173669.html)
-   [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
