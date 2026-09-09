---
id: "section_N251955"
type: "section"
title: "NetSuite IP Addresses"
branch: "best-practices-for-cloud-accounts"
category: "account-administration"
breadcrumb: "Account Administration > Best Practices for Cloud Accounts > NetSuite IP Addresses"
parent: "chapter_4607562099"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N251955.html"
anchors: ["subsect_157062775551", "subsect_34144003415", "subsect_26143832518", "subsect_157062544703"]
sha256: "2558a4196762355d548179d4d7e1928debd912ed48336481bb898836985b6f4b"
---

Oracle NetSuite does not support the use of NetSuite IP addresses to access or manage access to any NetSuite services. There are better alternatives than using a list of allowed IP addresses to manage access to NetSuite. Using IP addresses (either as part of a URL or in your Domain Name Server, or DNS) to access NetSuite services prevents dynamic DNS routing.

Ensure that you understand the following:

-   **The IP addresses of NetSuite services may change at any time without notice.**
    
-   NetSuite Customer Support will not provide a list of NetSuite IP addresses.
    
-   NetSuite Customer Support will not be able to assist you when your integration breaks due to a change in NetSuite IP addresses.
    
-   Using IP addresses to directly access NetSuite services can result in unpredictable service outages or significant performance degradation.
    

## Managing Access to NetSuite Services {#subsect_157062775551}

You should not rely on methods that require explicit reference to any NetSuite IP address. Modifying the results of DNS translation prevents optimal resource allocation. This practice can cause unpredictable service outages or performance degradation.

See the following sections for more information:

-   [Managing Inbound Access](#subsect_34144003415)
    
-   [Managing Outbound Access](#subsect_26143832518)
    

### Managing Inbound Access {#subsect_34144003415}

You should not modify routing to NetSuite services by using IP addresses manually resolved from DNS.

For more information about alternatives to managing inbound access in NetSuite, see the following topics:

-   **User access to NetSuite:** See [Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N327688.html).
    
-   **SOAP web services:** See [Integration Record Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4389727047.html). See also [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html).
    
-   **RESTlets:** See [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html) and [OAuth 2.0](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157769826287.html).
    
-   **REST web services:** See [Setting Up Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0627022005.html).
    
-   **Client application access to NetSuite:** See [Token-based Authentication (TBA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4247329078.html).
    
-   **Access to NetSuite through SuiteAnalytics Connect (ODBC):** See [Authentication Using Server Certificates for ODBC](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4041410260.html).
    
-   **Websites and web stores:** See [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html).
    

### Managing Outbound Access {#subsect_26143832518}

Note:

IP addresses for outbound communication from NetSuite are not documented in the NetSuite Help Center.

This information is not available in SuiteAnswers either.

NetSuite Customer Support will not provide you with a list of services or IP addresses for outbound communication from NetSuite.

If you choose to use IP addresses to access or manage access to NetSuite services in firewall or proxy configuration, it is your responsibility to monitor for changes and update these settings when NetSuite IP address ranges change. If you decide to deploy a firewall, ensure that you have the resources to make it work in cloud environment.

For more information about alternatives to managing outbound access in NetSuite, see the following topics:

-   **Outbound HTTPS calls from NetSuite using SuiteScript 2.0:** Improve the security of integrations and customizations that use the [N/https Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4418229131.html) for outbound HTTPS calls from NetSuite to a third-party server. Your integrations and customizations should use client certificates for outbound HTTPS calls. Client certificates ensure authenticity of the traffic source. See [N/https/clientCertificate Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1543986321.html).
    
-   **Access to an external SFTP server from NetSuite:** See [SSH Keys for SFTP](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558548485.html). See also [SFTP Authentication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4855401415.html).
    
-   **DNS Lookups:** If you cannot take advantage of any of the previous options, advanced firewall tools can perform a lookup on the DNS record `outboundips.netsuite.com` and automatically grant access to requests from NetSuite. For outbound access, you can enter `outboundips.netsuite.com` as the fully qualified domain name (FQDN). You can use the FQDN, for example:
    
    -   To permit NetSuite through your firewall to connect to your FTP servers.
        
    -   To let a SuiteScript integration transmit data from NetSuite to an external system.
        
-   **Email services:** See [Email Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993117.html).
    

To access a NetSuite service (routing), see the following topics:

-   [Understanding NetSuite URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4295564687.html)
    
-   [URLs for Account-Specific Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498251763.html)
    

In cases where an application accesses more than one NetSuite account, you can use APIs for dynamic service discovery. See [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html).

## CDNs in the NetSuite Global Distribution Network {#subsect_157062544703}

Oracle NetSuite has enhanced our global distribution network by incorporating Content Delivery Networks, or CDNs. A CDN is a system of connected servers that improve application response times by caching and delivering data using the geographical proximity of a server to a person accessing a website.

Warning:

NetSuite cannot predict the IP addresses CDN providers use to serve `*.netsuite.com` requests.

Due to our partnership with CDN providers, we cannot predict the IP addresses that are used to serve inbound requests to `*.netsuite.com` requests. If you are programming a firewall for your company's outbound requests (inbound to NetSuite) please allow all `*.netsuite.com` entry points.

The authenticity of NetSuite services is ensured by PKI (Public Key Infrastructure) certificates.

### Related Topics

-   [Understanding NetSuite URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4295564687.html)
-   [URLs for Account-Specific Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498251763.html)
-   [Dynamic Discovery of URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7094653807.html)
-   [Supported TLS Protocol and Cipher Suites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1554220186.html)
-   [Secure HTTPS Outbound Communication and SSL Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162385234670.html)
-   [VPN Configuration for User Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161609571818.html)
-   [Traffic Health](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157437326499.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
