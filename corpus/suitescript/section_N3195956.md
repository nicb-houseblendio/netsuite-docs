---
id: "section_N3195956"
type: "section"
title: "Item Receipt"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Item Receipt"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3195956.html"
anchors: ["bridgehead_1492786679", "bridgehead_1492786715", "bridgehead_N3195998", "bridgehead_N3196010", "bridgehead_N3196030"]
sha256: "c213e3e1e5de924ee11e34b2fa23baa35f88d26aea895826c6b9e11ddb4838c1"
---

An item receipt transaction records the receipt of returned items from customers. This transaction updates the following information:

-   Items on return authorizations are recorded as received.
    
-   Inventory records are updated for the new stock levels.
    
-   Inventory asset accounts are updated with the values of returned items.
    
-   Status of the return is updated.
    

The item receipt transaction is available when the Advanced Receiving feature is enabled.

For help working with this record in the UI, see [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html) and [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html).

The internal ID of this record is `itemreceipt`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/itemreceipt.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492786679}

The item receipt record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492786715}

The item receipt record is partially scriptable. It can be updated, deleted, and searched using SuiteScript. It cannot be created or copied.

## Usage Notes {#bridgehead_N3195998}

The Item Fulfillment/Item Receipt sublist is a **list** sublist.

## Using Landed Cost Fields {#bridgehead_N3196010}

When you create a landed cost category, the associated field IDs for the first category are landedcostamount1 and landedcostsource1. If you create a second category, the IDs will be landedcostamount2 and landedcostsource2.

This pattern increments by one with each additional category. For example, the IDs for the next landed cost category will be landedcostamount3 and landedcostsource3, and so on.

## Creating Item Receipt Records {#bridgehead_N3196030}

You cannot create standalone item receipts using SuiteScript. For example, the following will throw an error:

          `var itemReceipt = record.create({      type: record.Type.ITEM_RECEIPT  })` 
        

To create an item receipt, you must use [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html), which transforms the data from one record type, purchase order, for example, into an item receipt. To create an item receipt, your code would be similar to the following:

          `// Transform a record with a specific id to a different record type.   // For example, from PO to Item Receipt  // Get the object of the transformed record.        var trecord = record.transform({          fromType: record.Type.PURCHASE_ORDER,          fromId: 26,          toType: record.Type.ITEM_RECEIPT      });        qty = trecord.getSublistValue({          sublistId: 'item',          fieldId: 'quantity',          line: 1      });      trecord.setSublistValue({          sublistId: 'item',          fieldId: 'quantity',          line: 1,          value: '2'      });        var idl = trecord.save ({          enableSourceing: true      });        email.send({          author: -5,          recipient: -5,          subject: 'Transform Email',          body: 'Original Qty = '  });` 
        

### Related Topics

-   [Receiving a Customer Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1307628.html)
-   [Handling Returned Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1308274.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
