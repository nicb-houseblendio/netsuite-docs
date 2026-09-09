---
id: "section_N3418621"
type: "section"
title: "Support for Existing WSDL Versions"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > NetSuite WSDL Versioning > Support for Existing WSDL Versions"
parent: "section_N3418174"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html"
anchors: []
sha256: "23a61a1bf1724b3cb06b81568511db63ad8caa1a98a254c0b2788d6c5e8f6cfd"
---

Important:

Oracle NetSuite has scheduled the gradual removal of SOAP web services from the product as part of ongoing efforts to provide modern integration channels.

The 2025.2 SOAP endpoint is the last planned SOAP endpoint and any later SOAP endpoints would be released only as necessary to meet business, technical, or other significant requirements.

The support period of older endpoints is also affected and with the 2027.1 release, only the 2025.2 endpoint will be supported. With the 2028.2 release, SOAP will no longer be available in NetSuite and existing SOAP integrations with NetSuite will stop working. For more information, see [SOAP Removal Plans FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2104046421.html).

See also the [Removal of SOAP Web Services](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1021357/kw/1021357).

**SuiteTalk REST web services** is the technology intended to replace SOAP. All newly built integrations should use REST web services with OAuth 2.0 for authentication.

-   For any custom integration applications, that you have developed using SOAP, you should start planning the migration of your solution to REST as soon as possible. For a detailed guide for the migration, see [SOAP Web Services To Rest Web Services Upgrade Guide](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_8110600984.html).
    
-   If you use a partner SOAP application to integrate with NetSuite, consult with your partner to provide you with a REST-based application instead.
    
-   If you use an Oracle NetSuite integration application, a REST-based application will be provided by Oracle NetSuite.
    

With the new endpoint generally available, the following WSDL versions are still supported:

-   2025.2
    
-   2025.1
    
-   2024.2
    
-   2024.1
    
-   2023.2
    

After your NetSuite implementation is upgraded to a newer version, the oldest endpoint is no longer supported, but it is still available. If you use an older version, you should upgrade to the latest WSDL version or consider migrating your application to REST.

The following endpoints are still accessible, but no longer supported:

-   2023.1
    
-   2022.2
    
-   2022.1
    
-   2021.2
    
-   2021.1
    
-   2020.2
    
-   2020.1
    
-   2019.2
    

After your NetSuite implementation is upgraded to a newer version, retired endpoints are not available anymore.

Keep the following points in mind when planning to upgrade to a newer endpoint:

-   When you upgrade to a new version, support ends for the oldest supported endpoint, and the oldest available endpoint is retired.
    
-   Upgrade to a newer endpoint when your WSDL is retired, or your integrations will stop working because the old endpoint will be unavailable.
    

### Related Topics

-   [NetSuite Versioning and WSDL Versioning Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418264.html)
-   [Upgrading WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418339.html)
-   [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
