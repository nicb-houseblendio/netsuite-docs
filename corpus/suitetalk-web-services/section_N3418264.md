---
id: "section_N3418264"
type: "section"
title: "NetSuite Versioning and WSDL Versioning Overview"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > NetSuite WSDL Versioning > NetSuite Versioning and WSDL Versioning Overview"
parent: "section_N3418174"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418264.html"
anchors: []
sha256: "efe7005e76385dad049fef7473e66699dac27e2c27d3ac02784cda0e78487a97"
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
    

The naming convention for NetSuite versions and WSDL versions are the same. For example, for 2025.2, there is an accompanying 2025\_2 version of the WSDL, as shown in the following WSDL URLs:

[https://webservices.netsuite.com/wsdl/v2025\_2\_0/netsuite.wsdl](https://webservices.netsuite.com/wsdl/v2025_2_0/netsuite.wsdl)

[https://content.netsuite.com/download/WSDL\_v2025\_2\_0.zip](https://content.netsuite.com/download/WSDL_v2025_2_0.zip)

NetSuite WSDL versioning denotes:

-   the major version: **v2025\_2**
    
-   the minor or patch version: **\_0**
    

Typically, a new NetSuite release includes a WSDL version that supports the latest features and enhancements. For instance, when new workflows or records are added to NetSuite, the corresponding WSDL usually includes new operations or records to match these enhancements. In some releases, a new WSDL also includes enhancements to the SOAP web services platform itself. These enhancements are independent of NetSuite product enhancements.

Note that upgrading your NetSuite account doesn't necessarily mean you need to upgrade your WSDL version. For instance, you can continue using the 2025.1 WSDL with a NetSuite account that's been upgraded to 2025.2. For more information, see [Upgrading WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418339.html).

When a new NetSuite release and WSDL version are available, review the relevant sections of the Sneak Peeks and Release Notes. These documents list all of the new functionality and any schema bug fixes offered in the latest WSDL.

### Related Topics

-   [Upgrading WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418339.html)
-   [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html)
-   [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
