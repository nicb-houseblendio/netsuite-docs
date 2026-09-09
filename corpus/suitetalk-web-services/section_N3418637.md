---
id: "section_N3418637"
type: "section"
title: "SOAP Web Services Governance Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > SOAP Web Services Governance Overview"
parent: "chapter_N3412777"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html"
anchors: ["bridgehead_N3418711", "bridgehead_N3418736", "bridgehead_N3419120", "bridgehead_N3419305", "bridgehead_N3419441"]
sha256: "39226333cbe71ca0ce5206500239f408a3e20b99c367f86a540042bb53953b5f"
---

Important:

Oracle NetSuite has scheduled the gradual removal of SOAP web services from the product as part of ongoing efforts to provide modern integration channels.

The 2025.2 SOAP endpoint is the last planned SOAP endpoint and any later SOAP endpoints would be released only as necessary to meet business, technical, or other significant requirements.

The support period of older endpoints is also affected and with the 2027.1 release, only the 2025.2 endpoint will be supported. With the 2028.2 release, SOAP will no longer be available in NetSuite and existing SOAP integrations with NetSuite will stop working.

For more details, see the [SOAP Removal Plans FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2104046421.html). For a list of the currently supported endpoints, see [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html).

Also, see [Removal of SOAP Web Services](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1021357/kw/1021357).

**SuiteTalk REST web services** is the technology intended to replace SOAP. All newly built integrations should use REST web services with OAuth 2.0 for authentication.

-   For any custom integration applications, that you have developed using SOAP, you should start planning the migration of your solution to REST as soon as possible. For a detailed guide for the migration, see [SOAP Web Services To Rest Web Services Upgrade Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_8110600984.html).
    
-   If you use a partner SOAP application to integrate with NetSuite, consult with your partner to provide you with a REST-based application instead.
    
-   If you use an Oracle NetSuite integration application, a REST-based application will be provided by Oracle NetSuite.
    

NetSuite uses mechanisms to optimize and control SOAP web services usage on its application and database servers. These mechanisms provide the following benefits:

-   Requests are monitored and controlled to prevent excessive impact on the user experience.
    
-   Heavy SOAP web services usage by some users does not affect other users.
    

NetSuite SOAP web services governance includes:

-   Record limiting (see [Understanding Record Limiting](#bridgehead_N3418711))
    
-   Request limiting (see [Understanding Request Limiting](#bridgehead_N3419305))
    

Note:

For information about the maximum number of sessions, see [Session Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html#bridgehead_N3447864).

Important:

For information about the new web services and RESTlet concurrency governance, see [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html).

## Understanding Record Limiting {#bridgehead_N3418711}

The following limits apply:

-   The number of records in a list operation.
    
-   The number of records in a page of search results. Search results are set by the pageSize field of the [searchPreferences complex type](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/other/searchpreferences.html?mode=package). A minimum and maximum exists for this parameter.
    

Limits differ for synchronous and asynchronous operations.

## Synchronous Operations {#bridgehead_N3418736}

| 
Operation or parameter

(on a per request basis)



 | Minimum Record Count | Maximum Record Count |
| --- | --- | --- |
| [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | \- | 200 |
| [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | \- | 200 |
| [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | \- | 1000 |
| [getItemAvailability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3498308.html) | \- | 10000 |
| [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | \- | 100 |
| [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html) | \- | 100 |
| pageSize parameter of searchPreferences complex type, when used in synchronous searches | 5 | 1000 |

## Asynchronous Operations {#bridgehead_N3419120}

| 
Operation or parameter

(on a per request basis)



 | Minimum Record Count | Record Count |
| --- | --- | --- |
| asyncAddList | \- | 400 |
| asyncGetList | \- | 2000 |
| asyncUpdateList | \- | 200 |
| asyncUpsertList | \- | 200 |
| asyncDeleteList | \- | 400 |
| pageSize parameter of searchPreferences complex type, when used in asynchronous searches | 5 | 2000 |

Note:

For details on asynchronous processing, see [Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3770809638.html).

## Understanding Request Limiting {#bridgehead_N3419305}

Request limits refer to the size of your SOAP request. The maximum allowed size for a SOAP request is 100MB.

## Understanding Governance Errors {#bridgehead_N3419441}

The following faults are thrown because of other governance violations.

-   **ExceededRecordCountFault** - thrown if a request exceeds the allowed record count.
    
-   **ExceededRequestLimitFault** - thrown if the allowed number of concurrent requests is exceeded.
    
-   **ExceededRequestSizeFault** - thrown if a request exceeds 100M.
    

For more information about exceptions, refer to [SOAP Web Services Error Handling and Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3536378.html).

For information about concurrency governance, see [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413869.html)
-   [NetSuite WSDL and XSD Structure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413913.html)
-   [NetSuite WSDL Versioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418174.html)
-   [SOAP Web Services Performance Optimization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1537861842.html)
-   [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html)
-   [Glossary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419527.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
