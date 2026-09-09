---
id: "section_N2479403"
type: "section"
title: "Point Your Domain Name at Your Domain (DNS Settings)"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Set Up Domains for Web Stores > Point Your Domain Name at Your Domain (DNS Settings)"
parent: "section_N2484898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html"
anchors: ["bridgehead_4243064238"]
sha256: "af536061128228a978ee77ed1a206db10c8b5feb559126a67970f0b97383840f"
---

To ensure visitors to your website (for example, `www.example.com`) arrive at your NetSuite-hosted domain, you need to configure DNS settings with your domain name provider. Your domain name provider uses DNS settings to send visitors to the domain hosted on NetSuite servers.

In non-technical terms, configuring DNS settings is like setting up a mail redirection when you move house - you tell the post office (domain name provider) to send all letters addressed to your old address (your domain name) to your new address (your NetSuite-hosted domain). The people sending you letters use your old address but you receive them at the new address. The information the post office holds, mapping your old address to your new address, is the equivalent of DNS settings.

Your domain provider uses CNAME records to make your domain name an alias for the NetSuite-hosted domains linked to your account. You can get the CNAME records for your domain hosting and DNS verification from the NetSuite Domain record.

When you're setting up DNS settings with your domain provider, be aware of the following:

-   Domain names should always point to a CNAME record. CNAME records must be correctly set up at all times to avoid issues with SSL certificates and securing your domain.
    
-   If you're using CNAME flattening (also known as a dynamic A record or ANAME record), the records must be correctly set up with your domain provider. See [CNAME Flattening (Dynamic A Record)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1547053319.html).
    
-   Wildcard DNS records aren't supported.
    
-   NetSuite provides CDN and caching services, which must be enabled in NetSuite. Third-party CDN and caching services are not supported and must not be used as they can cause operational issues. See [Enable CDN Caching](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4636849610.html).
    
-   All domain types available in NetSuite must be secured. See [Secure Your Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603043411.html).
    
-   When you're using a secure domain, you'll also need to set up a CNAME record for DNS verification with your domain provider. See [Set Up DNS Verification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603035652.html).
    

For more information about the importance of proper DNS setup and the risks of improper DNS setup, see [Importance of Proper DNS Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1115112645.html).

For information about the different types of CNAME records you can set up for your Commerce website, see the following topics:

-   DNS verification record - See [Set Up DNS Verification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603035652.html).
    
-   DNS hosting record (CNAME) - See Step 3 of the process documented in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html).
    
-   CNAME flattening/Dynamic A record - See [CNAME Flattening (Dynamic A Record)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1547053319.html).
    

Important:

When setting up your DNS, ensure that the time to live (TTL) is not higher than 3600 (an hour in seconds). If you exceed this value, you can encounter issues with your domain.

#### To configure DNS settings with your domain provider:

1.  Obtain the CNAME records for your domain as described in Step 3 of the help topic, [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html).
    
    The CNAME records for your domain will resemble the following example:
    
    ![Example of CNAME records on NetSuite Domain record page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/SystemManagement/Domains/CNAMERecordsRedwood.png)
    
    Note:
    
    The CNAME records assigned to each domain name in each NetSuite account are unique. Make sure you copy the CNAME records for the domain you want to set up.
    
2.  Log in to your domain provider's website to manage DNS settings and to set up CNAME records.
    
    Note:
    
    DNS configuration is a task that you complete outside of NetSuite.
    
    Important:
    
    Changing DNS settings affects the ability to view your website. Therefore, changes should be made by someone with DNS setup experience. Also, consider consulting with your domain provider before updating your DNS settings.
    
3.  Configure the DNS settings using the instructions provided by your domain provider. Most providers have online help with step-by-step guides for adding and editing CNAME records. Instructions vary depending on the domain provider.
    
4.  After you've set up the DNS settings with your domain provider, you'll need to set up the domain record in NetSuite. For more information, see [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html).
    
    If the domain record already exists in NetSuite, go to the Domain record page, click **Edit** and then click **Save**. This redeploys the domain record and connects it to your domain name. For more information about deploying a domain, see [Deploy Your Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603043220.html).
    

## Add or Change a Domain Name {#bridgehead_4243064238}

Every time you add a new domain name in NetSuite, you'll need to use the CNAME records shown for that domain to set up DNS with your domain provider. The CNAME records are displayed on the Domain record in NetSuite.

Changing your domain name is not supported in NetSuite. If you want to change the domain name, you must delete the old domain and create a new one. Then, set up the DNS with your domain provider and use the CNAME records shown for the new domain in NetSuite.

### Related Topics

-   [Set Up Domains for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2484898.html)
-   [Importance of Proper DNS Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1115112645.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
