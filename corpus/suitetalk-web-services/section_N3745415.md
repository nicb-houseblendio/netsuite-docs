---
id: "section_N3745415"
type: "section"
title: "Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Subrecords > Inventory Detail > Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled"
parent: "section_N3744760"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html"
anchors: ["bridgehead_N3745490", "bridgehead_N3745782", "bridgehead_N3745795", "bridgehead_N3745907"]
sha256: "41a46f7932ce74207a7be0d60e25c6f4c0f5a5fd2ac38f50b1b2e9269484d152"
---

The SOAP web services code used to access bin number and serial/lot number data for items, including transaction line items, varies according to whether the Advanced Bin / Numbered Inventory Management feature is enabled. If this feature is not enabled, this data is available directly from the item. If this feature is enabled, this data must be accessed through the inventory detail subrecord, which was introduced in the 2011.2 endpoint.

If this feature is enabled in your account, you need to do the following to avoid unexpected results or errors in your SOAP web services code.

1.  Update to the 2011.2 endpoint or later to have access to the inventory detail subrecord and its bin and numbered inventory fields.
    
2.  Review the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord to get an understanding of how it is structured in the schema.
    
3.  Review the list of [Records that May Include Inventory Detail Data](#bridgehead_N3745782).
    
4.  Review any existing code for these records that accesses bin or numbered inventory fields, and update this code to use the inventory detail subrecord. See [Sample Code Changes after Enabling Advanced Bin / Numbered Inventory Management](#bridgehead_N3745490).
    

## Sample Code Changes after Enabling Advanced Bin / Numbered Inventory Management {#bridgehead_N3745490}

The following code samples illustrate the difference between:

-   Setting a serial number value for an item in an inventory adjustment transaction without Advanced Bin / Numbered Inventory Management, and
    
-   Setting inventory detail data, including the serial number, with the Advanced Bin / Numbered Inventory Management feature enabled.
    

When the feature is enabled, code like the bolded, red text on the left must change to code like the bolded, red text on the right.

| 
WITHOUT Advanced Bin/Numbered

Inventory Management



 | 

With Advanced Bin/Numbered

Inventory Management ENABLED



 |
| --- | --- |
| InventoryAdjustment ia = new InventoryAdjustment(); ia.setSubsidiary(new RecordRef(null,"1",null,null)); ia.setAccount(new RecordRef(null,"1",null,null)); InventoryAdjustmentInventory item = new InventoryAdjustmentInventory(); item.setItem(new RecordRef(null, i.getInternalId(), null, null)); item.setLocation(new RecordRef(null,"1",null,null)); item.setAdjustQtyBy(new Double(2)); item.setSerialNumbers("Grape16324299(2)"); ia.setInventoryList(new InventoryAdjustmentInventoryList(new InventoryAdjustmentInventory\[\] {item},true)); sessMgr.getPort().add(ia); | InventoryAdjustment ia = new InventoryAdjustment(); ia.setSubsidiary(new RecordRef(null,"1",null,null)); ia.setAccount(new RecordRef(null,"1",null,null)); InventoryAdjustmentInventory item = new InventoryAdjustmentInventory(); item.setItem(new RecordRef(null, i.getInternalId(), null, null)); item.setLocation(new RecordRef(null,"1",null,null)); item.setAdjustQtyBy(new Double(2)); InventoryAssignment assign = new InventoryAssignment(); assign.setReceiptInventoryNumber("Grape19816143,Melon12289447"); assign.setQuantity(new Double(2)); InventoryDetail id = new InventoryDetail(); id.setInventoryAssignmentList(new InventoryAssignmentList(new InventoryAssignment\[\] {assign},true)); item.setInventoryDetail(id); ia.setInventoryList(new InventoryAdjustmentInventoryList(new InventoryAdjustmentInventory\[\] {item},true)); sessMgr.getPort().add(ia); |

## Records that May Include Inventory Detail Data {#bridgehead_N3745782}

Review the following lists to understand which code you may need to modify after enabling the Advanced Bin / Numbered Inventory Management feature.

## Items Affected by Advanced Bin/Numbered Inventory Management {#bridgehead_N3745795}

The following types of items include inventory detail data when the Advanced Bin / Numbered Inventory Management feature is enabled:

-   [Assembly Item (BOM Item)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713949.html) (when Use Bins is set to True)
    
-   [Lot Numbered Assembly Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3719877.html)
    
-   [Serialized Assembly Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3727646.html)
    
-   [Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3717575.html) (when Use Bins is set to True)
    
-   [Lot Numbered Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3720360.html)
    
-   [Serialized Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3728128.html)
    

## Transactions Affected by Advanced Bin / Numbered Inventory Management {#bridgehead_N3745907}

The following types of transactions include inventory detail data for each line item when the Advanced Bin / Numbered Inventory Management feature is enabled:

-   [Assembly Build](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659969.html)
    
-   [Assembly Unbuild](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3660532.html)
    
-   [Bin Putaway Worksheet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3661129.html)
    
-   [Bin Transfer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3661654.html)
    
-   [Cash Refund](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3662733.html)
    
-   [Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3663345.html)
    
-   [Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3664209.html)
    
-   [Credit Memo](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3666537.html)
    
-   [Estimate/Quote](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3673214.html)
    
-   [Inventory Adjustment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3676432.html)
    
-   [Inventory Transfer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3678082.html)
    
-   [Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3678746.html)
    
-   [Item Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3680777.html)
    
-   [Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3681685.html)
    
-   [Purchase Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3687718.html)
    
-   [Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3688557.html)
    
-   [Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3690924.html)
    
-   [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html)
    
-   [Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3694535.html)
    
-   [Vendor Credit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3695165.html)
    
-   [Vendor Return Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3696445.html)
    
-   [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3697954.html)
    

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3432503.html)
-   [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
