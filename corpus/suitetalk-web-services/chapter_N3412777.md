---
id: "chapter_N3412777"
type: "chapter"
title: "SuiteTalk SOAP Web Services Platform Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview"
parent: "book_156388532579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html"
anchors: ["bridgehead_1507208354"]
sha256: "deac68196d68ebf69c801b5e311157deac8afd9716cb845598b9c419bc90dd70"
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
    

The SOAP web services platform provides programmatic access to your NetSuite data and business processes through an XML-based application programming interface (API). The SOAP web services platform has the following key characteristics:

-   **SOAP encoded web services** - the Platform uses SOAP-based web services with document style, or Doc style, encoding.
    
    Doc style encoding uses message-oriented exchanges, where an XML schema in the the SOAP message defines the message structure between two applications. RPC exchanges are NOT supported.
    
-   **HTTPS Transport** - currently the only transport supported is HTTPS as defined in the WSDL document.
    

For a list of NetSuite records that are supported in SOAP web services development, see [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html) and the [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html) . To see code samples of all SOAP web services operations, see [SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html).

NetSuite regularly updates its server certificates and trusted certificate store to ensure the highest security standards for connectivity. Client applications integrating with NetSuite should use an updated certificate store to prevent integration issues due to expired or changed certificates. This issue typically does not affect modern browsers because these clients are maintained to use the latest certificates.

Important:

The following material applies to the 2025.2 WSDL, but NetSuite also supports earlier endpoints. For documentation about older endpoints that are supported, see [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html). For more information, see also [NetSuite WSDL and XSD Structure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413913.html) and [NetSuite WSDL Versioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418174.html).

## In This Guide {#bridgehead_1507208354}

Explore to the following sections to learn more about the SOAP web services platform:

[SOAP Web Services Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3419686.html) - helps you set up your SOAP web services development environment and create your first service. It also describes how to modify or set SOAP web services preferences. This section also describes general concepts that pertains to SOAP web services development.

[SOAP Web Services Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3422061.html) - covers setting company-wide, request-level, and search preferences, as well as Internal ID preferences.

[Integration Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4399047360.html) - provides information about managing external applications by using integration records.

[Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html) - defines the concept of a role within NetSuite and the necessity of providing a role ID during authentication. This section also describes how to assign a default role to a SOAP web services user, as well as how to set a 'Web Services Only' role for a user.

[Records, Fields, Forms, and Sublists in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3428523.html) - describes how to work with records, fields, and sublist objects in SOAP web services. This section also provides information about working with custom forms.

[SOAP Web Services Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3444088.html) - describes how to process requests synchronously versus asynchronously. Also provided are steps for monitoring your SOAP web services requests.

[SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html) - describes all aspects of SOAP web services security and session management.

[Platform Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3448700.html) - describes the Web Services Concurrent License.

[Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3452524.html) - describes the various types available in the SOAP web services platform.

[SOAP Web Services Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3477815.html) - describes each operation that can be performed through SOAP web services and provides SOAP, C# and Java code samples.

[SOAP Web Services PHP Toolkit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3533866.html) - describes the tools that assist in the development of PHP applications that interface to the SOAP web services platform.

[SOAP Web Services Error Handling and Error Codes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3536378.html) - provides tables of possible SOAP faults, fault status codes and error status codes that can be thrown for a particular request.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
