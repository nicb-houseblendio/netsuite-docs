---
id: "section_N1490669"
type: "section"
title: "Intercompany Inventory Items Guidelines"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Automated Intercompany Management > Setting Up Automated Intercompany Management > Intercompany Inventory Items Guidelines"
parent: "section_N1486610"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490669.html"
anchors: []
sha256: "3a307f6e32878b144ad6c0005bdc64e676ce2dda94baaf3c7f8104bdf08962bb"
---

You can transfer inventory items between subsidiaries. Inventory items do not have to be marked exclusively for intercompany transfers. You must, however, identify an inventory location on intercompany purchase orders and sales orders.

-   **Arm's length Inventory Transfers** - Use the purchase order/sales order workflow for arm's length transfers. Both the source and destination subsidiaries must have access to the inventory item.
    
-   **Non-Arm's Length Inventory Transfers** - (_Transactions > Inventory > Enter Intercompany Transfer Orders_). On the **Accounting** subtab of the item record, check the **Eliminate Intercompany Transactions** box for the account selected as the Gain/Loss Account. When the item cost is not used as the transfer cost, any difference between the cost and the transfer price posts to this account. NetSuite eliminates the gain/loss amount when you run intercompany elimination at period close.
    
-   **Intercompany Drop Ship** - If you use the Automated Intercompany Drop Ship feature, the Dropship Expense Account on item record defaults to a value. The value is the account specified in the **Default Expense Account** field on the Accounting Preference page, **Items/Transactions** subtab. You can override this account on an item record, if needed. The account used for the DropShip Expense Account must have the **Eliminate Intercompany Transactions** box checked.
    

### Related Topics:

-   [Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486928.html)
-   [Account Types and Intercompany Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1487157.html)
-   [Creating Intercompany Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1489768.html)
-   [Creating Intercompany Customers and Vendors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1490202.html)
-   [Customizing Standard Journal Entries for Intercompany Elimination](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1492223.html)
-   [Setting Up Automated Intercompany Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1486610.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
