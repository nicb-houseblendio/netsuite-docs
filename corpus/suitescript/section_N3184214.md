---
id: "section_N3184214"
type: "section"
title: "Phone Call"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Activities > Phone Call"
parent: "chapter_N3184006"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3184214.html"
anchors: ["bridgehead_1516396243", "bridgehead_1516396283", "bridgehead_1502829370"]
sha256: "252eb4ddf98eabea5676a13e7f870a699df5513f975e461daabcf2b0bb47ee55"
---

Phone calls records are used to document phone call activity. All information submitted for a phone call record is stored on a record in the phone call list, on the customer record who calls and on any contact's records referenced in the call contact list.

For help working with this record in the user interface, see [Working with Phone Calls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509876.html).

The internal ID for this record is `phonecall`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/phonecall.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1516396243}

The phone call record is scriptable in both server and client SuiteScript.

## Supported Functions {#bridgehead_1516396283}

The phone call record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_1502829370}

When the Time Tracking feature is enabled, the TimeItemList sublist is available. This list is used to track employee time associated with the phone call, including payroll, billing, and project fields. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

### Related Topics

-   [Working with Phone Calls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N509876.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3650400.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
