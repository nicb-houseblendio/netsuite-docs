---
id: "section_N3743940"
type: "section"
title: "Expense Category"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Expense Category"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3743940.html"
anchors: ["bridgehead_N3743958", "bridgehead_N3744138", "bridgehead_3845275009"]
sha256: "00513d818fa03c14a6e4c5606a5a2954a3898b08bb1b28097f5ffc0a2c3ad075"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Expense Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_82134258767.html).

Expense categories are used to group expenses. Popular categories include transportation, lodging, mileage, and entertainment. Each expense category is linked to an account. When employees enter an expense report, they select a category for each expense, and the expense automatically posts to the associated expense account. Note that new expense categories cannot be created at the time an expense report is entered.

For more information, see [Creating an Expense Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2415916.html).

The expense category record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3743958}

The following operations can be used with the expense category record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3744138}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [expense category](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/expensecategory.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_3845275009}

Before you begin working with expense categories, you need to understand the rateRequired field. The purpose of this field is to determine the behavior of expenses that use this category. That is, when rateRequired is set to true, an expense report line item using this category must have values in the Rate and Quantity fields. These values are then used to determine the amount of the expense. Note that you can also set default rates for your expense categories. You do this by using either the defaultRate body field (in accounts that are not OneWorld) or the Rates sublist (in OneWorld accounts).

Related to your ability to create defaults, be aware of the following: If your account is not a OneWorld account, the rateRequired value affects the availability of the defaultRate field. That is, when the value of rateRequired is true for any particular expense category, you can set a value for defaultRate for that category. Otherwise, the field is not available. The defaultRate field determines the default rate for the category throughout your organization.

If your account is a OneWorld account, you use the Rates sublist, which stores a default rate for the category for each subsidiary. Unlike the defaultRate body field, an expense category's Rates sublist is available even when you set the rateRequired value to false.

The default value of rateRequired is false.

### Related Topics

-   [Expense Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913978.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
