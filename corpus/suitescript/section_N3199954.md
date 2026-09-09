---
id: "section_N3199954"
type: "section"
title: "Work Order Close"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Work Order Close"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199954.html"
anchors: ["bridgehead_1493058230", "bridgehead_1493058399", "bridgehead_N3200014", "bridgehead_3854693233"]
sha256: "35acf3f4569367bec63aa6491964dbc4229c222e61e36f8c729050507e44712a"
---

If the Manufacturing Work In Process (WIP) feature has been enabled, you can use SOAP web services to interact with work order close records. You can verify that WIP is enabled by going to _Setup > Company > Enable Features_, and reviewing the Items & Inventory subtab.

With WIP, instead of creating a single assembly build record to denote that a work order has been addressed, you track progress of the work using three records: work order issue, work order completion, and work order close. This approach lets you manage the assembly process in a more granular way, and to keep the General Ledger up to date as materials move through the different phases of assembly.

For details on the benefits of WIP, see [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html). For information about the process of closing a work order without WIP enabled, see [Marking Work Orders Closed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323037.html).

For help working with this record in the UI, see [Entering Work Order Closes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html).

The internal ID for this record is `workorderclose`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/workorderclose.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493058230}

The work order close record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1493058399}

The work order close record is partially scriptable. It can be updated, deleted, and searched using SuiteScript. It cannot be copied or created.

## Usage Notes {#bridgehead_N3200014}

To use this record you must have the following features enabled: Work Orders and Manufacturing Work in Process.

In the UI, this record is accessed by going to _Transactions > Manufacturing > Close Work Order_.

Note these additional details:

-   You must use [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) to create a new instance of this record. In this case, workorder is the originating record type. For more details, see [Prerequisites for Creating a Work Order Issue Record](#bridgehead_3854693233).
    
-   Assembly item should have scrap account, WIP account, and WIP Cost Variance Account specified.
    
-   [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html) and [record.copy(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258260.html) are not supported on this record.
    

## Prerequisites for Creating a Work Order Issue Record {#bridgehead_3854693233}

Before you can create a work order issue record, a work order record must already exist, and the work order must be configured to use WIP (the WIP box on the work order record must be selected). This is true regardless of whether you are creating the work order issue record using initialize and add, or add by itself. If you try to create a work order issue record referencing a work order that has not been configured to use WIP, the system generates an error reading in part, 'One of the following problems exists: You have an invalid work order < work order ID >, the work order does not use WIP, or the work order is already closed.' You can create and modify work orders by choosing _Transactions > Manufacturing > Enter Work Orders_.

You can also interact with work orders using SuiteScript, as described in [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199912.html).

Note also that the assembly item referenced in the work order must be properly set up for WIP, as described in the [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html).

### Related Topics

-   [Entering Work Order Closes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2340152.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
