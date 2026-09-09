---
id: "section_N3184172"
type: "section"
title: "Event"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Activities > Event"
parent: "chapter_N3184006"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184172.html"
anchors: ["bridgehead_1516396108", "bridgehead_1516396165", "bridgehead_1502829239"]
sha256: "89515022d7867229a051175f4abe78a43fb1360bd196add9b393f232fb8de778"
---

Events are scheduled activities that are automatically added to your calendar when created.

For help working with this record in the user interface, see [Creating a New Event Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501988.html).

The internal ID for this record is `calendarevent`. Note that setting recurring events in SuiteScript is not currently supported.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/calendarevent.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1516396108}

The event record is scriptable in both server and client SuiteScript.

## Supported Functions {#bridgehead_1516396165}

The event record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_1502829239}

When the Time Tracking feature is enabled, the TimeItemList sublist is available. This list is used to track employee time associated with the phone call, including payroll, billing, and project fields. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

### Related Topics

-   [Creating a New Event Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N501988.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
