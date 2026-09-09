---
id: "section_N3190839"
type: "section"
title: "Reallocate Items"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Items > Reallocate Items"
parent: "chapter_N3188218"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3190839.html"
anchors: ["bridgehead_1493323571", "bridgehead_1493323625"]
sha256: "9fae358a88eb2dcc96cbab852ff864eb5bc4938e7d7353f744241f0cfadd0eb5"
---

NetSuite sometimes automatically allocates items from inventory to commit them to fill orders. Inventory may be automatically committed in the following cases:

-   As each sales order is created or approved, your account automatically allocates inventory from the item's quantity available.
    
-   Inventory is automatically committed to fill backorders when goods are received from your vendors.
    
-   The inventory generated from assembly work orders is automatically allocated.
    

For help working with this record in the UI, see [Reallocating Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263567.html).

The internal ID for this record is `reallocateitem`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/reallocateitem.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493323571}

The reallocate items record is only exposed in user event scripts. You can run `beforeLoad`, `beforeSubmit`, and `afterSubmit` user event scripts on this record.

## Supported Functions {#bridgehead_1493323625}

The reallocate items record can only be copied and searched. It cannot be created, updated, or deleted using scripts.

### Related Topics

-   [Reallocating Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2263567.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3188218.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
