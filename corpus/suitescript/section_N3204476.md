---
id: "section_N3204476"
type: "section"
title: "Promotion"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Marketing > Promotion"
parent: "chapter_N3204288"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3204476.html"
anchors: ["bridgehead_1492549126", "bridgehead_1492549135", "bridgehead_N3204517", "bridgehead_1520425583"]
sha256: "c868b124a06b7fce22f6016a7240ccf2fcb7b74e93356f4d496156d7755a694e"
---

Promotions allow you to create special offers to motivate your customers to purchase products in higher quantities. Promotions can help you to move out-of-date stock, increase sales, and reward valuable clients. Promotions provide discounts that customers can apply to Web store orders and orders placed with sales reps. Furthermore, NetSuite promotions enable you to target specific customers, locations or channels, and time periods.

For help working with this record in the UI, see [Promotions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4737596252.html), [Configuring Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4690874193.html), and [The Promotion Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4692026541.html).

The internal ID for this record is `promotioncode`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/promotioncode.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492549126}

The promotion record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492549135}

The promotion record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3204517}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| discounttype | radio | Valid values in scripts are:
-   percent
-   flat

 |

When applying a free gift promotion to a transaction using SuiteScript, the free gift is not automatically added or removed from the order.

The following SuiteScript example shows how to apply the free gift and remove it when the transaction is no longer eligible:

          `// Create Sales Order var mySalesOrder = record.create({     type: record.Type.SALES_ORDER,     isDynamic: true }); mySalesOrder.setValue({     fieldId: 'entity',     value: '41' });   // Add free gift promotion to the promotion machine mySalesOrder.selectNewLine({     sublistId: 'promotions' }); mySalesOrder.setCurrentSublistValue({     sublistId: 'promotions',     fieldId: 'promocode',     value: '103' }); mySalesOrder.commitLine({     sublistId: 'promotions' });  // Add eligible item with quantity 4 to the item machine mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'item',     value: '233' }); mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'quantity',     value: '4' }); mySalesOrder.commitLine({     sublistId: 'item' });  // *********** Manually add free gift and link it to the free gift promotion *********** mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'item',     value: '244' }); mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'quantity',     value: '2' }); mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'freegiftpromotion',     value: '103' }); mySalesOrder.commitLine({     sublistId: 'item' });  // Check Free Gift Promotion colums on Promotion Machine: // firstFreeGiftQuantity should say 2 // firstEligibleFreeGifts should say 2 // firstFreeGiftsAdded should say 2 var firstFreeGiftQuantity= mySalesOrder.getSublistValue({     sublistId: 'item',     fieldId: 'quantity',     line: 2 }); var firstEligibleFreeGifts = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'eligiblefreegifts',     line: 1 }); var firstFreeGiftsAdded = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'freegiftsadded',     line: 1 });   // *********** Reduce eligible item quantity to 3 *********** mySalesOrder.selectLine({     sublistId: 'item',     line: '1' }); mySalesOrder.setCurrentSublistValue({     sublistId: 'item',     fieldId: 'quantity',     value: '3' }); mySalesOrder.commitLine({     sublistId: 'item' });   // Verify that the columns have been updated but the user still needs to manually remove 1 Free Gift // secondFreeGiftQuantity should say 2 // secondEligibleFreeGifts should say 1 // secondFreeGiftsAdded should say 2 var secondFreeGiftQuantity= mySalesOrder.getSublistValue({     sublistId: 'item',     fieldId: 'quantity',     line: 2 }); var secondEligibleFreeGifts = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'eligiblefreegifts',     line: 1 }); var secondFreeGiftsAdded = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'freegiftsadded',     value: 1 });  // *********** Manually reduce Free Gift quantity *********** mySalesOrder.selectLine({     sublistId: 'item',     line: '2' }); mySalesOrder.setSublistValue({     sublistId: 'item',     fieldId: 'quantity',     value: '1' }); mySalesOrder.commitLine({     sublistId: 'item' });  // Verify that the promotions machine columns have been updated again // Verify that the columns have been updated but the user still needs to manually remove 1 Free Gift // firstFreeGiftQuantity should say 1 // firstEligibleFreeGifts should say 1 // firstFreeGiftsAdded should say 1 var thirdFreeGiftQuantity= mySalesOrder.getSublistValue({     sublistId: 'item',     fieldId: 'quantity',     line: 2 }); var thirdEligibleFreeGifts = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'eligiblefreegifts',     line: 1 }); var thirdFreeGiftsAdded = mySalesOrder.getSublistValue({     sublistId: 'promotions',     fieldId: 'freegiftsadded',     line: 1 });` 
        

## Working with the Discount Amount Search Column {#bridgehead_1520425583}

When you use the Discount Amount search column, instead of using the discountamount internal ID, use discountrate.

### Related Topics

-   [Promotions Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4737596252.html)
-   [Configuring Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4690874193.html)
-   [The Promotion Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4692026541.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Marketing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3204288.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
