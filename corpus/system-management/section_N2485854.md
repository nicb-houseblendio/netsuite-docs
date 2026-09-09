---
id: "section_N2485854"
type: "section"
title: "Manual Certificates"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Advanced Domain Setup > Manual Certificates"
parent: "chapter_1521812758"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html"
anchors: []
sha256: "9d0f3b883fc1644f8e025dc9ff2d216f16000c62a69a8b45dbe90bf3489b6df0"
---

To secure a domain in NetSuite using an SSL certificate from a certificate authority (CA) of your choice, you must first acquire the SSL certificate. Complete the following steps to do this:

1.  **Confirm you have access to the required features associated with secure domains.** Certain fields that are required for the secure domain setup process in NetSuite do not appear unless you have enabled the required features. See [Set Up Domains for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2484898.html).
    
    Note:
    
    A fixed number of secure domain licenses are included with a Commerce web store license. If you need more secure domains, you need to obtain additional secure domain licenses or free up one of your existing licenses. See [Secure Domain Licenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1498574038.html) for more information.
    
2.  **Identify the type of SSL certificate you need.** For information about selecting an SSL certificate type, see [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html).
    
3.  **Generate and download a Certificate Signing Request (CSR).** The CA uses the CSR to verify your company's identity.
    
    To obtain a CSR for your secure domain, you first need to set up the domain with the correct domain name. For information about downloading the CSR for your domain, see [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html).
    
    Warning:
    
    Be aware of the following:
    
    -   You must download the CSR file from the Domain record page in NetSuite. If you use any other CSR to get your SSL certificate, it won't work to secure your NetSuite domain.
        
        To view the Domain record page, go to Commerce > Hosting > Domains and click **View** next to your domain name.
        
    -   You must generate and download the CSR file on the same day. If you don't, you may not be able to upload your certificate in NetSuite.
        
    -   If you don't click **Save** after you download your CSR file, you may not be able to upload your certificate in NetSuite.
        
    -   For more information, see [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html).
        
    
4.  **Submit your CSR to the CA.** After you have obtained the CSR for your domain, you must submit it to the CA. This is something you do outside of NetSuite. For more information, see [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html).
    
5.  **Retrieve your certificates.** After the CA notifies you that your SSL certificate is ready, you must retrieve your certificate files. This is something you do outside of NetSuite. For more information, see [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html).
    
6.  **Secure your domain using the SSL certificates.** After you've downloaded your certificate files, link them to your domain to secure it. For information about how to do this, see [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html).
    

For information about the difference between automatic and manual certificates, see [Automatic and Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157538985860.html).

### Related Topics

-   [Advanced Domain Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1521812758.html)
-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html)
-   [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html)
-   [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html)
-   [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html)
-   [Maintenance of Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2489874.html)
-   [Manual Certificates FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
