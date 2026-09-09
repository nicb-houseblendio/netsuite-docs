---
id: "section_N1757784"
type: "section"
title: "Cost Estimate Type Descriptions"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Working with Cost Estimate Types > Cost Estimate Type Descriptions"
parent: "section_N1757575"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757784.html"
anchors: []
sha256: "4db7fc7e166a09bc036f5cbbcd25deb91694bd132503d467ed7f4d637d9a84a4"
---

When the Gross Profit feature is enabled, one or more cost estimate types become available for each item type, and a default is assigned to each item according to its type.

The following cost estimate types may be available. All of these types may be available on both items and transactions, except for the Custom cost estimate type, which is only available on transactions.

For a list of cost estimate types and how they are calculated in NetSuite OneWorld accounts, see [Cost Estimate Types in NetSuite OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1758108.html).

-   **Average Cost -** Uses a calculated average cost of the units purchased. When the Multi-Location Inventory feature is enabled, NetSuite calculates the average per location.
    
-   **Custom -** (Only available on transaction item lines.) Enables you to override estimated costs calculated through another cost estimate type.
    
    For example, an inventory item with a cost estimate type of Last Purchase Price defined on its item record however may require different cost estimates in some cases. In that case, a user with the Override Estimated Cost on Transactions permission could select Custom in the Cost Estimate Type field on the transaction item line and manually enter the estimated costs.
    
    Note the following:
    
    -   When SuiteScripts are used to set the estimated cost for a transaction line item, the Custom cost estimate type must be selected.
        
    -   When the Project Management feature is enabled and a sales transaction such as a sales order is created for a project, the Custom cost estimate type is automatically selected. The system populates the estimated cost based on the associated project costs.
        
    -   The Custom cost estimate type always preserves its value. This value is not reset when linked transactions are created from the original transaction, even when the Recalculate Estimated Cost on Creation of Linked Transactions preference is enabled.
        
-   **Derived from Member Items** - Total costs of items currently included in a kit. This Cost Estimate Type only applies to kits and sums the estimated costs of each item in the kit, based on each of their individual Cost Estimate Types. Uses the latest definition of the kit, not its historical definition.
    
-   **Last Purchase Price** - Uses the most recent purchase price of the item as determined by purchase order receipt transactions. If you make multiple purchases on the same day that use different rates, this value is the highest purchase price on that day, per location if applicable. When you use the Multi-Location Inventory feature, the last purchase price reflects the most recent receipt at any location. If you track inventory costing, NetSuite identifies the cost of the item based on your COGS settings.
    
    Note:
    
    The last purchase price as related to Gross Profit is affected by your setting for the preference **Include Landed Cost in Last Purchase Price**. Read more about this preference in [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html).
    
-   **Preferred Vendor Rate** - This option is only meaningful if the Multi-Vendor feature is enabled and multiple vendors supply the same item.
    
-   **Purchase Order Rate** - Initially uses the Preferred Vendor Rate cost, and then after a purchase order is entered, this type uses the most recent actual purchase order rate. Special orders and drop-shipped items use this cost information.
    
-   **Purchase Price** - Uses the purchase price paid for the item. If no price is entered, uses the most recent purchase price by default.
    

Note the following:

-   For accounts with the Multiple Currencies feature enabled, if you select a preferred vendor for an item, the price is shown in the currency selected on the vendor's record. If no preferred vendor is selected, the price is shown in the base currency.
    
-   For the purpose of calculating gross profit, costs exclude shipping and handling charges. The costing method (Average, FIFO, and LIFO) for an item determines the inventory valuation of an item used to calculate the actual gross profit that appears on financial reports.
    
-   For information about the available and default cost estimate types for different types of items, see [Available Cost Estimate Types for Each Item Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1758354.html).
    

### Related Topics

-   [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html)
-   [Available Cost Estimate Types for Each Item Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1758354.html)
-   [Modifying a Cost Estimate Type on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761469.html)
-   [Item Cost Estimate Type Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761708.html)
-   [Modifying a Cost Estimate Type on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761948.html)
-   [Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html)
-   [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
