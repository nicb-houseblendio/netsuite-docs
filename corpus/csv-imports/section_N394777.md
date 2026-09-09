---
id: "section_N394777"
type: "section"
title: "Bin Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Bin Import"
parent: "section_N394620"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394777.html"
anchors: []
sha256: "02f21d3ce2f2e4358a2fb21d05122140f4cfd8b64130e0c764ae37bea9af4466"
---

Bin records define bin locations within a warehouse or stock room. Bin record numbers are associated with items and included on receiving and fulfilling transactions to keep track of the on-hand quantity for each bin.

For details about bins in NetSuite, see [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html).

Note:

Bin imports aren't available unless the Bin Management feature is enabled in your account. To enable this feature, go to _Setup > Company > Enable Features_ and on the Items & Inventory subtab, check Bin Management.

Note the following:

-   A Bin Number field value is required to uniquely identify each Bin record.
    
-   If the Multi-Location Inventory (MLI) feature is enabled, the Location field is required. Note that if you use bins with MLI, you must use bins in all locations. After a bin record has been saved for the first time, the location value can't be changed.
    
-   If the Warehouse Management feature is enabled, you can import data for the following fields: Type, Sequence Number, and Zone. For more information about working with these fields, see [Creating Bin Locations or Carts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161314312081.html#section_1541433492).
    
-   After bin records have been created, you can associate them with inventory item records. To associate bins with an item record, you need to set the item's Use Bins field value to True, and add bin records to the item's Bin Numbers sublist. You can set the Preferred field value to True for one item bin record per location. You can complete these tasks on the Item page in the user interface, or through an Items import.
    

For details about fields that can be mapped in the bin record, see the SOAP Schema Browser's [bin](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/bin.html). You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with this tool, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Creating Bin Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2274082.html)
-   [Basic Bin Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271509.html)
-   [Advanced Bin / Numbered Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2271791.html)
-   [Items Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html)
-   [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html)
-   [Supply Chain Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394620.html)
-   [Item Revision Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395019.html)
-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)
-   [Warehouse Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_156356229851.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
