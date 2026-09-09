---
id: "section_N3754626"
type: "section"
title: "Subsidiary"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Subsidiary"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3754626.html"
anchors: ["bridgehead_N3754643", "bridgehead_N3754870", "bridgehead_3993897086"]
sha256: "dccd9f72f6017c66976794ae3dea1996ae292ce66dc0d1221888ab1653a50337"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157607424766.html).

A NetSuite OneWorld account enables you to manage data for a hierarchical structure of separate legal entities, or subsidiaries. This structure is organized as a tree that rolls up to a root, or top-level parent subsidiary. The root subsidiary is the highest-level subsidiary in your account, and all other subsidiaries are below it in the hierarchy. If an account that is upgraded to OneWorld has preexisting data, this data is used for the root subsidiary.

Each subsidiary represents a separate company within your global organization. Subsidiaries can be international or domestic. When you create a subsidiary record in NetSuite, the country you define for its address determines the NetSuite edition and tax nexus associated with that subsidiary.

For more details, see [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html) and [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html).

The subsidiary record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3754643}

The following operations can be used with the subsidiary record.

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3754870}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [subsidiary](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/subsidiary.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Note for Accounts Using the 2013.2 and Earlier WSDLs {#bridgehead_3993897086}

If you are using the 2013.2 endpoint or earlier, be aware that the subsidiary field, as defined in your WSDL, includes some body fields that are no longer used by NetSuite. Therefore, even if you are using an older WSDL that lists these fields, you can no longer interact with them. The fields are:

-   anonymousCustomerInboundEmail
    
-   anonymousCustomerOnlineForms
    
-   caseAssignmentTemplate
    
-   caseAutomaticClosureTemplate
    
-   caseCopyEmployeeTemplate
    
-   caseCreationTemplate
    
-   caseEscalationTemplate
    
-   caseUpdateTemplate
    
-   companyNameForSupportMessages
    
-   employeeCaseUpdateTemplate
    
-   mainSupportEmailAddress
    

### Related Topics

-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
