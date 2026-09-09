---
id: "section_N3195884"
type: "section"
title: "Item Fulfillment"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Item Fulfillment"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3195884.html"
anchors: ["bridgehead_1492786208", "bridgehead_1492786256", "bridgehead_N3195928", "bridgehead_1534269204"]
sha256: "5bec9ddf268fa20c0d1deb98a498036d312d5795d77122bf7d978f78367d42b8"
---

An item fulfillment transaction records the shipment of some or all items on an order to the customer. The processes for item fulfillment transactions depend on whether the Advanced Shipping feature is enabled.

-   If Advanced Shipping is not enabled, the fulfillment and invoicing processes are combined. When an item fulfillment is created, a related invoice is created at the same time.
    
-   If Advanced Shipping is enabled, fulfillment and invoicing are two independent processes, and shipments can be recorded separately from billing.
    

For help working with this record in the UI, see [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html).

The internal ID for this record is `itemfulfillment. Copy` and `create` are not allowed for this record.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/itemfulfillment.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492786208}

The item fulfillment record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492786256}

The item fulfillment record is partially scriptable. It can be updated, deleted, and searched using SuiteScript. It cannot be created or copied.

## Usage Notes {#bridgehead_N3195928}

When working with this record, you can set _pick, pack_, or _ship_ as event trigger types that will execute your user event script. In the NetSuite Help Center, see [SuiteScript 2.1 User Event Script Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4387799721.html) for more information.

The Item Fulfillment/Item Receipt sublist is a **list** sublist.

The Shipping sublist is included on the item fulfillment record. This sublist is not currently showing on this record in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/index.html). To get the internal IDs for the Shipping sublist, open the Records Browser and go to one of the other record types that support this sublist. These records are sales order, cash sale, invoice, and estimate / quote.

The Shipping sublist's Shipping Tax Code field, internal ID shippingtaxcode, appears only if per-line taxes have been set on the Item sublist.

## Scripting with Item Fulfillment Return Addresses {#bridgehead_1534269204}

The internal ID for the return address subrecord is returnshippingaddress. The following table maps return address subrecord field IDs to prior return address field IDs.

| **Item Fulfillment Return Address Subrecord ID = returnshippingaddress** | **Deprecated Return Address Fields** |
| --- | --- |
| Field Label | Field ID | Field Label | Field ID |
| Country | country | Country | returnshipcountry |
| Attention | attention | \- |
| Addressee | addressee | \- |
| Phone | addrphone | \- |
| Address1 | addr1 | Address 1 | returnshipaddr1 |
| Address2 | addr2 | Address 2 | returnshipaddr2 |
| City | city | City | returnshipcity |
| State | state | State | returnshipstate |
| Zip | zip | Zip | returnshipzipcode |
| Address | addrtext | \- | returnaddress |
| Override | override | \- |

The following sample shows how to create an item fulfillment return address using the subrecord.

          `require(['N/record'], function(record) {      var salesOrder = record.transform({          fromType: record.Type.SALES_ORDER,          fromId: 1020,          toType: record.Type.ITEM_FULFILLMENT,          isDynamic: true,      });         var returnAddressSubrecord = salesOrder.getSubrecord({          fieldId: 'returnshippingaddress'      });         returnAddressSubrecord.setValue({          fieldId: 'country',          value: 'US'      });         returnAddressSubrecord.setValue({          fieldId: 'attention',          value: 'Amy Kall'      });         returnAddressSubrecord.setValue({          fieldId: 'addressee',          value: 'ABCCompany'      });         returnAddressSubrecord.setValue({          fieldId: 'addrphone',          value: '3256874555'      });         returnAddressSubrecord.setValue({          fieldId: 'addr1',          value: '955 Campus Dr Ste 101'      });         returnAddressSubrecord.setValue({          fieldId: 'city',          value: 'San Mateo'      });         returnAddressSubrecord.setValue({          fieldId: 'state',          value: 'CA'      });         returnAddressSubrecord.setValue({          fieldId: 'zip',          value: '94404'      });         var recordId = salesOrder.save();  });` 
        

### Related Topics

-   [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
