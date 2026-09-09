---
id: "section_N3757717"
type: "section"
title: "Budget Category"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Other Lists > Budget Category"
parent: "chapter_N3757146"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3757717.html"
anchors: ["bridgehead_N3757754", "bridgehead_N3757918", "bridgehead_N3757956", "procedure_N3757970"]
sha256: "869a0917c85f553960d855c154b5f2c5620490b993f10b81b5ac2ce21d4e80d6"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Budget Category](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0522035327.html).

Budget categories are used with the **Multiple Budgets** feature to create budgets for a variety of scenarios. Be aware that budget categories are available only if you have the Multiple Budgets feature enabled in your account. See [Usage Notes](#bridgehead_N3757956) for steps on enabling this feature.

The budget category record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3757754}

The following operations can be used with the budget category record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getAll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3489077.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3757918}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the [budget category](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/budgetcategory.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3757956}

To use the budget category record, a NetSuite administrator must first enable the Multiple Budgets feature in your account.

#### To enable Multiple Budgets: {#procedure_N3757970}

1.  Go to _Setup > Company > Setup Tasks > Enable Features_.
    
2.  Click the Accounting subtab.
    
3.  Check the Multiple Budgets box in the Advanced Features grouping.
    
4.  Click Save.
    

After this feature is enabled, any user can create budget categories in the UI. For steps on creating budget categories, see [Creating Budget Categories for Local Subsidiary Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1506823.html) in the NetSuite Help Center.

### Related Topics

-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
