---
id: "section_N3187339"
type: "section"
title: "Prospect"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Prospect"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3187339.html"
anchors: ["bridgehead_1492182944", "bridgehead_1492182984", "bridgehead_N3187381", "bridgehead_N3187613"]
sha256: "711eca57ef1f2c419f297a3084e4a4783613cceb5ff5f33c64eff5f211297404"
---

Prospect records enable you to track all the information you need to convert a prospect into a customer.

The internal ID for this record is `prospect`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/prospect.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492182944}

The prospect record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492182984}

The prospect record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3187381}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| password | Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| password2 | Confirm Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| **Search Filters and Search Columns** |
| ccnumber | Credit Card Number | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

The Access / contactroles sublist is included in the customer record on the Access subtab. It is an inline editor subtab. The Access / contract roles sublist is related to the Contact / contactroles sublist. For details, see the contactroles sublist in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/prospect.html).

The Time Tracking sublist is included with the prospect record. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

## Transform Types {#bridgehead_N3187613}

In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

| Target Record Name | Target Record Internal ID | Field Defaults |
| --- | --- | --- |
| Estimate/Quote | estimate | \- |
| Opportunity | opportunity | \- |
| Sales Order | salesorder | \- |

### Related Topics

-   [Record Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1074872.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
