---
id: "section_N3413869"
type: "section"
title: "SOAP Web Services Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > SOAP Web Services Overview"
parent: "chapter_N3412777"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413869.html"
anchors: []
sha256: "be68fc79bb6d574753abf507281b73b15f515e7cbb89e94812225276601ff55a"
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
    

SOAP web services are Extensible Markup Language (XML) applications mapped to programs, objects, databases or complex business functions. They use a standardized XML messaging system to send or receive requests to authorized parties over the internet. Companies can use SOAP web services to create standardized processes that other organizations can use or integrate with their own processes. As each web service's programming logic is platform-independent, SOAP web services offer flexibility and independence for integration across businesses.

We use the following protocols to publish, expose or access SOAP web services:

-   WSDL (Web Services Description Language): a WSDL file exposes a Web service interface, interaction patterns and protocol mapping. WSDL can be readily interpreted by other applications, systems and platforms.
    
-   UDDI (Universal Description, Discovery and Integration): A Web Service can be categorized and registered in a UDDI Registry so that applications can locate it and retrieve its WSDL. Currently NetSuite does NOT provide a UDDI registry.
    
-   SOAP (Simple Object Access Protocol): A Web Service can use the SOAP messaging format to define an envelope for SOAP web services communication through HTTP, HTTPs or other transport layers.
    

With SOAP web services, you can integrate existing business functions within your organization to NetSuite through the use of web services. SOAP web services enable real-time operations like data retrieval, addition, update, and deletion.

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [NetSuite WSDL and XSD Structure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3413913.html)
-   [NetSuite WSDL Versioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418174.html)
-   [SOAP Web Services Performance Optimization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1537861842.html)
-   [SOAP Web Services Governance Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418637.html)
-   [Web Services and RESTlet Concurrency Governance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1500275531.html)
-   [Glossary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3419527.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
