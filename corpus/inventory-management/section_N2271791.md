---
id: "section_N2271791"
type: "section"
title: "Advanced Bin / Numbered Inventory Management"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Basic Inventory Management > Bin Management > Advanced Bin / Numbered Inventory Management"
parent: "section_N2270284"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html"
anchors: ["bridgehead_0419115001", "procedure_N2271818", "bridgehead_N2271856", "bridgehead_4713947221", "bridgehead_4272937436", "procedure_N2271907"]
sha256: "79ab3e9cdd86cdda39fc53ea17e24bfab4aac18f96c0580187c3ded554f32683"
---

If you enable the Advanced Bin / Numbered Inventory Management feature, it provides an enhanced version of tracking inventory in bins. If you use the Lot Tracking and Serialized Inventory features, it includes bin tracking for serial and lot numbered items, respectively. For regular and numbered items, you can enable bin tracking on a per-location basis.

The Advanced Bin / Numbered Inventory Management feature includes functionality that is not available in the basic Bin Management feature. For more information, see [Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2270284.html).

## Advanced Bin Management Setup {#bridgehead_0419115001}

To set up advanced Bin Management, complete the procedures in the following topics:

Note:

If you use basic Bin Management and you want to upgrade to advanced Bin Management, see [Upgrading to Advanced Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html#subsect_0419103450).

1.  Enable the following features: **Bin Management** and **Advanced Bin/Numbered Inventory****Management** feature. See [Enabling Bin Management Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273046.html).
    
2.  Optionally, you can set bin preferences. See [Setting Bin Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2273755.html).
    
3.  If you use Multi-Location Inventory, set the Use Bins setting per location. See [Enabling Bin Management by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4713998969.html#subsect_156863697327).
    
4.  Add bins and assign each to a location that uses bins. See [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html).
    
5.  Enable the **Use Bins** setting for regular, lot, or serialized items that you track in bins. Optionally, you can also specify a preferred bin. See [Setting Up Item Records for Bins](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274433.html).
    
6.  If you have items, including lot or serial numbered types, with existing transactions or quantities, you can assign them to bins using the advanced Bin Put-Away Worksheet. See [Updating Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2277819.html).
    

For information about using SuiteScript with this feature, see [SuiteScript Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163726005075.html).

For information about using SOAP web services code with this feature, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html)

## No Pre-association Requirement {#procedure_N2271818}

Use bins on transactions without being required to pre-associate bins to items. This lets you put away items using the Bin Put-Away Worksheet, even if bins are not associated with those items.

-   The Bin Management feature requires you to associate a bin with the item on the item record. You must do this to select the bin for that item on transactions.
    
-   The Advanced Bin / Numbered Inventory Management feature lets you use any bin for any item. You do not have to identify the bin on the item's record. However, you can associate bins with any item on the item record. Then, those bins show in the Associated bins list on transactions. You can also set a preferred bin for an item.
    

## Use Bins for Serialized and Lot Numbered Items {#bridgehead_N2271856}

When you also use the Lot Tracking or Serialized Inventory features, you can assign bins to serial numbered items and lot numbered items. To set one these bins as your preferred bin, see [Lot, Serial, and Bin Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504285820.html).

If you use basic Bin Management, you cannot associate serial or lot items with bins.

## Use Bins on a Per-Location Basis {#bridgehead_4713947221}

When you also enable the Multi-Location Inventory feature, you can use bins at only specific locations. For example, you can set warehouse and store locations to use bins to track inventory. You can also choose to not use the Advanced Bin Management functionality at your head office location.

If you use basic Bin Management, you cannot use bins on a per-location basis.

For more information, see [Bin Management by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4713998969.html).

## Inventory Subtabs for Advanced Bin Management {#bridgehead_4272937436}

Depending on the item type, item records show the following subtabs on which you can track on hand and available quantities:

-   **Inventory Detail** - For items that use bins, this subtab shows the quantities for inventory numbers within each bin.
    
    Note:
    
    To display the inventory numbers on hand, you can select Inventory Numbers on Hand in the View field. Items that you do not put away are not included in the on-hand count at the bin level.
    
-   **Bin Numbers** - Shows the quantities for each bin
    
-   **Inventory Numbers** - Shows the quantities for each inventory number within a location
    

## Inventory Detail Subrecord {#procedure_N2271907}

Note:

The inventory detail subrecord on item records display on-hand and available quantities in five decimal places, whereas it displays those on transactions in eight decimal places. If you want to get these quantities with eight decimal places from the inventory detail subrecord through scripting, saved search, or formula, use the [Inventory Balance Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518564230.html). Otherwise, you might get a mismatch between the quantity values.

On the **Inventory Detail** subtab of item records, you can view quantities for bins, lot numbers, serial numbers, and inventory statuses. On transactions or records, you can click the **Inventory Detail** icon to filter the bins list, choose a bin, and enter a quantity. For items that use and don't use bins, you can also specify the inventory statuses, lot number, or serial number depending on the features you use. For more information, see [Entering Inventory Details on Transactions or Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0326021504.html).

Permissions for the inventory detail subrecord are inherited from its parent transaction. For example, to edit the inventory detail from a sales order, you must have permission to edit the sales order. For more information, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

### Related Topics

-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Printing Bin Putaway Worksheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2275156.html)
-   [Bin Transfers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2278346.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
