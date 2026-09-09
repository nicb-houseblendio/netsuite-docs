---
id: "section_N3713653"
type: "section"
title: "Item Search"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Searches > Item Search"
parent: "chapter_4177763939"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3713653.html"
anchors: []
sha256: "221fcf61308b01ff20d69000dd8106a0c393f99dc3aabd43d371ecd1af69ba7b"
---

Most item record types use the ItemSearch complex type for search. The **basic** element in ItemSearch references ItemSearchBasic, which lists all of the filter fields available when searching items.

The ItemSearch record also lists all search joins available in an item search. For details, see the SOAP Schema Browser's [ItemSearch](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/search/itemsearch.html?mode=package) reference page. The ItemSearch complex type is defined in the [lists accounting XSD](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd).

Be aware that the search filter fields available vary depending on the item type you are searching. For example, not all of the search filter fields defined in ItemSearchBasic exist on the Subtotal Item record.

Important:

By default, only a record's body fields are returned on a search. If you want to return the information specified on a record's sublist, you must set the **bodyFieldsOnly** element of the SearchPreferences type to **false**. For general information on searching in SOAP web services, see [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html).

For more details on this search type, see the following topics:

-   [Item Search Usage Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4349721305.html)
    
-   [Item Search Code Sample](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4349720855.html)
    

### Related Topics

-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3704574.html)
-   [Usage Notes for Item Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705128.html)
-   [Working with Matrix Items in SOAP web services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3705423.html)
-   [Shared Field Definitions for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3707811.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
