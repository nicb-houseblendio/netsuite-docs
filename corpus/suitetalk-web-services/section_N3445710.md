---
id: "section_N3445710"
type: "section"
title: "Authentication for SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Security > Authentication for SOAP Web Services"
parent: "chapter_N3445516"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html"
anchors: ["bridgehead_4489663579", "bridgehead_4489663126", "bridgehead_4489664235"]
sha256: "361f93d6978d9189e31edf28c29fe491ffd4b050423a2401f00e6aed8aeff5d0"
---

Authentication is the process of determining the identity of requesters by verifying the credentials they present. Most SOAP web services operations require authentication.

The available methods of authentication include the following:

-   [Token-Based Authentication](#bridgehead_4489663579)
    
-   [User Credentials](#bridgehead_4489663126)
    

Important:

Use only one authentication method in one SOAP message. Mixing different authentication types in a single SOAP message returns a SOAP fault.

## Token-Based Authentication {#bridgehead_4489663579}

With this approach, the request must include a consumer key, a token, and other data. Authentication details must be sent by using request-level credentials, not the login operation. For details on structuring a SOAP request this way, see [Request-Level Credentials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489690806.html#bridgehead_N3447228).

You generate a consumer key and secret when you create an integration record and configure the record to permit token-based authentication (by checking the **Token-based Authentication** box). For details, see [Integration Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4399047360.html).

Important:

Token-based authentication is supported for use only with the 2015.2 endpoint and later.

## User Credentials {#bridgehead_4489663126}

Important:

As of the 2020.2 SOAP web services endpoint, authentication through request-level credentials is not supported. The [Passport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3453226) complex type is not supported. If you attempt to authenticate through request-level credentials in SOAP web services 2020.2 and later endpoints, the web services request is not processed, and an error message is returned. You must ensure that SOAP web services integrations created with 2020.2 and later SOAP web services endpoints use TBA. Authentication through user credentials continues to be supported in integrations that use SOAP web services 2020.1 and earlier endpoints. For more information, see [Token-based Authentication and Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4381113277.html).

With this approach, the request must include the credentials associated with a single user: an email address, password, role, and NetSuite account ID. To find your account ID, go to the SOAP Web Services Preferences page at _Setup > Integration > Integration Management > SOAP Web Services Preferences_. For a list of NetSuite role internal IDs, see [Internal IDs Associated with Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3427186.html).

When you authenticate by using user credentials, there are two approaches to how the SOAP request may be structured: you can use the login operation or you can use request-level credentials. For details, see [Structuring SOAP Requests to Include Authentication Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4489690806.html).

For requests that use the 2015.2 WSDL or later, application ID is also required, although technically application ID is not considered a part of the user authentication process. An application ID is used to link a request to an integration record that exists in your NetSuite account. To use any integration record for requests that authenticate through user credentials, the record must have the **User Credentials** box checked. For details, see [Integration Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4399047360.html).

## Outbound Single Sign-on (SuiteSignOn) {#bridgehead_4489664235}

This approach allows an external application to perform callbacks to NetSuite after the SuiteSignOn handshake is complete and there is a live SuiteSignOn token. For more information about SuiteSignOn, see [Outbound Single Sign-on (SuiteSignOn)](#bridgehead_4489664235).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html)
-   [Authentication for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html)
-   [Using the Login Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1521211724.html)
-   [Authorization for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447510.html)
-   [Session Management for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html)
-   [Encryption for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448169.html)
-   [Custom Field Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448524.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
