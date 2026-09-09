---
id: "section_N3752734"
type: "section"
title: "Revenue Recognition Schedule"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Lists > Revenue Recognition Schedule"
parent: "chapter_N3739470"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3752734.html"
anchors: ["bridgehead_N3753350", "bridgehead_N3753524", "bridgehead_4157312542"]
sha256: "23767eba24d65c365b95b1ef31dd489e25c020c988b938c43c90bba2d180eb11"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Revenue Recognition Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2100141079.html).

A revenue recognition schedule indicates the posting periods in which revenue should be recognized, and the amount to be recognized in each period, for an item sale. A revenue recognition schedule is generated for any sales transaction item that has an associated revenue recognition template. The point at which a revenue recognition schedule is generated for an item sale depends upon the type of sales transaction and enabled features and preferences set in your account. The schedule could be generated when a transaction is first saved, when it is approved, or when it is billed. Revenue recognition schedules provide a basis for the generation of journal entries that record the impact of item sales. This record is available when the Revenue Recognition feature is enabled. For more details, see [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html).

Revenue recognition schedules are system-generated. In SOAP web services, you can get or search this type of record's data, and edit the name field only. To make other changes, you need to modify the associated revenue recognition template. See [Revenue Recognition Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3753754.html).

The Revenue recognition schedule record is defined in the [listAcct (accounting)](https://webservices.netsuite.com/xsd/lists/v2025_2_0/accounting.xsd) XSD.

## Supported Operations {#bridgehead_N3753350}

The following operations can be used with the revenue recognition schedule record.

[get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3753524}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [revenue recognition schedule](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/revrecschedule.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_4157312542}

If you are using an endpoint that predates 2014.2, be aware of the following: Some fields have been deprecated for both RevRecScheduleSearchBasic and RevRecScheduleSearchRowBasic. That is, regardless of which endpoint you are using, these fields are no longer honored.

The fields no longer honored in RevRecScheduleSearchBasic include the following:

-   defRev
    
-   entity
    
-   externalId
    
-   externalIdString
    
-   incomeAcct
    
-   srcDoc
    
-   srcDocDate
    

The fields no longer honored in RevRecScheduleSearchRowBasic include the following:

-   defRev
    
-   entity
    
-   externalId
    
-   incomeAcct
    
-   postPeriod
    
-   srcDoc
    

### Related Topics

-   [Revenue Recognition Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3753754.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3739470.html)
-   [Other Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3757146.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Working with Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1691981.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
