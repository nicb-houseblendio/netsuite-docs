---
id: "section_N3662262"
type: "section"
title: "Budget"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Budget"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3662262.html"
anchors: ["bridgehead_N3662302", "bridgehead_N3662530", "bridgehead_4769787129", "bridgehead_4771620826", "bridgehead_1493970965"]
sha256: "8f86e39d76b3e9e274d6ad5ef3c959b5d251867af254cf698c96562d980524a3"
---

A budget records the expected values of income and expenses for your business. You can create budgets for specific customers, items, departments, classes, locations, or any combination of these criteria. You can also create budgets for multiple subsidiaries in NetSuite OneWorld. For general information about budgets, see [Setting Up a Budget](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1503407.html).

In SOAP web services, the budget record is defined in the [tranFin (financial)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/financial.xsd) XSD. Note that before updating a row on this record, you must perform a **get** on the entire record.

## Supported Operations {#bridgehead_N3662302}

The following operations can be used with the budget record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3662530}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [budget](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/budget.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_4769787129}

## Custom Segments for the Budget Record {#bridgehead_4771620826}

You cannot use CustomFieldList to create custom fields on the budget record, but you can set a custom segment value for a budget record by setting its CustomFieldList property. You cannot create a custom segment, but you can use SOAP web services to add, delete, and update segment values.

You can use CustomJoin for BudgetSearch and BudgetSearchRow, which are both defined in the [common](https://webservices.netsuite.com/xsd/platform/v2025_2_0/common.xsd) XSD.

For details, see [Working With Custom Segment Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4514768175.html), [CustomFieldLists for Setting Custom Segment Values](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4514127747.html), and [CustomFieldList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3438152.html).

## Supported Accounting Periods in the Budget Record {#bridgehead_1493970965}

The budget record supports more than 12 accounting periods for add, get, and search operations. If your accounting setup consists of more than 12 accounting periods, you can add, retrieve, and search for up to 24 accounting periods. For more information about accounting periods, see [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html).

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
