---
id: "section_N3200062"
type: "section"
title: "Work Order Completion"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Work Order Completion"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3200062.html"
anchors: ["bridgehead_1493058483", "bridgehead_1493058509", "bridgehead_N3200122", "bridgehead_3854691310"]
sha256: "10d42b774eba22310932f637097ab631bd3bc76e6df7278fbb2e0a4d28daabca"
---

If the Manufacturing Work In Process (WIP) feature has been enabled, you can use SOAP web services to interact with work order completion records. You can verify that WIP is enabled by going to _Setup > Company > Enable Features_, and reviewing the Items & Inventory subtab.

With WIP, instead of creating a single assembly build record to denote that a work order has been addressed, you track progress of the work using three records: work order issue, work order completion, and work order close. This approach lets you manage the assembly process in a more granular way, and to keep the General Ledger up to date as materials move through the different phases of assembly. For more on the benefits of WIP, refer to [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html).

The work order completion record is used to indicate that assemblies have been built. You can also optionally use this record to record that raw materials - items in the componentList sublist - have been consumed as part of the assembly process. This latter option is called entering a completion with backflush. For example, you might enter a completion with backflush if previous records (such as work order issue) did not record the consumption of all the materials you ended up using.

In the UI, you can view the form used for creating the work order completion record by choosing _Transactions > Manufacturing > Enter Completions_, selecting a Subsidiary (for OneWorld accounts), then clicking **Complete** that corresponds with one of the listed work orders. An alternate method is to view the work order and click one of two buttons: Enter Completions or Enter Completions With Backflush.

For help working with this record in the UI, see [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html).

The internal ID for this record is `workordercompletion`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/workordercompletion.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493058483}

The work order completion record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1493058509}

The work order completion record is partially scriptable. It can be updated, deleted, and searched using SuiteScript. It cannot be copied or created.

## Usage Notes {#bridgehead_N3200122}

To use this record you must have the following features enabled: Work Orders and Manufacturing Work in Process.

In the UI, this record is accessed by going to _Transactions > Manufacturing > Enter Completions_.

Note these additional details:

-   You must use [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) to create a new instance of this record. In this case, workorder is the originating record type. For more details, see [Prerequisites for Creating a Work Order Issue Record](#bridgehead_3854691310).
    
-   Assembly item should have scrap account and WIP account specified.
    
-   [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html) and [record.copy(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258260.html) are not supported on this record.
    
-   The Component sublist is available only when backflush = true
    

## Prerequisites for Creating a Work Order Issue Record {#bridgehead_3854691310}

Before you can create a work order issue record, a work order record must already exist, and the work order must be configured to use WIP (the WIP box on the work order record must be selected). This is true regardless of whether you are creating the work order issue record using initialize and add, or add by itself. If you try to create a work order issue record referencing a work order that has not been configured to use WIP, the system generates an error reading in part, 'One of the following problems exists: You have an invalid work order < work order ID >, the work order does not use WIP, or the work order is already closed.' You can create and modify work orders by choosing _Transactions > Manufacturing > Enter Work Orders_.

You can also interact with work orders using SuiteScript, as described in [Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199912.html).

Note also that the assembly item referenced in the work order must be properly set up for WIP, as described in the [Setting Up Items as WIP Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335987.html).

### Related Topics

-   [Entering Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2339352.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
