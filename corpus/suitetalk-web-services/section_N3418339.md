---
id: "section_N3418339"
type: "section"
title: "Upgrading WSDL Versions"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SuiteTalk SOAP Web Services Platform Overview > NetSuite WSDL Versioning > Upgrading WSDL Versions"
parent: "section_N3418174"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418339.html"
anchors: ["bridgehead_N3418438", "bridgehead_N3418462", "bridgehead_N3418588"]
sha256: "f309d8e113d708f9b18b7c2e3dc3d2d37de305aa2221edbdb68400ca36ad6bcc"
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
    

NetSuite customers typically upgrade their WSDL when a new version offers features that address a specific business requirement. They also upgrade when NetSuite announces the end of support for their current WSDL version. For more details, see [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html). When you upgrade the WSDL you are using, it's best to upgrade to the latest available version to prolong the life cycle for your integrated application.

Important:

You are not always required to upgrade your WSDL when your NetSuite account is upgraded. However, when your account is upgraded, you should re-test all existing integrations to ensure they work against the latest version of NetSuite (see [Testing After a NetSuite Upgrade](#bridgehead_N3418462) for details). Also, you should consider that when your NetSuite account is upgraded to the newest version, the oldest available WSDL is automatically retired and stops working. You must upgrade your WSDL before NetSuite retires it. See [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html) for more details.

For help with upgrading your WSDL, reach out to your integration's developer, as each application has its own upgrade process.

After a WSDL upgrade, your development environment will show any API incompatibilities between the old and new versions. You won't be able to proceed with unit testing until you've resolved any compilation errors in your IDE. So, most WSDL upgrade issues are typically resolved during the development phase.

A WSDL upgrade might require re-coding parts of your integrated application to ensure compatibility with the latest NetSuite version. You might need to re-code due to various reasons, including:

-   A new required field has been added to NetSuite.
    
-   A field that was optional in previous versions of NetSuite becomes required in the latest version.
    
-   A field that is referenced in your integration has been removed from NetSuite.
    
-   The data type for a field has changed.
    
-   The method signature changes for a SOAP web services operation that is used in your integration.
    
-   The authentication method has changed.
    

Note:

See [Working with the Araxis Merge Diff File](#bridgehead_N3418588) for information about how to use Araxis to see the changes made from one WSDL version to the next. You can also get an idea of the types of changes you must make by reading the release notes from the endpoint you are currently using onwards to the last release of the WSDL.

## Testing After a WSDL Upgrade {#bridgehead_N3418438}

When upgrading your WSDL to use a new NetSuite feature, start by exploring how it works in the UI. In most cases, Generally, NetSuite SOAP web services mirrors the UI, making it easier to understand how features work programmatically. Therefore, familiarizing yourself with a feature in the UI will reduce the time it takes to learn how to use it in SOAP web services.

Note that WSDL upgrades require significant planning and testing. Consequently, you might choose to upgrade only when your current version is nearing retirement. (See [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html) for more information.)

## Testing After a NetSuite Upgrade {#bridgehead_N3418462}

NetSuite aims to maintain backward compatibility from one NetSuite version to the next. However, custom workflows in your integration might be affected when your NetSuite account is upgraded. Therefore, you should test all existing integrations in your Release Preview account for the NetSuite upgrade and report any issues you may find to ensure a smooth upgrade of your production account.

In your Release Preview account, you also must modify the WSDL references you are using in your application to point to one of the following endpoints (based on the endpoint you are currently using):

Note:

You can access the UI for your Release Preview account from https://system.netsuite.com. Initially, only users with an Administrator role have access to the Release Preview account. For more information, see [The Release Preview Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1121105228.html).

-   https://webservices.netsuite.com/wsdl/v2025\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2025\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2024\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2024\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2023\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2023\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2022\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2022\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2021\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2021\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2020\_2\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2020\_1\_0/netsuite.wsdl
    
-   https://webservices.netsuite.com/wsdl/v2019\_2\_0/netsuite.wsdl
    

Note:

If you are engaged with a partner for any of your SOAP web services integrations, you should contact them and inform them of when your Release Preview account will be available. They can then set up a time with you and a test plan for the integration.

## Working with the Araxis Merge Diff File {#bridgehead_N3418588}

Use the Araxis diff file in the release notes to compare the latest WSDL with its predecessor. In the diff file, begin by investigating the records you're currently working with. For example, if your application uses customer and vendor records, check the diff file for updates to these records. Look for changes like new or removed fields, or changes to field data types.

ITo compare the latest WSDL with your current version, download [Araxis](http://www.araxis.com/) and compare it with any version available on the Developer Portal.

For more information about using the Araxis diff file to review NetSuite WSDL changes, see _Araxis Merge Diff File for the 2025.2 Endpoint_ in the 2025.2 Release Notes.

### Related Topics

-   [NetSuite Versioning and WSDL Versioning Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418264.html)
-   [Support for Existing WSDL Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3418621.html)
-   [SOAP Web Services Archives](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3892701016.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
