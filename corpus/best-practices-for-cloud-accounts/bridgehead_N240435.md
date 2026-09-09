---
id: "bridgehead_N240435"
type: "bridgehead"
title: "Dynamic URL Discovery for SOAP Web Services"
branch: "best-practices-for-cloud-accounts"
category: "account-administration"
breadcrumb: "Account Administration > Best Practices for Cloud Accounts > Dynamic Discovery of URLs > Dynamic URL Discovery for SOAP Web Services"
parent: "article_7094653807"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N240435.html"
anchors: []
sha256: "bd3205cd620d55f1e7e3bd6aae303ffe13b2fae0a92887b6b6c4e1a220fb884f"
---

When sending requests to a NetSuite account, an external client needs to use the account's correct domain name. For example, a SOAP web services request must be sent to the account's correct web services domain.

You can use the SOAP web services operation [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) to achieve this. Send the getDataCenterUrls request to webservices.netsuite.com, the NetSuite web services dynamic discovery domain: **webservices.netsuite.com**. The getDataCenterURLs operation helps you retrieve the correct SOAP web services domain name for a specified NetSuite account. You can use this operation in production, sandbox, and Release Preview accounts.

Important:

The dynamic discovery service is upgraded early and independently of your account, so [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) may be processed with the new WSDL version, even though the target account hasn't been upgraded yet. If your integration uses an older endpoint like 2018\_2 and is negatively impacted, use one of the following alternatives:

-   Use one of the supported endpoints for the NetSuite 2025.2 release on all SOAP calls, ideally the 2025\_1 endpoint.
    
-   Instead of dynamic discovery [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) requests use the Account Specific Endpoint (Setup > Company > Company Information > Company URLs | SuiteTalk SOAP URL) to target all SOAP calls. This way it is still possible to use https://<accountID>.suitetalk.api.netsuite.com/services/NetSuitePort\_2018\_2, if your own account is on the 2025.1 version.
    
-   Append the URL parameter NS\_VER=2025.1 on your endpoint URL for your initial dynamic discovery [getDataCenterUrls](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3494684.html) request (https://webservices.NetSuite.com/services/NetSuitePort\_2018\_2?NS\_VER=2025.1). This will force routing for this initial request to system endpoint where it will not fail.
    

### Related Topics

-   [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html)
-   [Dynamic URL Discovery for RESTlet Clients](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7155543679.html)
-   [The DataCenterUrls REST Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157011836591.html)
-   [The REST Roles Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157011522878.html)
-   [Understanding NetSuite URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4295564687.html)
-   [NetSuite IP Addresses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N251955.html)
-   [Understanding NetSuite URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4295564687.html)
-   [URLs for Account-Specific Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498251763.html)
-   [Supported TLS Protocol and Cipher Suites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1554220186.html)
-   [Secure HTTPS Outbound Communication and SSL Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162385234670.html)
-   [VPN Configuration for User Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161609571818.html)
-   [Traffic Health](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157437326499.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
