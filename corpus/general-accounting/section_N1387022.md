---
id: "section_N1387022"
type: "section"
title: "Items/Transactions Accounting Preferences"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Features and Preferences > Accounting Preferences > Items/Transactions Accounting Preferences"
parent: "section_N1384948"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html"
anchors: ["bridgehead_N1387138", "bridgehead_N1387389", "bridgehead_1484086302", "bridgehead_N1387462", "bridgehead_N1387765", "bridgehead_N1387830", "bridgehead_N1387974", "bridgehead_N1388006"]
sha256: "a9d35f7d0de19e7e559b81cb13fada2a0d4a0552da95757eb9828904d0424803"
---

The following preference options are available on the Items/Transactions subtab of the Accounting Preferences page:

-   [Accounts](#bridgehead_N1387138)
    
-   [Sales and Pricing](#bridgehead_N1387389)
    
-   [Charge-Based Billing](#bridgehead_1484086302)
    
-   [Inventory](#bridgehead_N1387462)
    
-   [Payment Processing](#bridgehead_N1387830)
    
-   [Other Transaction Preferences](#bridgehead_N1387974)
    
-   [Other Item Preferences](#bridgehead_N1388006)
    

## Accounts {#bridgehead_N1387138}

| Field | Description |
| --- | --- |
| Purchase Discount Account | Use this option to set the default expense account for purchase discounts. |
| Sales Discount Account | Use this option to set the default expense account for sales discounts. |
| Default Expense Account | Use this option to set the default expense account for non-inventory, service, and other charge items. Employees with permission can change the account on individual item records. |
| Default Income Account | Use this option to set the default income account for inventory, non-inventory, service, and other charge items. Employees with permission can change the account on individual item records. For more information, see [Permissions Documentation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326485.html). |
| Default Receivables Account | Use this option to set the default A/R account to be used on receivable transactions. You can set the default A/R account on customer records by editing the record, clicking the Financial subtab, and selecting an A/R account in the Default Receivables Account field. |
| Default COGS Account | Use this option to set the default Cost Of Goods Sold (COGS) account for inventory, non-inventory, service, and other charge items. Employees with permission can change the account on individual item records. |
| Default Asset Account | Use this option to set the default asset account for inventory items. Employees with permission can change the account on individual item records. |
| Default Payment Account | Use this option to set the default bank account to appear in the Deposit To field on cash sales and customer payments. |
| Default Vendor Payment Account | Use this option to set the default vendor payment account for a individual subsidiaries. This can be useful if one or more of your subsidiaries make vendor payments independently with unique accounts. |
| Default Gain/Loss Account | When the Use Item Cost as Transfer Cost preference is disabled, the transfer price on a transfer order is used as the item cost on the item receipt. Any difference between the actual cost and the transfer price posts to a Gain/Loss account when the item is shipped. In this field, select the default Gain/Loss account to use for posting transfer cost discrepancies. This account autofills the Gain/Loss Account field on item records you create. The account you select must be different from the Asset or Cost of Goods Sold (COGS) account for the item. You can choose an Income account, Other Income account, Expense account, or Other Expense account. Note: If you have enabled the Expand Account Lists preference, you can choose any account in this field. If you leave this field blank or select Use Income Account, the income account for the item is used. |
| Default Bill Quantity Variance Account | Use this option to set the default account for posting variances in billing quantities associated with this item. These variances occur when there is a difference in the quantity of an item showing on the receipt and the quantity of an item showing on the bill. The account you select defaults to show in the Bill Quantity Variance Account field on item records you create. Note: After you select a variance account in this field, you can select another account at a later date if a change is necessary. Account changes are noted on the System Notes subtab of the History subtab of item records. |
| Default Bill Price Variance Account | Use this option to set the default account for posting variances in billing prices associated with this item. These variances occur when there is a difference in the price of an item showing on the purchase order and the price of an item showing on the bill. The account you select defaults to show in the Bill Price Variance Account field on item records you create. Note: After you select a variance account in this field, you can select another account at a later date if a change is necessary. Account changes are noted on the System Notes subtab of the History subtab of item records. |
| Default Bill Exchange Rate Variance Account | Use this option to set the default account for posting variances in exchange rates associated with this item. These variances occur when there are exchange rate differences between the receipt and the bill for an item. The account you select defaults to show in the Bill Price Variance Account field on item records you create. Note: After you select a variance account in this field, you can select another account at a later date if a change is necessary. Account changes are noted on the System Notes subtab of the History subtab of item records. |
| Default Unbuild Variance Account | Use this option to set the default account for posting variances that result from unbuilding an assembly item. The account you select shows by default in the Unbuild Variance Account field on item records. If the Unbuild Variance Account field is left blank on item record, variance amounts for the item post to the Cost of Goods Sold (COGS) account. Note: In NetSuite OneWorld, even when a default is set, this account defaults to be blank if the default account isn't available to the subsidiary on the form. |
| Default Vendor Return Variance Account | Use this option to set the default account you want to show in the Customer Return Variance Account field on new item records. The account you select is used to post amounts to for cost variances of items returned to vendors. For more information, see [Account Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2172688.html). |
| Default Customer Return Variance Account | Use this option to set the default account you want to show in the Customer Return Variance Account field on new item records. The account you select is used to post amounts to for cost variances of items returned to customers. For more information, see [Account Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2172688.html). |
| Default Production Quantity Variance Account | Use this option to set the default account for posting production quantity variances for items using standard costing. The account you select here shows by default in the Production Quantity Variance Account field on item records. Note: In NetSuite OneWorld, even when a default is set, this account defaults to be blank if the default account isn't available to the subsidiary on the form. |
| Default Production Price Variance Account | Use this option to set the default account for posting production price variances for items using standard costing. The account you select here shows by default in the Production Price Variance Account field on item records. Note: In NetSuite OneWorld, even when a default is set, this account defaults to be blank if the default account isn't available to the subsidiary on the form. |
| Default Purchase Price Variance Account | Use this option to set the default account for posting purchase price variances for items using standard costing. The account you select here shows by default in the Purchase Price Variance Account field on item records. Note: In NetSuite OneWorld, even when a default is set, this account defaults to be blank if the default account isn't available to the subsidiary on the form. |
| Default Inventory Cost Revaluation Account | Use this option to set the default account for posting variances that result from standard costing inventory revaluation transactions. The account you select here shows by default in the Adjustment Account field on inventory revaluations. Note: In NetSuite OneWorld, even when a default is set, this account defaults to be blank if the default account isn't available to the subsidiary on the form. |
| Default Inventory Count Account | Use this option to set the default account to display in the Account field on inventory count records. This account is used to post inventory count variances. This is typically an expense account. |
| Default WIP Cost Variance Account | Use this option to set the default expense account for cost or average cost assemblies when the reconciliation amount can't be returned to the asset account because the amount has been shipped. The selected account displays in the WIP Cost Variance Account field on assembly item records. |
| Default Dropship Expense Account | Use this option to set the default account to track expenses for drop shipments. |
| Default Scrap Account | Use this option to set the default expense account for scrapping that occurs during the work order completion. The selected account displays in the Scrap Account field on assembly item records. |
| Default WIP Account | Use this option to set the default asset account used when a work order component issue is entered. The selected account displays in the WIP Account field on assembly item records. |
| Anyone Can Set Item Accounts | Use this option to allow any employee with access to item records to choose accounts on item records. For example, when you check this box, any employee with access can set expense, asset, income, and Cost Of Goods Sold (COGS) accounts on item records. |
| Do Not Update COGS and Asset Accounts on Existing Transactions when Accounts are Changed | Set this option to retain the old COGS and Asset accounts of existing transactions even when you change the account from the item record. If you check this preference, the **Update COGS and Asset accounts on existing transactions when accounts are changed** box becomes available. You can find this option on the **Accounting** subtab of assembly and inventory item records. This option overrides your preference setting to update either or both accounts on existing transactions. For more information, read the help topic, [Changing the COGS and Asset Accounts on Assembly and Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0324022028.html). Note: After you check this box, existing transaction lines using COGS and Asset lines will no longer be updated, regardless whether the hidden preference **Ignore Closing Period When Updating G/L Accounts** is enabled or disabled. |
| Default Project Cost Variance Account | Use this option to set the default account used when posting project time for job costing. |
| Default Deferred Revenue Account | Use this option to set the default account for deferred revenue on sales transactions. The default option is the system-generated Deferred Revenue account. This preference is available only when advanced revenue management (essentials) is enabled. |
| Default ICJE Auto Balance Receivables Account | Use this option to set the default account for the Auto Balance button for the Receivables Account on Intercompany Journal Entries. Accounts available for selection are of type Accounts Receivable or Other Current Asset with the Eliminate Intercompany Transactions box checked. For more information, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html). |
| Default ICJE Auto Balance Payables Account | Use this option to set the default account for the Auto Balance button for the Payables Account on Intercompany Journal Entries. Accounts available for selection are of type Accounts Payable or Other Current Liability with the Eliminate Intercompany Transactions box checked. For more information, see [Making Advanced Intercompany Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4803443925.html). |

## Sales and Pricing {#bridgehead_N1387389}

| Field | Description |
| --- | --- |
| Consolidate Projects on Sales Transactions | Set this option to consolidate projects on customer invoices. You can create invoices for one customer including multiple projects. you're no longer able to issue invoices to a specific project. Instead, you issue the invoices to the customer. |
| Default Estimate Expiration (in days) | Use this option to set the default number of days before quotes can expire. |
| Maximum # of Quantity-based Price Levels | Set the maximum limit for the most price levels allowed to be assigned to an item when using Quantity Pricing. |
| Allow Quantity Discounts per Price Level on Schedules | Enable this option to allow edits to quantity discounts for each price level on quantity pricing schedules. |
| Include Reimbursements in Sales and Forecast Reports | Use this option to include billable expenses in sales and forecast reports. If this preference isn't enabled, transactions that affect expense accounts aren't included in sales and forecast reports. |
| Include Shipping in Sales and Forecast Reports | Enable this option to include shipping charge amounts in sales and forecast reports. If this preference isn't enabled, report calculations don't include shipping charges. |
| Transaction Types to Exclude From Forecast Reports | Select the transactions you don't want to include in forecast report calculations. Select multiple transaction types by pressing and holding CTRL as you make your selections. |
| Transaction Types to Exclude From Sales Reports | Select the transactions you don't want to include on sales report calculations. Select multiple transaction types by pressing and holding CTRL as you make your selections. |

## Charge-Based Billing {#bridgehead_1484086302}

| Field | Description |
| --- | --- |
| Default Fixed Date Charge Rule Stage | Use this option to set the default stage for fixed date charge rules. Charges created in the Ready stage are ready to be billed. Charges created in the Hold stage won't be billed until they're moved to the Ready stage. Select Hold if you have an approval process in place for new charges. |
| Default Milestone Charge Rule Stage | Use this option to set the default stage for milestone charge rules. Charges created in the Ready stage are ready to be billed. Charges created in the Hold stage won't be billed until they're moved to the Ready stage. Select Hold if you have an approval process in place for new charges. |
| Default Project Progress Charge Rule Stage | Use this option to set the default stage for project progress charge rules. Charges created in the Ready stage are ready to be billed. Charges created in the Hold stage won't be billed until they're moved to the Ready stage. Select Hold if you have an approval process in place for new charges. |
| Default Time-Based Charge Rule Stage | Use this option to set the default stage for time-based charge rules. Charges created in the Ready stage are ready to be billed. Charges created in the Hold stage won't be billed until they're moved to the Ready stage. Select Hold if you have an approval process in place for new charges. |
| Consider Charges in Hold State as Revenue | If you use Project Revenue Recognition, check this box to allow generated charges in the Hold state to be recognized according to established project revenue recognition rules. |

## Inventory {#bridgehead_N1387462}

| Field | Description |
| --- | --- |
| Scan Individual Items | Set your bar code scanning preference.
-   Set this option to individually scan the bar code for each item when fulfilling or receiving orders. For example, when you fulfill an order for 3 each of item XY123, scanning one bar code of item XY123 sets the fulfillment quantity to ONE. Then, you must scan the bar code of each of the remaining items to fulfill all three.
-   Clear this box to scan an item bar code one time and set the fulfillment/receipt quantity to the total amount of the item on the order. For example, when you fulfill an order for 3 each of item XY123, scanning one bar code of item XY123 sets the fulfillment quantity to THREE.

 |
| Centralize Purchasing in a Single Location | Set this option to consolidate inventory purchasing into one location, if you handle inventory in several locations. When this preference is enabled, you can order and receive all inventory in only one location and then transfer it to your other locations. For information about creating purchase orders, see [Purchase Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2399585.html). For information about moving inventory to different locations after receipt, see [Distributing Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2304534.html). |
| Days Before Lot Expiration Warning | Set the number of days in to receive a warning before items expires. For example, when you sell a lot item that is close to its expiration date, you get a warning. |
| Require Bins on All Transactions Except Item Receipts | When this option is enabled, any created transaction that changes inventory levels and includes an item that uses bins requires you to select a bin for the item to save the transaction. If there is no bin field on a transaction such as sales orders and purchase orders, bins are not required. Note that Item Receipts don't require a bin selection, even with this preference enabled. Disable this preference to permit transactions to be created that include items with no bin selected. Note that even with this preference disabled, NetSuite always requires bins on transactions where an item quantity is reduced such as on cash sales, item fulfillment, or negative inventory adjustments. Bins are not required on transactions where an item quantity is increased such as purchases and positive inventory adjustments. |
| Use Preferred Bin on Item Receipts | When you enable this option, the Bin field on item receipts defaults to the preferred bin instead of leaving the field blank. Disable this preference if you prefer the Bin field to remain blank by default. |
| Include Landed Cost in Last Purchase Price | Enable this option to always include the landed cost amount for the last purchase price.

-   Item costs displayed on item records include landed cost.
-   Gross Profit transactions apply the last purchase price including landed cost.
-   Purchase orders and other transactions default to use the last purchase price including landed cost when no default purchase price is found.

Disable this preference to always exclude the landed cost from the last purchase price amount.

-   Item costs displayed on item records don't include landed cost.
-   Gross Profit transactions apply the last purchase price excluding landed cost.
-   Purchase orders and other transactions default to use the last purchase price excluding landed cost when no default purchase price is found.

 |
| Print Lot Item Labels from Transactions by Quantity | Enable this option to configure labels to be printed by quantity. For example, consider an item receipt that has a line for Lot Item A, with a quantity of 12. By default, with the Print Lot Item Labels From Transactions By Quantity box cleared, one item label is printed for Lot Item A. If you check the box, 12 item labels are printed for Lot Item A. |
| Default Planning Rule Group | If you use the Supply Allocation and Material Requirements Planning features, you can select a planning rule group that provides the default lead time for transfer orders, including intercompany transfer orders. This lead time is used to calculate the Expected Receipt Date for items replenished through either of the following methods only: Material Requirements Planning or Master Production Schedule. For more information, see [Creating Planning Rule Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161944833572.html). |
| Recalculate Snapshot on Inventory Count Reject | If you use the Inventory Count feature, you can check this box to take a new inventory snapshot when you reject a count. Based on the new snapshot, NetSuite recalculates the adjustment quantity and variance. The new snapshot replaces the initial one that is taken when you start a count. If you process transactions during a count, NetSuite considers any on-hand quantity updates when you approve the rejected count. For more information, see [Setting Up Inventory Count](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2297156.html). |
| Display Current Count on Transfers | Set this preference to display the current on-hand quantity and value of items that you add to inventory transfers. It replaces the values based on the transaction's date, which is computed by default. To help prevent slowness when opening existing transactions, you should set this preference if you tend to add a large number of item lines to a single transaction. |
| Display Current Count on Worksheets | Set this preference to display the current on-hand quantity and value of items that you add to inventory worksheets. It replaces the values based on the transaction's date, which is computed by default. To help prevent slowness when opening existing transactions, you should set this preference if you tend to add a large number of item lines to a single transaction. |
| Display Current Count on Adjustments | Set this preference to display the current on-hand quantity and value of items that you add to inventory adjustments. It replaces the values based on the transaction's date, which is computed by default. To help prevent slowness when opening existing transactions, you should set this preference if you tend to add a large number of item lines to a single transaction. |

## Cost Accounting {#bridgehead_N1387765}

| Field | Description |
| --- | --- |
| Inventory Costing Method | Use this option to set the inventory costing method. The available options are: Average, Group Average, First In First Out (FIFO), or Last In First Out (LIFO). The costing method you choose determines how you manage the costs associated with buying the same items at different purchase prices over a specified time period. For details about costing methods, see [Costing Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2191818.html). |
| Default Cost Category | Use this option to set the default cost category to associate with new item records you create. The account you select displays by default in the Cost Category field on item records. View existing cost categories at _Setup > Accounting > Accounting Lists_ > Cost Category. |
| Average Cost Completion Unit Cost | Select one of the following:
-   **Average Cost** - Select this cost calculation method to see deviations between the cost of component consumption and the average cost of assemblies. If these variances are valid, they're incorporated into the assembly cost using the Inventory Adjustment Worksheet.
-   **Open WIP Amount** - Select this cost calculation method for calculating the completion cost based on the Open WIP amount.

 |
| Use Intransit Value in Group Average Cost Calculations | When you use the Multi-Location Inventory feature with the Group Average Costing feature, you can choose to include the account values for group average cost items that are in transit between locations. This allows in-transit inventory accounts to be balanced during the bulk process. Enabling this preference helps produce more accurate costing calculations and financial statement reporting by ensuring the group average cost reflects the assets of both on-hand and in-transit inventory accounts.

-   Clear this box to exclude the asset values of in-transit inventory accounts during the Balance Location Costing
-   Check this box to include the asset values of in-transit inventory accounts during the Balance Location Costing Group Accounts bulk process.

Note the following when this preference is enabled:

-   When this preference is enabled, the Create and Edit Inventory Transactions Dated in Closed Periods preference must be disabled.
-   Transfer Orders and Intercompany Transfer Orders are required to enable the Use Item Cost as Transfer Cost preference. For details about this preference, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).
-   Items set to use the Group Average costing method are not allowed to be added to intercompany purchases or sales. To transfer items between subsidiaries, they must be moved using an intercompany transfer order.
-   Transfer Orders and Intercompany Transfer Orders can't include both items that use Standard costing and items that use Group Average costing.

Note: If you plan to enable the Include Intransit in Group Average Cost Calculations preference, you should do so immediately after enabling the Group Average Costing feature. The setting for this preference can't be changed after any item with a Group Average costing method has had costing calculations run. |

## Payment Processing {#bridgehead_N1387830}

| Field | Description |
| --- | --- |
| Customers Can Pay Online | Enable this option to alloow your customers to pay their invoices online. Online payments require you to have a merchant account with the ability to accept credit card payments. NetSuite offers merchant account services, or you can use your own. To use the NetSuite merchant account services, go to _Setup > Accounting > Payment Processing Profiles_. |
| Process an Online Payment with Sales Order Creation at Customer Center. | Enable this option to require authorization for customers' credit cards on sales orders placed by Customer Center users logged in to NetSuite. To use this feature, you must have an Internet Merchant Solutions (IMS) account and you must set up a credit card processing profile at _Setup > Accounting > Payment Processing Profiles_. When customers order from your Customer Center, IMS automatically processes their credit cards and Verisign validates the payments. Authorization numbers automatically appear on the appropriate sales orders. For information about setting up customer credit card processing, see [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html). The option here is different from the **Process an online payment with sales order creation** option at _Commerce > Websites > Website List_. For more information about requiring authorization on credit card transactions, see [Require Authorization for Web Store Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2470131.html).
-   The Get Authorization on Customer Center Sales Order option applies to sales orders placed by Customer Center users logged in to the NetSuite application.
-   The Require Authorization on Credit Card Transactions option Web site preference applies to sales orders placed by customers logged in to your Web site.

You can enable one of these options at a time or both of them together. |
| Use Card Security Code for Credit Card Transactions | Use this option to add a field for your customers' Card Security Code (CSC) numbers on sales transactions. It also requires your customers to enter CSC numbers during the checkout process in your Customer Center or Web site. This feature can help prevent fraudulent orders. Note: To verify CSC numbers on your Web site, you must enable Require Authorization on Credit Card Transactions at _Commerce > Websites > Website List_. To verify CSV numbers for orders placed by Customer Center users logged in to NetSuite, you must enable the Get Authorization on Customer Center Sales Orders option. These options are available only after you add a credit card processing profile at _Setup > Accounting > Payment Processing Profiles_. |
| Allow Adjusted Expiration Date to Improve Recurring Payments | Clear this box if you don't want payments to be marked as recurring on the following transactions:

-   sales orders that use the Sales Order - Cash Sale form and have billing schedules
-   memorized cash sale sales orders

Note: Some credit card processing profiles don't support recurring payment authorization requests. If this option is enabled, whenever a credit card authorization request is declined due to expired credit card, a second request is sent with the expiration date updated to ensure that recurring payments are not interrupted. For more information, see [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html). |
| Enable Sale Payment Operations on a Sales Order by Automatically Creating a Customer Deposit | Check this box to enable using payment processing profiles that don't support authorization and instead support the sales request. When you check this box and use this type of profiles on sales orders, funds are immediately captured from the shopper's account and associated with the sales order as a customer deposit. For more information, see [Alternative Non-Credit Card Payment Methods for Web Store Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4213266422.html). To use this feature, you must have a merchant account provided by the gateway or the payment service provider. |
| Use Strict Rules for the Selection of Payment Processing Profiles | Enable this option to display only payment processing profiles that support all of the following requirements:

-   The selected payment method
-   The customer's currency
-   The customer's subsidiary (NetSuite OneWorld only)

If this preference is enabled, and there is no payment method supported by the shopper's currency, no credit card payment method shows on the Payment Information page of your website. This preference takes precedence over the Restrict Payment Methods by Customer Currency preference on the Shopping subtab at _Commerce > Websites > Website List_. For more information, see [Restricting Payment Processing Profiles by Customer Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html#bridgehead_4335053679). |
| Preserve Transactions When Payment is on Hold | If you enable this option, cash sale and customer payment transactions are preserved if the payment fails due to a payment hold. Preserved transactions have the Unapproved Payment status and are non-posting. |

## Other Transaction Preferences {#bridgehead_N1387974}

| Field | Description |
| --- | --- |
| Duplicate Number Warnings | Use this option to choose whether to receive duplicate number warnings or not when transactions are submitted with the same numbers. If you import transactions and use the Advanced Numbering feature, NetSuite responds to duplicates according to these settings. When you import a transaction, NetSuite determines which advanced numbering rule applies to it using your rules' criteria. It then checks if a transaction with the same document numbers already exist for the same rule. If a duplicate is detected, NetSuite uses your Duplicate Number Warnings preference as described below. Choose between the following:
-   **No Warnings** - Users are not warned when the transaction they're saving will create a duplicate document number. If you import transactions and use Advanced Numbering, NetSuite doesn't warn you when the imported transactions use duplicate document numbers and imports all transactions.
-   **Warn (UI only)** - Users receive a message when attempting to save a transaction record with the same document number as another record of the same type. When the warning is displayed, a user can enter a different number before attempting to save again. If you import transactions and use Advanced Numbering, NetSuite doesn't warn you when the imported transactions use duplicate document numbers and imports all transactions.
-   **Warn and Block** - Users receive a message when attempting to save a transaction record with the same number as another record of the same type. When the warning is displayed, the user must click Cancel and change the document number in the record. If you import transactions and use Advanced Numbering, NetSuite warns you when imported transactions create duplicate document numbers, and doesn't import these transactions.

 |
| Sort Reconcile By | Choose to sort reconciliations by Date or Check Number. You can change this setting on individual reconciliations. |
| Recalculate Estimated Cost on Creation of Linked Transactions | Choose a setting to recalculate estimated costs and the resulting gross profit as a transaction moves through the sales cycle. For example, to recalculate when a sales order is converted to an invoice. |

## Other Item Preferences {#bridgehead_N1388006}

| Field | Description |
| --- | --- |
| Matrix Item Name/Number Separator | Choose the character you want to use in your matrix subitem names. This character appears between the item name and options for each subitem. |
| Gift Certificate Auth Code Generation | Choose between the following:
-   **System Generated** - NetSuite generates an authorization code when a gift certificate is sold, requiring no manual tracking of codes. These codes can be long, but this is the preferred method unless you have pre-printed certificates or cards.
-   **Enter on Order** - You can manually enter an authorization code on an order when a gift certificate is sold. This can be helpful if there are numbers printed on cards or certificates, or if you want to use your own numbering system. It can be difficult, however, to remember which number comes next.
-   **Add on Item** - You can enter authorization codes on the gift certificate item record. This is helpful if you're tracking physical cards or certificates before they're sold. If you're using your own numbering system, it's helpful because you don't duplicate or skip authorization codes. After the certificate is sold, you can then select the appropriate code.

 |
| Enforce Minimum Quantity on Return Authorizations | Enable this option to indicate that items can be returned only if the quantity returned is equal to or greater than the minimum quantity attribute on the item record. For example, to save a return authorization for an item that has a minimum quantity of five, you must enter a return quantity of five or more. See [Sales Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2172023.html) for more information about item minimum quantity. |
| Send Gift Certificate Email | When a gift certificate is sold at cash sale or an invoice, the gift certificate is sent to the provided email. This preference is enabled by default. |
| Make Gift Certificate Fields Required on Transaction Lines | After you disable the Send Gift Certificate Email preference, you can disable this preference to no longer include gift certificate fields on transaction lines. |

### Related Topics:

-   [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html)
-   [Order Management Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html)
-   [Projects Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3769284587.html)
-   [Time & Expenses Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html)
-   [Approval Routing Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391689.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
