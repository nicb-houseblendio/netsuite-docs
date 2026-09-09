---
id: "section_N3202484"
type: "section"
title: "Expense Category"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Lists > Expense Category"
parent: "chapter_N3200673"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3202484.html"
anchors: ["bridgehead_1492454232", "bridgehead_1492454243"]
sha256: "ddfe627c4182e37afcb92b95c3d17c965d621b58459ce9d65f556eef764fc911"
---

Expense categories are used to group expenses. Popular categories include transportation, lodging, mileage, and entertainment. Each expense category is linked to an account. When an employee enters an expense report, they select a category for each expense, and the expense automatically posts to the associated expense account. Note that new expense categories cannot be created at the time an expense report is entered.

If you use NetSuite OneWorld, be aware that an expense category is available to only those subsidiaries assigned to the account linked with the expense category. If you want to enable intercompany expense transactions, you should set up expense categories linked to expense accounts that are available to all subsidiaries, for use in these transactions. For intercompany expense transactions, users cannot save expense lines unless they contain expense categories available to both the employee subsidiary and customer subsidiary.

To enter expense categories, go to _Setup > Accounting > Expense Categories > New_.

For help working with this record in the UI, see [Creating an Expense Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415916.html).

The internal ID for this record is `expensecategory`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/expensecategory.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492454232}

The expense category record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492454243}

The expense category record is fully scriptable - it can be created, updated, copied, deleted, and searched using SuiteScript.

### Related Topics

-   [Creating an Expense Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415916.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3200673.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
