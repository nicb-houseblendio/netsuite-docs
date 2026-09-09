---
id: "chapter_N3975465"
type: "chapter"
title: "Grid Order Management"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Grid Order Management"
parent: "book_4416276704"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3975465.html"
anchors: ["bridgehead_1491379510", "bridgehead_N3975786"]
sha256: "706ade65061d1da44e120004e0a82787d946fed75f641f4d426f7ff51d31cda4"
---

To get you started in using Grid Order Management, read the following topics:

-   [Grid Order Management Overview](#bridgehead_1491379510)
    
-   [Setting Up Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505109329.html)
    
    -   [Installing the Grid Order Management SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505109764.html)
        
    -   [Roles and Permissions for Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110051.html)
        
    -   [Limitations of Grid Order Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4273583432.html)
        
    -   [Setting Grid Order Management Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505110343.html)
        
-   [Setting Up Grid Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4273599062.html)
    
    -   [Setting Up Grid Matrix Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3977380.html)
        
    -   [Setting Up Grid Item Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3977514.html)
        
-   [Managing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274152949.html)
    
    -   [Entering Single Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978320.html)
        
    -   [Entering Multi-Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4664083498.html)
        
    -   [Editing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3978408.html)
        
    -   [Importing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499322449.html)
        
    -   [Viewing the Grid Matrix Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4809938296.html)
        
-   [Grid Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274156343.html)
    
    -   [Single Transaction Grid Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4810021848.html)
        
    -   [Bulk Grid Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4810023417.html)
        
    -   [Customizing the Grid Print Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1490941841.html)
        
    -   [Customizing the Printout using Advanced PDF/HTML Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4579351495.html)
        
    -   [Uploading Custom Grid Print Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1491207945.html)
        

## Grid Order Management Overview {#bridgehead_1491379510}

The Grid Order Management SuiteApp lets you enter and print orders in a grid format for assembly and inventory items. This SuiteApp enables you to create custom grid print templates and assign them to selected transactions.

As you create the grid order, you can view relevant item information such as the item name, location, available quantity, and price. This comprehensive grid format can save you time on order entry, increase order accuracy, and help you sell or fulfill orders faster.

This SuiteApp offers the following features:

-   **Grid Order Entry** - This feature lets you enter order transactions in grid format. Grid Order Entry is available for purchase orders, sales orders, transfer orders, and quotes. For more information, see [Managing Grid Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4274152949.html).
    
-   **Standard Grid Order Printing** - This feature lets you print transaction records in grid format for items added through Grid Order Entry. Standard Grid Order Printing is available only for purchase orders and sales orders. For more information, see [Standard Grid Order Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4579488225.html).
    
-   **Grid Print Templates** - This feature lets you print transaction records in grid format using tailorable grid templates. Grid Print Templates are available for cash sales, invoices, packing slips, picking tickets, purchase orders, quotes, and sales orders. For more information, see [Grid Print Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4579488425.html).
    
-   **Bulk Grid Printing** - This feature lets you print multiple transaction records that use grid print templates. Bulk Grid Printing is available for cash sales, invoices, packing slips, picking tickets, quotes, and transfer orders. For more information, see [Bulk Grid Printing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4810023417.html).
    

The following table shows the available features for each transaction record.

| Transactions | Available Features |
| --- | --- |
| Grid Order Entry | Standard Grid Order Printing | Printing Using Grid Print Templates | Bulk Grid Printing |
| --- | --- | --- | --- |
| Cash sale | N | N | Y | Y |
| Inventory adjustment | Y | N | N | N |
| Invoice | N | N | Y | Y |
| Packing slip | N | N | Y (2) | Y (2) |
| Picking ticket | N | N | Y | Y |
| Purchase order | Y | Y | Y | N |
| Quote | Y | N | Y | Y |
| Sales order | Y (1) | Y | Y | N |
| Transfer order | Y | N | N | Y |
| (1) Multi-grid order entry is available only for sales orders. (2) Grid print templates can be used to print packing slips for item fulfillments that were created from sales orders or transfer orders only. |

For better Grid Order Management performance, use Mozilla Firefox or Google Chrome web browsers.

## Grid Order Management SuiteApp Availability {#bridgehead_N3975786}

Grid Order Management is a managed and shared SuiteApp. Contact your NetSuite account manager to purchase the SuiteApp and to have it shared with your account for installation.

The Grid Order Management SuiteApp only supports English.

To install the SuiteApp, see [Installing the Grid Order Management SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1505109764.html).

### Related Topics

-   [Sales Orders and Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4416276704.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
