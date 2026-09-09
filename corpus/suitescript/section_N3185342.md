---
id: "section_N3185342"
type: "section"
title: "Employee"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Entities > Employee"
parent: "chapter_N3184398"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3185342.html"
anchors: ["bridgehead_1492030420", "bridgehead_1492030471", "subsect_0302024710", "bridgehead_N3185384", "bridgehead_1503508422", "bridgehead_N3185556"]
sha256: "684f8002d5316ef3f7eca0158eeb7e4a3e8a33421cffb903fbbcacf938e73eb2"
---

For help working with this record in the user interface, see [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html).

The internal ID for this record is `employee`.

This record contains the following sublist: subscriptions.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/employee.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492030420}

The employee record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492030471}

The employee record supports the following functions: create, read, update, and delete. The following functions aren't supported: copy, search, and transform.

## Prerequisites {#subsect_0302024710}

To use the subscriptions sublist of this record with SuiteScript, you must enable the Marketing Automation and Subscription Categories features. For more information, see [Marketing Automation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N973384.html).

## Usage Notes {#bridgehead_N3185384}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| password | Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| password2 | Confirm Password | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |

## Scripting when Advanced Employee Permissions is Enabled {#bridgehead_1503508422}

When the Advanced Employee Permissions feature is enabled keep the following in mind:

-   Before submit scripts can be run, either as the role that has manipulated the record or as an administrator, the script only has access to the information that has been submitted from the browser. In the case of an employee record being edited, the before submit script only has access to the fields or sublists the role editing the record is permitted to edit. Therefore, you cannot assume that all fields and sublists on the employee record are available in a before submit script.
    
-   After submit scripts can be run as administrator, which means complete access to an employee record. When the Advanced Employee Permissions feature is enabled, perform actions, such as setting the value of a field, as a role that is known to have the appropriate level of access or as an administrator.
    

For information about this feature, see [Advanced Employee Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1494536002.html).

## Transform Types {#bridgehead_N3185556}

In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

| Target Record Type | Target Record Internal ID | Field Defaults |
| --- | --- | --- |
| Expense Report | expensereport | \- |
| Time | timebill | \- |

### Related Topics

-   [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html)
-   [Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3184398.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
