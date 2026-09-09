---
id: "section_N3732831"
type: "section"
title: "Issue"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Support > Issue"
parent: "chapter_N3732579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3732831.html"
anchors: ["bridgehead_N3732867", "bridgehead_N3733124", "bridgehead_3984274606"]
sha256: "e31ddaa0f077a922f26d4b2d61a6652e145630191b0d307f89298e04bbc8f961"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Issue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_4093608295.html).

The issue record is defined in the [listSupport (support)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/support.xsd) XSD.

For details about using issue records in the user interface, see [Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2438260.html).

## Supported Operations {#bridgehead_N3732867}

The following operations can be used with Issue records.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3733124}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [issue](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/issue.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_3984274606}

Be aware that the behavior of the issue record varies depending on the value of the Use Multiple Versions and Builds preference, which you set at _Setup > Issues > Issue Preferences_. When you select the **Use Multiple Versions and Builds** box, the issue record uses three sublists: customFieldList, fixedInVersionList, and relatedIssuesList. When you do not set this preference, the record uses the following six body fields:

-   versionBroken
    
-   buildBroken
    
-   versionTarget
    
-   buildTarget
    
-   versionFixed
    
-   buildFixed
    

Note that these body fields are exposed in the 2014.1 and later WSDLs, but not in previous WSDLs.

### Related Topics

-   [Support](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3732579.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
