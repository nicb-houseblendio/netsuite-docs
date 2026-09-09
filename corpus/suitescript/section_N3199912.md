---
id: "section_N3199912"
type: "section"
title: "Work Order"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Work Order"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199912.html"
anchors: ["bridgehead_1493057685", "bridgehead_1493057733", "bridgehead_1501526895", "bridgehead_1502143908"]
sha256: "8c94040ddac51134b87cdb4b0a7489f9753c583fc6ea210b08735432bc9e5bb6"
---

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/workorder.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

Work order transactions track the production of assembly items needed for stock or to fill orders. Work orders track the quantities of assemblies that need to be built and the quantities of components, or member items, needed to do so. This type of transaction is available when the Assembly Items and Work Orders features are enabled and is used when the Allow Purchase of Assembly Items accounting preference is not enabled.

Special order work orders track assemblies for a particular sale, and Production work orders track assemblies to increase stock. Both use the same work order form, but Production work orders do not link to a sales transaction. Production work orders are generated when the back ordered quantity of an assembly reaches its assigned build point. After the build point is reached, a work order is added in the Mass Create Work Orders queue.

For help working with this record in the UI, see [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html).

The internal ID for this record is `workorder`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/workorder.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493057685}

The work order record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1493057733}

The work order record is fully scriptable, which means that the record can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_1501526895}

## Fields {#bridgehead_1502143908}

| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| --- | --- | --- |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

### Related Topics

-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
