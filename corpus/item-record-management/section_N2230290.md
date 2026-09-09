---
id: "section_N2230290"
type: "section"
title: "Serial Numbered Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Types > Serial Numbered Items"
parent: "chapter_N2222944"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html"
anchors: ["bridgehead_N2230521", "bridgehead_N2230563", "bridgehead_N2230551", "bridgehead_N2230584"]
sha256: "1a8931095102193b995b984baa6fdc4ae5f9a69b2abe18cbcd951e42c076ac26"
---

Serialized inventory is a way to track the purchase and sale of physical inventory items by assigning a serial number to each item. Serializing inventory lets you choose a specific serial numbered item to fulfill or receive an order. You can access the history of any serialized item to track the cost of the item, or check its status.

To use serialized inventory, enable the feature and set up item records. For more information, see [Enabling Serial Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230646.html) and [Entering Serialized Inventory Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230957.html).

After your serialized inventory is set up, you can manage serialized inventory to know the status of each serialized item. For more information, see the following:

-   [Track Serialized Inventory on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231339.html)
    
-   [Add New Serial Numbers to Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2231739.html)
    
-   [Adjusting Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235043.html)
    

On transactions, you can buy, sell, and process serialized items. For more information, see the following help topics:

-   [Receiving a Purchase Order With a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233116.html)
    
-   [Serialized Items on Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233510.html)
    
-   [Fulfilling a Sales Order with a Serialized Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2233933.html)
    
-   [Memorizing Transactions with Serialized Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234305.html)
    

You can include serialized items in assembly items, or build assemblies which have a serial number assigned to them. For more information, see [Building a Serialized Assembly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2234538.html).

Customer records show the serial numbers of items purchased by each customer to reference for returns or entering cases. For more information, see [Removing Serial Numbers on Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235383.html).

You can use the Multiple Units of Measure feature to assign units to serialized inventory.

Important:

Specific rules apply when you are working with serialized inventory units on transactions. For more information, see [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html).

You can use serialized inventory as members of Kit/Package items. For more information, see [Entering Serial and Lot Components on the Item Record for the Kit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225398.html).

## Serial Numbers on Transactions {#bridgehead_N2230521}

In the Serial/Lot Number field of a transaction, enter the serial number of the item. Separate each serial number with a space, comma or by pressing Enter after each one.

Note:

You must enter a serial number for each serialized item. For example, if you enter a quantity of 2, then you must enter two serial numbers.

You can choose multiple serial numbered items on transactions. Click the Select Multiple link next to the Serial/Lot Numbers field. A popup window opens that lists available serial numbers for the item. Click each item in the left pane to add it in the list right pane. Click Done to add all items in the right pane to the transaction.

By entering a specific serial or lot number, you are designating a specific item and NetSuite attempts to allocate the specific item for this order. If you don't enter a specific serial or lot number, NetSuite allocates only the specified quantity of this item to the order. Then, you can designate the specific serial or lot number for the item later.

## Serialized Items With Bin Management {#bridgehead_N2230563}

If you use Advanced Bin / Numbered Inventory Management, you can use serialized items with bin management. For more information, see [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html).

### Inventory Detail Selector {#bridgehead_N2230551}

With Advanced Bin / Numbered Inventory Management, you can click the Inventory Detail icon on transactions to add or remove serialized inventory. When you click the Inventory Detail icon, a popup window lets you select or edit the quantity and serial number appropriate for the transaction.

You can display the Inventory Detail icon in the following two ways:

-   **Arrow** ![Inventory Detail Arrow icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/InventoryDetailIconBlue.png) - The arrow icon indicates that the inventory detail is available for the item and needs to be configured. It appears only in edit mode for a transaction.
    
-   **Check mark** ![Inventory Detail Checkmark](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/InventoryDetailIconGreen.png) - The check mark icon indicates that you have already configured the inventory detail for this item. It appears in view mode for transactions, and in edit mode after you configure the inventory detail.
    

Permissions for the inventory detail selector are inherited from its parent transaction. For example, to edit the inventory detail from a sales order, you must have permission to edit the sales order. For more information, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

## Custom Information about Serialized Item Records {#bridgehead_N2230584}

Serialized inventory records can be customized with item number fields. These fields let you track information specific to each item or workflow unique to your business, such as quality control procedures or recall information.

When you receive serialized inventory from vendors, you can enter a memo or custom information about the item. To do so, click the Open icon next to the Serial number when viewing an item receipt.

After you enter information in custom item number fields, you can search for items on sales transactions based on the custom information. On sales transactions, you can search for serial numbers based on custom information from the inventory record. For more information, see [Customizing Lot or Serial Numbered Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2238963.html).

### Related Topics

-   [Avoiding Quantity Mismatches when Committing Numbered Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_96151731732.html)
-   [Searching for Serialized Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1508171622.html)
-   [Serial Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2230290.html)
-   [Item Records for Data Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163300696254.html)
-   [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html)
-   [Item Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2224824.html)
-   [Kit/Package Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2225190.html)
-   [Matrix Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2227654.html)
-   [Lot Numbered Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2235684.html)
-   [Drop Ship Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2239232.html)
-   [Special Order Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2242662.html)
-   [Gift Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2244991.html)
-   [Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2247990.html)
-   [Service Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248153.html)
-   [Download Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248348.html)
-   [Discount Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248474.html)
-   [Subtotal Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248793.html)
-   [Description Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248894.html)
-   [Markup Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2248975.html)
-   [Expense Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4042372470.html)
-   [Non-Inventory Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249092.html)
-   [Other Charge Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249208.html)
-   [Payment Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2249363.html)
-   [Item Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2222944.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
