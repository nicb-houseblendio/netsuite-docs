---
id: "section_N1388149"
type: "section"
title: "Order Management Accounting Preferences"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Features and Preferences > Accounting Preferences > Order Management Accounting Preferences"
parent: "section_N1384948"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1388149.html"
anchors: ["bridgehead_N1388312", "bridgehead_N1390085", "bridgehead_N1390212", "bridgehead_N1390473", "bridgehead_N1390583", "bridgehead_N1390949", "bridgehead_N1390978", "bridgehead_N1391052", "bridgehead_N1391167", "bridgehead_158394484605", "bridgehead_163169880548", "bridgehead_0207105126", "bridgehead_3887104251", "bridgehead_158394548043"]
sha256: "5a431e3fbbe06fca3af632c69964c4200aadeeb0623349f93f678ef7c88f9943"
---

The following types of preferences are available on the Order Management subtab of the Accounting Preferences page:

-   [Sales Orders](#bridgehead_N1388312)
    
-   [Picking/Packing](#bridgehead_N1390085)
    
-   [Fulfillment](#bridgehead_N1390212)
    
-   [Invoicing](#bridgehead_N1390473)
    
-   [Drop Shipment & Special Orders](#bridgehead_N1390583)
    
-   [Purchasing](#bridgehead_N1390949)
    
-   [Receiving](#bridgehead_N1390978)
    
-   [Returns](#bridgehead_N1391052)
    
-   [Transfer Orders](#bridgehead_N1391167)
    
-   [Vendor Bills](#bridgehead_158394484605)
    
-   [Supply Change Orders](#bridgehead_163169880548)
    
-   [Waves](#bridgehead_0207105126)
    
-   [Work Orders](#bridgehead_3887104251)
    
-   [Intercompany Inventory Transfer](#bridgehead_158394548043)
    

## Sales Orders {#bridgehead_N1388312}

| Field | Description |
| --- | --- |
| Default Sales Order Status | Choose your default status for sales orders:
-   Choose **Pending Approval** if your company uses the approval process for sales orders.
-   Choose **Pending Fulfillment** if your company doesn't use the approval process for sales orders. You can still choose a sales order status at the time you enter a transaction.

 |
| Require Re-approval on Edit of Sales Order | Choose to require re-approval when someone edits a sales order that was previously approved. Partially fulfilled sales orders are not affected by this preference. When a sales order is partially fulfilled, the status can't be changed back to pending approval. Note: If you edit a sales order when using a role with permission to approve sales orders, a sales order status isn't set to the Pending Approval status. |
| Send Email Confirmation when Sales Order Canceled | Check this box if you want an email sent to the customer when a sales order is canceled. |
| Default Location for Sales Orders | Select a default location to associate with sales orders. You can change the location on sales orders you enter as needed. |
| Item Commitment Transaction Ordering | Select one of the following to determine which order has items committed to it when there is an open quantity.

-   **Order by Expected Ship Date** - Commits only based on the latest expected ship date.
-   **Order by Order Priority** - Commits based on set customer priority regardless of transaction date or expected ship date. When the Item Commitment Transaction Ordering preference is set to Order by Order Priority, then an Order Priority column is displayed on forms for work orders, sales orders, and transfer orders. NetSuite uses this field to calculate the order priority for allocation.
-   **Order by Transaction Date** - Commits only based on the latest transaction date.

 |
| Perform Item Commitment After Transaction Entry | Check this box to enable NetSuite to automatically allocate items based on the preference under Item Commitment Transaction Ordering. When this preference is enabled, NetSuite performs automatic inventory allocation when new item quantities become available. By default, when this preference isn't set, you must manually choose which orders to allocate items to. |
| Automatically Set to Firm Committed Quantities in a Wave | If you use Warehouse Management, you can set this preference to automatically check the Commitment Confirmed box for transaction lines of orders that you include in a wave. When the Commitment Confirmed box is checked, you can't reallocate the committed quantities to a different order. |

## Picking/Packing {#bridgehead_N1390085}

| Field | Description |
| --- | --- |
| Always Print Kit Items on Picking Tickets | Choose to print individual kit items on picking tickets. When you print kit items, each picking ticket shows individual items that make up a kit item. Showing each item in the kit item gives your employees more specific information to fulfill an order. |
| Show Uncommitted Items on Picking Tickets | Check this box if you prefer for picking tickets to include items that are not yet committed to the order. This means that the picking ticket can include items that are not yet available to be picked. Clear this box if you prefer that picking tickets include only committed items that are available to be picked. |
| Show Non-Inventory Items on Printed Forms | Check this box to show non-inventory items such as services or discounts on picking tickets and packing slips. |
| Name for Picked Status | Enter a name to rename the status for orders that have been picked. Picked orders are orders with some or all of the items pulled from inventory, but are not yet packed or shipped. |
| Name for Packed Status | Enter a name to rename the status for orders that have been packed. Packed orders have items that have been picked from inventory and packaged to be shipped to the customer. |
| Name for Shipped Status | Enter a name to rename the status for orders that have been shipped. Shipped orders have items that have been picked from inventory, packed, and sent to the customer. |
| Show Additional Items on Packing Slips | Make a selection for this preference to determine how items show on packing slips. Options available for this preference are as follows:
-   **None** - Show only items being fulfilled in the shipment.
-   **Unfulfilled Items on Order** - Show only unfulfilled and partially fulfilled items on the packing slip. Line items that are completely fulfilled don't show on the packing slip.
-   **All Items on Order** - Show all ordered items. Any quantity yet to be fulfilled shows in the Remaining/Back Ordered column. Line items that are completely fulfilled show on the packing slip. Note: Choosing this option causes non-inventory items to show on packing slips even if the Show Non-Inventory Items on Printed Forms preference isn't enabled.

 |
| Show Drop Ship Items on Packing Slips | Check this box to have packing slips include drop-ship items. Clear this box to leave drop-ship items off packing slips. |
| If you use Warehouse Management, you can set the following preferences: |
| Use Pick to Clean Process at Locations Using Warehouse Management | Check this box to prioritize picking from bins that you can empty first, before bins with larger quantities. |
| Show Additional Pick Task Columns | Check this box if you want to display the two additional columns on pick task subrecords. In these columns, you can add more details for each pick task line. |

## Fulfillment {#bridgehead_N1390212}

| Field | Description |
| --- | --- |
| Limit Status on Packing Slip Queue | Select Picked or Packed to filter the packing slip list by order status. |
| Fulfill Based on Commitment | Select from the following to set item fulfillment restrictions:
-   **Limit to Committed** - This setting restricts fulfillment to a quantity not greater than the quantity committed. Orders default to fulfill only the committed items and quantities and the fulfillment quantity and **can't** be increased beyond the committed quantity. Other items that are not committed don't show on the fulfillment and **can't** be added.
-   **Allow Uncommitted** - This setting enables you to fulfill a quantity greater than the quantity committed on an order. This setting may cause your quantity on hand count of the item to be negative and make tracking item commitment and stock status more difficult. Orders default to fulfill only the committed items and quantities. The fulfillment quantity, however, can be increased beyond the committed quantity and other items that are not committed can be added.
-   **Ignore Commitment** - This setting places no restrictions on fulfillment that are based on commitment. Orders default to fulfill all unfulfilled items and quantities without regard to commitment.

Note: If you also enable the Allow Overage on Item Fulfillments preference, Fulfill Based on Commitment should be set to Ignore Commitment or Allow Uncommitted. |
| Default Items to Zero Received/Fulfilled | Enable this preference to default items to zero quantity when you open a fulfillment or receipt transaction. Then, you mark the items you want to fulfill or receive on the form. Disable this preference to default items to the full quantity when you open a fulfillment or receipt transaction. Then, you clear the items you don't want to fulfill or receive on the form. |
| Allow Overage on Item Fulfillments | Enable this preference to be able to enter a quantity larger than the quantity remaining for an item on a fulfillment. Disable this preference to limit the quantity fulfilled to the quantity remaining on the fulfillment. If you enable Allow Overage on Item Fulfillments, the Fulfill Based on Commitment preference should be set to Ignore Commitment or Allow Uncommitted, if enabled. |
| Filter Bulk Fulfillment Page by Location | Check this box to filter your fulfillment list by the location identified on the order. For example, if you select Atlanta in the location filter of the fulfillment page and click Mark All, NetSuite fulfills only items with the Atlanta location chosen. Note: If you disable this preference, all items on orders you mark for fulfillment are fulfilled from the location in the header of the bulk fulfillment, regardless of the location identified on the order. |
| Send Order Fulfilled Confirmation Emails | Enable this preference to send a confirmation email showing the total quantity shipped upon fulfillment. The email is sent to the customer email address identified on the sales order.

-   If you use the Advanced Shipping feature, the email is sent when the order is fulfilled.
-   If you don't use the Advanced Shipping feature, the email is sent when the order is billed.
-   If you use the Pick, Pack, and Ship feature, the email is sent when the order is shipped.

 |
| Use Web Site Template for Fulfillment Emails | You can enable a preference to use the same template to generate confirmation email for both web store and non-web store orders. Enabling this preference gives your confirmation email a consistent appearance. Note: You must enable the Web Store and Advanced Site Customization features to use this preference. To enable these features, go to _Setup > Company > Enable Features_. On the Web Site subtab, check the Web Store box and the Advanced Site Customization box, then click Save. **When you enable this preference, you can customize the email template.** |
| Manufacturing Issue Based on Commitment | Select from the following to set assembly item build restrictions:

-   **Limit to Committed** - This setting restricts the build to a quantity not greater than the quantity committed on the work order.
-   **Allow Uncommitted** - This setting enables you to build a quantity greater than the quantity committed on the work order. In this case, when the build is saved, the items on the work order are still uncommitted.
-   **Ignore Commitment** - This setting places no restrictions on the build that are based on commitment.

 |
| Update Transaction Date Upon Fulfillment Status Change | Enable this preference to pick items in one accounting period and ship in another accounting period. For more details, read [Fulfilling Orders Across Multiple Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3997655525.html). Note: You must enable the Pick, Pack and Ship feature to use this preference. |
| Create Item Fulfillment at Locations Using Warehouse Management | Select your preference for item fulfillment creation:

-   **Per Order** - Generate an item fulfillment for each released order
-   **Per Order Line** - Generate an item fulfillment for each line item of a released order

 |

## Invoicing {#bridgehead_N1390473}

| Field | Description |
| --- | --- |
| Show Unfulfilled Items on Invoices | Check this box to have your invoices show items that have yet to be fulfilled. |
| Invoice in Advance of Fulfillment | Check this box to invoice your customers for the full amount prior to the complete fulfillment of an order. With this preference, you can invoice your customers in advance for an entire order that is shipped in parts. Clear this box to limit the quantity fulfilled to the quantity remaining on the fulfillment. |
| Convert Absolute Discounts to Percentage | Set this preference to convert currency-amount discounts into percentage discounts spread across several invoices. Note: The discount must be applied at the transaction level, not the line level. When this preference is enabled, a sales order billed on multiple invoices has the discount applied evenly to all bills for that order. The discount must be applied at the transaction level and must be a currency amount. If this preference isn't enabled, the entire discount is applied only to the first bill. For example, you use Advanced Billing to enter a sales order for $1,000 that includes a transaction-level discount of $100. The sales order is billed in 10 monthly installments of $100. When you bill the order, the first invoice shows a 10% discount in the amount of $10.00, and each of the next nine bills shows a 10% discount in the amount of $10.00. To help minimize rounding issues, NetSuite calculates the value of percentage discounts on sales orders and shows the equivalent currency-amount discounts on invoices. When a line item on a sales order has a billing schedule and you apply a line-level percentage discount, the invoice generated shows the discount as a currency amount. For example, you enter a sales order for Item A worth $600 with a billing schedule of 3 months. You then add a line-level discount of 10%, which is equivalent to $60 (10% x $600). NetSuite distributes this $60 evenly into the 3 months, so each invoice gets a $20 discount. This calculation helps avoid small discrepancies due to percentage rounding. |
| Base Invoice Date on Billing Schedule Date | This preference determines how the date and posting period are set on invoices and cash sales produced from billing schedules.
-   Check this box to generate the date and posting period of an invoice or cash sale from the date and posting period of the next billing schedule instance. For example:
    -   Today is 3/1/05.
    -   The next billing date for order #123456 is 6/1/05.
    -   Today, you click Next Bill on order #123456.
    -   The date of the bill is 6/1/05.
-   Clear this box to define the date and posting period of invoices and cash sales when you bill them. You choose the date and posting period in the fields on the Bill Sales Order page.

 |

## Drop Shipment & Special Orders {#bridgehead_N1390583}

| Field | Description |
| --- | --- |
| Drop Ship P.O. Form | Select the form you would like to use by default for drop-ship purchase orders. If you enable this preference, only vendors associated with an item show in the Vendor list. Otherwise, the Vendor field shows all vendors. |
| Automatically Email Drop Ship P.O.s | Check this box to have purchase orders for drop-ship items automatically emailed to the preferred vendor. To use this preference, you must enter the preferred vendor's email address on that vendor's record. |
| Queue Drop Ship P.O.s for Printing | Check this box to have your drop-ship purchase orders queued for printing. |
| Automatically Fax Drop Ship P.O.s | Check this box to have your purchase orders for drop-ship items automatically faxed to the preferred vendor. To use this preference, you must enter the preferred vendor's fax number on that vendor's record. |
| Limit Vendor List on Items | Set this preference to filter the vendors available on sales orders and the Order Items page. If you enable this preference, only vendors associated with an item show in the Vendor list. If this preference is disabled, the Vendor field shows all vendors. For more information, see [Setting Up Drop Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239482.html). |
| Include Committed Quantities | When you need to drop ship or special order an inventory item and part of the ordered quantity is unavailable, the quantity ordered from the vendor depends on your setting for this preference.
-   When you disable this preference, clicking the Drop Ship/Special Order link creates a purchase order for only the backordered quantity.
-   When you enable this preference, clicking the Drop Ship/Special Order link creates a purchase order for the entire quantity ordered.

 |
| Update Drop Ship Order Quantities Automatically Prior to Shipment | Enable this preference to automatically update the quantity of a drop-ship item on linked transactions when a sales order or purchase order quantity is changed. When a drop-ship item quantity is changed on an existing sales order or purchase order before it's shipped, NetSuite examines the quantity on the linked transaction. If the quantity on the linked transaction doesn't match, NetSuite adjusts the corresponding quantity to match. For example, a sales order you entered shows a quantity of 10 units of drop-ship item #AB1001. The purchase order generated from that sales order also shows 10 units of item #AB1001. The next day, the order is changed and you reduce the sales order quantity to 8 units of item #AB1001. With this preference enabled, after you save the new quantity on the sales order, NetSuite examines the linked purchase order to sync the quantity of items being ordered. The purchase order is automatically updated to show 8 units of drop-ship item #AB1001. This preference applies only to assembly items and inventory items. Important: This preference applies only if the following conditions are met: The sales order line has not been fulfilled. The purchase order line has not been received or marked shipped. Neither the sales order or purchase order line have been manually closed. Disable this preference if you don't want to update the quantity of a drop-ship item on linked transactions when a sales order or purchase order quantity is changed. Then, when the quantity on linked forms doesn't match, the quantity remains unchanged and isn't updated to match. Note: When the sales order and purchase order quantities don't match, the item is no longer treated as a drop shipment and your inventory may be affected. Note: If you use the Multiple Units of Measure feature and enable the Update Special Order Quantities Automatically Prior to Shipment preference, note that you should use the same unit of measure on both the purchase order and sales order for an item. If you use different units of measure, it can cause errors due to rounding for differences greater than five decimal places. This preference defaults to be disabled. |
| Drop Ship Fulfillment Quantity Validation | If you use the Advanced Shipping and Drop Shipments & Special Orders features, when you fulfill or receive orders you can receive a warning or prevent users from processing orders with unequal amounts. Choose a setting for handling unequal quantities on linked sales orders and purchase orders that include drop-ship items:

-   **Allow unequal quantities** - This setting lets you fulfill without a warning even if linked transaction quantities are not equal.
-   **Warn only for unequal quantities** - This setting causes a warning to be displayed when you fulfill orders for linked transactions that have unequal quantities. This setting doesn't prevent processing after the warning is shown.
-   **don't allow unequal quantities** - This setting prevents you from fulfilling and when linked transaction quantities are not equal.

If this preference is set either to warn or allow, then transactions with unequal quantities remaining are fulfilled from inventory. This preference defaults to use the **Warn only for unequal quantities** setting. This preference applies only to inventory and assembly items. |
| Allow Both Mark Shipped Fulfillments and Receipts on a Drop Shipment Line | If you use the Advanced Receiving, Advanced Shipping, and Drop Shipments & Special Orders features, choose a setting for handling receipts and mark-shipped fulfillments with drop-ship orders:

-   **Allow** - This setting lets you do the following:
    -   Create a receipt against a drop-ship purchase order line that already has a mark shipped fulfillment line **without any warning**.
    -   Create a mark-shipped fulfillment against an order line that already has a receipt entered against it **without any warning**.

Warning: Drop shipment items that are received into inventory do have accounting impact and are committed to orders when they're received. Creating these transactions may cause imbalances in quantities and accounts.

-   **Warn only** - This setting does the following:
    -   Warns you when you try to create a receipt against a drop-ship purchase order line that already has a mark shipped fulfillment line. The warning notes that creating these transactions does have an inventory impact.
    -   Warns you when you try to create a fulfillment against an order line that already has an item receipt with inventory and accounting impact entered. The warning notes that creating a mark shipped fulfillment against this order line may cause imbalances in quantities and accounts.
-   **don't allow** - This setting does the following:
    -   Prevents you from creating a receipt against a drop-ship purchase order line that already has a mark shipped fulfillment line.
    -   Prevents you from entering a fulfillment against an order line that already has an item receipt with inventory and accounting impact.
    -   If an order is received as the first step after the purchase order for the drop ship sales order is created, you can no longer click Mark Shipped.
    -   After drop-ship items on an order have been received, you can change the quantity but you can no longer mark items shipped on that order.
    -   This preference defaults to use the **Warn only** setting. This preference applies only to inventory and assembly items.

 |
| Update Special Order Quantities Automatically Prior to Shipment | Enable this preference to automatically update the quantity of a special order item on linked transactions when a sales order or purchase order quantity is changed. When a special order item quantity is changed on an existing sales order or purchase order before it's shipped, NetSuite examines the quantity on the linked transaction. If the quantity on the linked transaction doesn't match, NetSuite adjusts the corresponding quantity to match. For example, a sales order you entered shows a quantity of 10 units of special order item #AB1001. The purchase order generated from that sales order also shows 10 units of item #AB1001. The next day, the order is changed and you reduce the sales order quantity to 8 units of item #AB1001. With this preference enabled, after you save the new quantity on the sales order, NetSuite examines the linked purchase order to sync the quantity of items being ordered. The purchase order is automatically updated to show 8 units of special order item #AB1001. This preference applies only to assembly items and inventory items. Important: This preference applies only if the following conditions are met: The sales order line has not been fulfilled. The purchase order line has not been received or marked shipped. Neither the sales order or purchase order line have been manually closed. Disable this preference if you don't want to update the quantity of a special order item on linked transactions when a sales order or purchase order quantity is changed. Then, when the quantity on linked forms doesn't match, the quantity remains unchanged and isn't updated to match. Note: When the sales order and purchase order quantities don't match, the item is no longer treated as a special order and your inventory may be affected. This preference defaults to be disabled. |

## Purchasing {#bridgehead_N1390949}

| Field | Description |
| --- | --- |
| Allow Expenses on Purchases | Check this box to add expenses to purchases. This adds an Expenses subtab to your order pages. With this preference, you can add expenses for things like rental fees and delivery of drop-ship items to your purchase orders. You can then bill these expenses to a specific customer. |
| Allow Purchase of Assembly Items | Check this box to add assembly items to purchase orders, vendor bills, checks, credit card transactions and vendor credits. You can also define purchase pricing on assembly item records. If you enable this preference and use the Demand Planning feature, demand plans can create purchases for assemblies. |
| Default Location for Purchase Orders | Select a default location to associate with purchase orders. You can change the location on purchase orders you enter as needed. |
| Maximum Purchase Lines to Consolidate | Enter a value in this field to define the maximum number of lines to consolidate on purchase orders. This definition applies in the following cases:
-   when you submit multiple orders on the Order Requisitions page and items from one or more requisitions are combined on a single purchase order.
-   when you submit multiple orders on the Order Items page and items from one or more planned orders are combined on a single purchase order.

This value defaults to 10 but you can enter a number up to 250. Setting the value of this field to 0 has the following effect:

-   On the Order Requisitions page, all requisition lines for a vendor are consolidated into a single purchase order.
-   On the Order Items page, all planned order lines for a vendor are consolidated into a single purchase order.

 |
| Allow Default Email on Purchase Orders using SuiteFlow Approval Routing | Choose a setting to determine how NetSuite handles email generated when the To Be Emailed box is checked on a purchase order.

-   **don't Allow** - Approval Routing is enabled for this transaction. Please contact your workflow administrator about enabling email processing within an approval routing workflow.
-   **Warn Only** - NetSuite warns you before sending an email to the designated recipient in addition to email produced by the approval routing workflow. Email is generated Upon saving the transaction.
-   **Allow** - Upon saving the transaction, no warning is given before NetSuite sends an email to the designated recipient in addition to email produced by the approval routing workflow.

 |
| Default Number of Request for Quote Pricing Tiers. | Enter the number of pricing tiers you prefer to appear on a request for quotes by default. You can change this number on an RFQ as needed. |

## Receiving {#bridgehead_N1390978}

| Field | Description |
| --- | --- |
| Bill in Advance of Receipt | Choose to bill purchase orders before you receive them. |
| Allow Overage on Item Receipts | Check this box to enter a quantity larger than the quantity remaining for an item on an item receipt. Clear this box to limit the quantity received to the quantity remaining on the item receipt. |
| Default Receiving Exchange Rate | Select one of the following in this field:
-   **Use Purchase Order Exchange Rate** - The default value of the exchange rate on the order line is the purchase order exchange rate.
-   **Use Exchange Rate at the Time of the Receipt** - The default value of the exchange rate on the order line is the exchange rate based on the receipt date.

Then, based on your setting, the correct rate defaults to show in the Exchange Rate field on receipts. |
| Use Purchase Order Rate on Bills | When the purchase order has multiple item receipts, the **Use Purchase Order Rate on Bills** accounting setting determines the bill rate. If you enable the **Use Purchase Order Rate on Bills** preference, the vendor bill rate uses the purchase order rate. If you disable this preference, the vendor bill rate uses the highest item receipt rate instead. You can find the **Use Purchase Order Rate on Bills** preference at Setup > Accounting > Preferences > Accounting Preferences > (Administrator). Note: This preference applies to the Item Rate field, not the Exchange Rate field. |
| Landed Cost Allocation per Line | When enabled, you can specify landed cost allocation amounts on a per-line basis on transactions and receipts, rather than distributing the cost based on an allocation method at a transaction level basis. For every item received, a landed cost sub-record can store custom values, which are reflected in inventory valuation reports. When this preference is enabled, all new item receipts, credit card charges, vendor bills, and checks default to use landed cost per line. You can change this default option by clearing the box to disable Landed Cost Allocation per Line when entering new transactions. |

## Returns {#bridgehead_N1391052}

| Field | Description |
| --- | --- |
| Default Return Auth. Status | Choose your default return authorization status. You can choose any return authorization status at the time you enter a transaction.
-   Select **Pending Approval** if your company uses the approval process for return authorizations.
-   Select **Pending Fulfillment** if your company doesn't use the approval process for return authorizations.

 |
| Refund in Advance of Return | Enable this preference to permit a purchase to be refunded before the item is returned. |
| Restock Returned Items | Enable this preference to check the Restock box on receipts by default. Clear this box to require the Restock box to be checked on each receipt. |
| Write-Off Account for Returns | Select the account to post to when you write off returned items. |
| Default Vendor Return Auth. Status | Choose the default status for vendor return transactions:

-   Select **Pending Approval** if your company uses the approval process for vendor return authorizations.
-   Select **Pending Fulfillment** if your company doesn't use the approval process for vendor return authorizations.

The status you select in this field shows by default in the status field of new vendor return authorizations you enter. You can choose another return authorization status at the time you enter a transaction. |
| Credit in Advance of Vendor Return | Check this box to enter vendor credit for the full amount of the return prior to the complete return of an order. With this preference, you can enter vendor credit in advance for an entire order that is returned in parts. |

## Transfer Orders {#bridgehead_N1391167}

| Field | Description |
| --- | --- |
| Default Transfer Order Status | Select one of the following to default on manual orders:
-   **Pending Approval Firm** - By default, require that someone with permission approves the order before it's processed. Firmed transfer orders are not available to be rescheduled or cancelled.
-   **Pending Approval Open** - By default, require that someone with permission approves the order before it's processed. Transfer orders that are Open, not Firmed, are available to be rescheduled or canceled. Recommendations for Open transfer orders are removed for each demand planning run.
-   **Pending Fulfillment** - By default, send transfer orders directly to the fulfillment queue without requiring further approval.

 |
| Generate Transfer Orders in Supply Planning | Select one of the following to default on auto-generated transfer orders:

-   **Generate in Pending Approval Firm Status** - By default, require that someone with permission approves the order before it's processed. Firmed transfer orders are not available to be rescheduled or cancelled.
-   **Generate in Pending Approval Open Status** - By default, require that someone with permission approves the order before it's processed. Transfer orders that are Open, not Firmed, are available to be rescheduled or cancelled. Recommendations for Open transfer orders are removed for each demand planning run.
-   **Generate in Pending Fulfillment Status** - By default, send transfer orders directly to the fulfillment queue without requiring further approval.

 |
| Use Item Cost as Transfer Cost | Choose one of the following to set how the transfer price functions on item receipts:

-   Check this box to use the transfer price as a declared shipping value for reference only, such as for insurance or international shipping.
    -   The transfer price isn't a charge for the destination location.
    -   The transfer price doesn't affect the Cost of Goods Sold (COGS) on transactions.
    -   The transfer price defaults to show the value in the Transfer Price field of item records. This value can be changed on individual transfer orders.
    -   Partial fulfillment and receipt of transfer orders is allowed, but you can't receive more than you have fulfilled as of any date. For example, if you have fulfilled 10 widgets out of 20 on a transfer order, you can't receive 12 widgets on that order.
    -   This preference also applies to items that use the **Standard** costing method. When enabled, the item's standard cost at the source location is used as the transfer cost on transfer orders for those items.
-   Clear this box to use the transfer price shown on the transfer order as the item cost on the item receipt.
    
    -   Any difference between the actual cost and the transfer price posts to a Gain/Loss account when the item is shipped.
    -   The transfer price and the Gain/Loss account are defined on each item record.
    -   The transfer price defaults to show the value in the Transfer Price field of item records. This value can be changed on individual transfer orders.
    
    For a detailed example, read [Setting Transfer Order Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2310077.html).

Note: This preference can also be set on individual transfer orders when they're created. Individual orders default to show the setting chosen in this field. The setting can't be changed and is permanent after the order is saved (or after approval if you use approval routing.) |
| Default Number of Request for Quote Pricing Tiers | Enter the number of pricing tiers you prefer to appear on a request for quotes by default. You can change this number on an RFQ as needed. For more information, see [Request for Quote Feature Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4212772813.html). |
| Default Transfer Order Incoterms | Choose a default transfer order incoterm of Ex Work (EXW) or Delivered at Place (DAP). For more information, see [In-Transit Ownership](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4813066512.html). |
| Default Lead Time Between Locations |  |

## Vendor Bills {#bridgehead_158394484605}

| Field | Description |
| --- | --- |
| Default Vendor Bill Status | Select a default vendor bill status of either Approved or Pending Approval. For more information, see [Setting the Default Vendor Approval Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2374176.html). |

## Supply Change Orders {#bridgehead_163169880548}

| Field | Description |
| --- | --- |
| Default Supply Change Order Status | Select a Default Supply Change Order Status to either Pending Approval or Approved. |
| Generate Action Messages For Previously Rejected Change Orders | Check this box to generate action messages for change orders that were previously rejected. |

## Waves {#bridgehead_0207105126}

| Field | Description |
| --- | --- |
| Default Status | Select a default wave status of either **Released** or **Pending Release**. For more information, see [Creating Wave Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1548078883.html). |
| Default Picking Type | Select a default picking type status among the following options: **Single Order**, **Multiple Orders**, or **Bulk Picking**. For more information, see [Creating Wave Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1548078883.html). |
| Allow Pick Decomposition on Waves | Check this box to automatically check the **Apply Pick Decomposition** box, instead of checking it during each wave creation or generation. For more information, see [Pick Task Decomposition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0207120728.html). |
| Update quantity of re-released pick task lines | Check this box to update existing pick task lines in **Ready** status to reflect newly committed back-ordered quantities when you re-release the order line. When this box isn't checked and you re-release an order line, a new wave is created that includes the newly committed quantities. For more information, see [Re-releasing Lines with Backorders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0803020225.html). |

## Work Orders {#bridgehead_3887104251}

| Field | Description |
| --- | --- |
| Allow Purchase of Assembly Items | Enable this preference to add assembly items to purchase orders, vendor bills, checks, credit card transactions and vendor credits. You can also define purchase pricing on assembly item records. |
| Automatically Fill Actual Production Start and End Dates | Check this box to have actual production start and end dates fill in automatically. If you prefer to control actual production dates manually, and don't want NetSuite to calculate production dates, clear this box to disable this feature. However, you'll then need to enter actual production dates manually on each work order. For more information, see [Actual Production Start or End Dates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157832628099.html). |
| Allow Overage on Work Order Transactions | Check this box to be able to enter a quantity larger than the quantity remaining for an item on a work order. Clear this box to restrict the amount to a maximum of the amount on the work order. |
| Default Work Order Status | Choose one of the following to define the default status of new work orders you manually create:
-   **Firm Planned** - Firmed planned work orders are **not** deleted before supply planning runs. No components are committed regardless of commit option settings.
-   **Open Planned** - Open planned work orders are deleted before supply planning runs. No components are committed regardless of commit option settings.
-   **Released** - No transaction has posted and no activities have been recorded. Components can be committed based on commit option settings. (Previously this status was called Pending Build.)

For details about work order statuses, read [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html). |
| Create Work Orders in Supply Planning | Select one of the following to define the default for supply planning work orders:

-   don't Generate
-   Generate in Planned Firm Status
-   Generate in Planned Open Status
-   Generate in Released Status

For details about work order statuses, see [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html). |
| Check Completed Quantity in Prior Operations During Operation Completion | Set this preference to validate that routing operation sequences are always followed in accordance with the work order. When the preference is enabled, NetSuite ensures that the correct quantity is completed for each operational step before permitting the work order to continue being processed. For example, if Step #2 of your routing requires 5 widgets that are created during Step #1, you can enable this preference and NetSuite verifies that 5 widgets are completed during step #1 before Step #2 can begin. Such verification helps prevent problems due to out-of-sequence processing. For orders completed across multiple days or shifts, partial quantities can be logged over time. |
| **Operation** | **Qty Day 1** | **Qty Day 2** | **Qty Day 3** | **Qty Day 4** |
| Operation 10 | 50 | 30 | 15 | 5 |
| Operation 20 | 40 | 40 | 5 | 15 |
| Operation 30 | 35 | 45 | 0 | 20 |
| Choose from the following settings:

-   **No Verification** - Choose this setting if you don't want to receive verification warnings.
-   **Require Confirmation before Saving** - Choose this setting to receive verification warnings. NetSuite permits the completed quantity to be greater than the predecessor completed quantity after the warning is acknowledged.
-   **don't Allow Saving** - Choose this setting to require that the completed quantity isn't greater than the predecessor completed quantity.

This field defaults to the No Verification selection. Note: Completion validation doesn't function when the completion transaction is edited or deleted. |
| Show Planned Capacity on Work Orders | Use this preference to automatically create planned time entries when processing manufacturing work orders. This preference determines the default setting for the Show Planned Capacity field on new work orders being created. When this preference is enabled, work orders display a Planned Time subtab. NetSuite generates planned time entries showing the amount of time being allocated to each work center per day. Note: These generated planned times can't be edited. |
| Default Scheduling Method | Choose either **Forward** or **Backward** scheduling. Your selection here shows by default in the Scheduling Method field on new work orders you enter. For more details, read [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html). |

## Intercompany Inventory Transfer {#bridgehead_158394548043}

| Field | Description |
| --- | --- |
| Update Intercompany Order Quantities Automatically Prior to Shipment | Enable this preference to automatically update the quantity of an intercompany purchase order item when the quantity is changed on the linked intercompany sales order. This preference applies only to assembly items and inventory items. When the quantity is changed on an intercompany sales order item before it's shipped, NetSuite examines the quantity on the linked intercompany purchase order. If the quantity on quantity on the linked intercompany purchase order doesn't match, NetSuite adjusts the corresponding quantity to match the sales order. For example, an intercompany sales order you entered shows a quantity of 10 units of item #AB1001. The intercompany purchase order generated from that sales order also shows 10 units of item #AB1001. The next day, the order is changed and you reduce the sales order quantity to 8 units of item #AB1001. With this preference enabled, after you save the new quantity on the sales order, NetSuite examines the linked purchase order to sync the quantity of items being ordered. The purchase order is automatically updated to show 8 units of item #AB1001. Important: This preference applies only if the following conditions are met: The sales order line has not been fulfilled. The purchase order line has not been received or marked shipped. Neither the sales order or purchase order line have been manually closed. Disable this preference if you don't want to update the quantity of an intercompany purchase order item when the quantity is changed on the linked intercompany sales order. Then, when the quantity on linked forms doesn't match, the quantity remains unchanged and isn't updated to match. |

### Related Topics:

-   [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html)
-   [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html)
-   [Projects Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3769284587.html)
-   [Time & Expenses Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391368.html)
-   [Approval Routing Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1391689.html)
-   [Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1384948.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
