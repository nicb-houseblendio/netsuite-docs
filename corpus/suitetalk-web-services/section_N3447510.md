---
id: "section_N3447510"
type: "section"
title: "Authorization for SOAP Web Services"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Platform Guide > SOAP Web Services Security > Authorization for SOAP Web Services"
parent: "chapter_N3445516"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447510.html"
anchors: ["bridgehead_N3447527"]
sha256: "a4e676ab55939565830e82915b58cdcc710a64222bca40d259d5c289016e1f67"
---

Authorization is the process of ensuring that the requester has the appropriate entitlement to perform the requested operation. When users request to be authenticated, they also provide their NetSuite role. For every SOAP web services request, the system uses the role definition to ensure that the user has the required permission for the requested operation as well as the requested record type. The role must be provided in the Passport type through the login operation:

Important:

As of the 2020.2 SOAP web services endpoint, authentication through request-level credentials is not supported. The [Passport](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3452954.html#bridgehead_N3453226) complex type is not supported. If you attempt to authenticate through request-level credentials in SOAP web services 2020.2 and later endpoints, the web services request is not processed, and an error message is returned. You must ensure that SOAP web services integrations created with 2020.2 and later SOAP web services endpoints use TBA. Authentication through user credentials continues to be supported in integrations that use SOAP web services 2020.1 and earlier endpoints. For more information, see [Token-based Authentication and Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4381113277.html).

## Example {#bridgehead_N3447527}

          `<soapenv:Body            <login xmlns="urn:messages_2018_1.platform.webservices.netsuite.com">                <passport>                    <ns1:email xmlns:ns1="urn:core_2018_1.platform.webservices.netsuite.com">test@netsuite.com</ns1:email>                    <ns2:password xmlns:ns2="urn:core_2018_1.platform.webservices.netsuite.com">********</ns2:password>                    <ns3:account xmlns:ns3="urn:core_2018_1.platform.webservices.netsuite.com">1234567</ns3:account>                    <ns4:role internalId="37" xmlns:ns4="urn:core_2018_1.platform.webservices.netsuite.com"/>                </passport>            </login>        </soapenv:Body>` 
        

For detailed information about NetSuite roles and permissions and how SOAP web services implement roles and permissions rules, refer to [Roles and Permissions in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3424144.html).

### Related Topics

-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)
-   [SOAP Web Services Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3445516.html)
-   [Authentication for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3445710.html)
-   [Session Management for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3447680.html)
-   [Encryption for SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448169.html)
-   [Custom Field Security](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3448524.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
