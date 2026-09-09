---
id: "section_N1758108"
type: "section"
title: "Cost Estimate Types in NetSuite OneWorld"
branch: "order-management-reports"
category: "order-management"
breadcrumb: "Order Management > Order Management Reports > Estimating Gross Profit > Working with Cost Estimate Types > Cost Estimate Types in NetSuite OneWorld"
parent: "section_N1757575"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1758108.html"
anchors: []
sha256: "43a69f4ee22934ce596844b089731ccb960fa45a8485371adfcbd7ab62492984"
---

In NetSuite OneWorld accounts, cost estimate types are calculated according to the following:

-   **Average Cost** - uses a calculated average cost of the units purchased. When the Multi-Location Inventory feature is enabled, NetSuite calculates the average per location.
    
-   **Derived From Member Items** - works as in non-OneWorld accounts.
    
    (Total costs of items currently included in a kit. This Cost Estimate Type applies only to kits and sums the estimated costs of each item in the kit, based on each of their individual Cost Estimate Types. It uses the latest definition of the kit, not its historical definition.)
    
-   **Item Defined Cost** - converts the cost in the item record to the transaction currency using the exchange rate of the transaction subsidiary.
    
-   **Last Purchase Price** - calculates estimated cost based on the last purchase price of the item within the transaction subsidiary or location. The cost is converted to the transaction currency using the exchange rate of the transaction subsidiary.
    
    Note:
    
    The last purchase price as related to Gross Profit is affected by your setting for the preference **Include Landed Cost in Last Purchase Price**. Read more about this preference in [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html).
    
-   **Purchase Order Rate** - works as in non-OneWorld accounts.
    
    (Initially uses the Preferred Vendor Rate cost, and then after a purchase order is entered, this type uses the most recent actual purchase order rate. Special orders and drop-shipped items use this cost information.)
    
-   **Purchase Price** - converts the item's purchase price to the transaction currency using the exchange rates of the transaction subsidiary.
    
    Note:
    
    Items for purchase that are part of kits or assemblies must use the Purchase Price cost estimate type.
    
-   **Preferred Vendor Rate** - converts the item's purchase price for the transaction subsidiary's preferred vendor to the transaction currency using the exchange rates of the transaction subsidiary. If no rate is available, the Purchase Price estimate type is used.
    

### Related Topics

-   [Working with Cost Estimate Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757575.html)
-   [Available Cost Estimate Types for Each Item Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1758354.html)
-   [Modifying a Cost Estimate Type on an Item Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761469.html)
-   [Item Cost Estimate Type Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761708.html)
-   [Modifying a Cost Estimate Type on a Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1761948.html)
-   [Setting the Recalculate Estimated Cost on Creation of Linked Transactions Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757197.html)
-   [Granting the Override Estimated Costs on Transactions Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1757391.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
