---
id: "section_N3186192"
type: "section"
title: "Lead"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Lead"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3186192.html"
anchors: ["bridgehead_1492032931", "bridgehead_1492033037", "bridgehead_N3186234", "bridgehead_N3186932"]
sha256: "fb6f3be0b53e3ea6eb2340ddd7d9b63667760508ccbf55ab5c51448862f08d27"
---

Leads are companies or individuals who represent potential customers. In NetSuite, leads are the first step in the sales cycle that progresses to prospect and then to customer.

For help working with this record in the user interface, see [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html).

The internal ID for this record is `lead`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/lead.html) for all internal IDs associated with this record.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492032931}

The lead record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492033037}

The lead record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3186234}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| datecreated | Date Created | This is a system-generated field that marks the date the record was created in NetSuite. You cannot change or override this field. Tip: If you need to capture 'date created' information that is not related to the date the record was created in NetSuite, create a custom field and set it to auto-default to today's date. |
| password | Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| password2 | Confirm Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| **Search Filters and Search Columns** |
| ccnumber | Credit Card Number | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

The Access / contactroles sublist is included in the customer record on the Access subtab. It is an inline editor subtab. The Access / contract roles sublist is related to the Contact / contactroles sublist. For details, see the contactroles sublist in the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/lead.html).

The Time Tracking sublist is included with the lead record. It is an inline editor sublist.

Important:

If any case, task, or event record has more than 9500 time entries in the Time Tracking sublist, all cases include a static list of time entries. These static lists are not accessible to scripting. Attempts to script on Time Tracking sublists that are static lists of time entries will not return accurate results.

## Transform Types {#bridgehead_N3186932}

In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

| Target Record Name | Target Record Internal ID | Field Defaults |
| --- | --- | --- |
| Opportunity | opportunity | \- |

### Related Topics

-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)
-   [Creating a Lead Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1095784.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
