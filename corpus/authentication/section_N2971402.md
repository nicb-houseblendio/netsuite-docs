---
id: "section_N2971402"
type: "section"
title: "Authentication for RESTlets"
branch: "authentication"
category: "account-administration"
breadcrumb: "Account Administration > Authentication > RESTlet Authentication > Authentication for RESTlets"
parent: "chapter_1529417663"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2971402.html"
anchors: []
sha256: "353d41fe161be0350305267ab5ca1b8b97c3ecdb4add15009ab83954661866e4"
---

RESTlets must use REST URLs to connect to NetSuite. If the RESTlet call comes from an external client, the URL must include a domain specific to your NetSuite account. To handle this task, you can also use the roles service, as described in [The REST Roles Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157011522878.html).

-   For a RESTlet called from an external client, you can use OAuth or the NetSuite-specific method NLAuth in the HTTP Authorization header. OAuth uses token-based authentication (TBA) or OAuth 2.0 to access resources on behalf of a user, without sharing login credentials. You should use OAuth 2.0 for RESTlet authentication. For more information, see the following topics:
    
    -   [OAuth 2.0 for Integration Application Developers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157780218434.html) for OAuth 2.0.
        
    -   [The Three-Step TBA Authorization Flow](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156337186044.html) for TBA.
        
    
    NLAuth passes in NetSuite login credentials such as company ID, user name, password, role, and application ID. See [Using User Credentials for RESTlet Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4623992425.html). NetSuite doesn't support user credentials authentication for new RESTlets.
    
-   For a RESTlet called from a client hosted by the same NetSuite account that hosts the RESTlet, you don't need to pass authentication information in the HTTP request. This doesn't apply to Suitelets. A check for all valid NetSuite session cookies occurs, and this existing session is reused.
    

Important:

RESTlet authentication can use either the HTTP Authorization header or all session cookies, but not both. Ensure that your script uses only one form of authentication.

### Related Topics

-   [Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_4299752196.html)
-   [RESTlet Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1529417663.html)
-   [Setting up Token-based Authentication for a RESTlet integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530099787.html)
-   [Setting up OAuth 2.0 for a RESTlet Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158263562006.html)
-   [Using User Credentials for RESTlet Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4623992425.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
