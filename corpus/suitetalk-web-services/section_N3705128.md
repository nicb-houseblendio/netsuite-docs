---
id: "section_N3705128"
type: "section"
title: "Usage Notes for Item Record Types"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Items > Usage Notes for Item Record Types"
parent: "chapter_N3704574"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html"
anchors: ["bridgehead_N3705215"]
sha256: "3f61eb0c270c2d51677ca840c12a91d9637847e7e3a8523aff6fcd19611bdb22"
---

Note the following when working with item record types:

-   Items are the goods and services you sell to customers, and the parts and raw materials you purchase from vendors. They can also include line items on sales and purchase forms, such as discounts and miscellaneous charges.
    
-   Depending on the features enabled for the account specified during the login call, some item types may not be available.
    
-   Setting the item base price will auto-calculate other pricing levels. For more information about setting item prices, see [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html) in the NetSuite Help Center.
    
-   To make an item featured, you must set the item category to the Home tab in the NetSuite UI.
    
-   The countryofmanufacture field for an item must be a country covered by FedEx or UPS.
    
-   All item records are defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.
    

## Working with Costing Methods {#bridgehead_N3705215}

As of the 2013.1 endpoint, the costingMethod field was added to [Lot Numbered Assembly Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3719877.html), [Lot Numbered Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3720360.html), [Serialized Assembly Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3727646.html), and [Serialized Inventory Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3728128.html). This field is not required for the add operation. Its value defaults to lot numbered for lot numbered items, and to specific for serialized items.

This field becomes read-only after it is set, so it is only used for add and advanced search operations. Note that this field is not returned in get and basic search operations. Instead, the read-only field costingMethodDisplay is returned. When this field is used as a Results column in advanced search operations, it returns different values for the 2013.1 endpoint than in earlier endpoints. Before, the return value for lot numbered items was fifo, and the returned value for assembly items was lifo. Now the return value for lot numbered items is lot numbered and the return value for serialized items is specific.

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [Item Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
