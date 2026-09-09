---
id: "section_N3197386"
type: "section"
title: "Time"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Time"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3197386.html"
anchors: ["bridgehead_1493049222", "bridgehead_1493049231", "subsect_161226738170", "subsect_161226738171", "subsect_161850954731"]
sha256: "a70dfcc9d0e1375f08f3e79aa76db469f909658fb4c64b455c0cd66a980257bf"
---

A time transaction, also known as TimeBill, records the hours worked by an employee. This transaction can be used to record billable hours and invoice customers. This transaction is available when the Time Tracking feature is enabled.

For help working with this record in the UI, see [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html).

The internal ID for this record is `timebill`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/timebill.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Type {#bridgehead_1493049222}

The time record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1493049231}

The time record is fully scriptable, which means that the record can be created, updated, copied, deleted, and searched using SuiteScript.

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

## retract {#subsect_161226738170}

| **Corresponding UI Button** | Retract |
| --- | --- |
| **Action Description** | Retracts pending timebill with the specified ID. |
| **Returns** | {"id": recordId, "action": "retract", "success": \[true or false\], "recordCount": number of retracted timebills} |
| **Supported Script Types** | Client and server scripts For additional information, see [SuiteScript 2.1 Script Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4387172495.html). |
| **Since** | 2021.1 |

### Parameters {#subsect_161226738171}

See [action.execute(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509391388.html) for details about parameters required for the execution of any action. RecordId is a default input parameter for this action. No additional input parameters are necessary.

### Sample Return Objects {#subsect_161850954731}

The following sample shows how to use a retract action on timebill.

              `{  {  "id": recordId,  "action": "retract",  "success": [true or false],  "recordCount": number of retracted timebills  },  "notifications":[ Error, Warning, Information and text]  }` 
            

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
