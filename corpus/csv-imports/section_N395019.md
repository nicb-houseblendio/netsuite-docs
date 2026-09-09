---
id: "section_N395019"
type: "section"
title: "Item Revision Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Item Revision Import"
parent: "section_N394620"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395019.html"
anchors: []
sha256: "0a9bf91916fb64e436256e450e44f49d2e3dfd7894bc55a76d8bc553bb5af5db"
---

When the Assembly Items feature is enabled, you can use this import to add and update item revision records that define which member items should be included in assembly builds during specific time frames.

The exact member components needed for assembly items are identified in the Bill of Materials (BOM), but required components may change over time. These changing requirements can be documented in item revision records, which are part of BOM member control functionality. An item revision record sets an effective date for a member item to be included in assembly builds. Each item revision record can be assigned to multiple assembly items, because one item can be a member of different assembly items. For more details, see [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html).

The Item Revision import supports the following fields:

-   Effective Date (required) - the date when a member item should begin to be included in assembly items to which this revision record is assigned
    
-   ExternalId - can be used as a unique identifier for each item revision record
    
-   Inactive - indicating whether the item revision record is inactive
    
-   Item (required) - the member item to which this item revision record applies
    
-   Memo - optional descriptive text
    
-   Name (required) - name of the item revision record
    

This import can't add or update values for the Obsolete Date field. When an imported revision record is saved, the system determines its obsolete date, based on its effective date and on the effective dates of other revision records for the member item, to avoid gaps or overlaps in dates covered by revisions.

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Supply Chain Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394620.html)
-   [Bin Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N394777.html)
-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Manufacturing Routing Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399906.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
