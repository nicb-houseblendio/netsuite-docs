---
id: "section_N2486648"
type: "section"
title: "Generate a CSR"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Advanced Domain Setup > Manual Certificates > Generate a CSR"
parent: "section_N2485854"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html"
anchors: []
sha256: "5859ab808c51ce17b475783e146bddf68c121941d61def17f16c8f0fdb5ebbc3"
---

Warning:

You must download your Certificate Signing Request (CSR) file from the Domain record page in NetSuite. If you obtain an SSL certificate using any other CSR, the certificate cannot be used to secure your NetSuite domain.

To view the Domain record page, go to Commerce > Hosting > Domains and click **View** next to your domain name.

#### To generate a CSR:

1.  After you have completed the initial domain setup steps specified in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html), click **Generate CSR File** on the Domain record page in NetSuite to generate the CSR file. This can take up to 15 minutes.
    
    To view the Domain record page, go to Commerce > Hosting > Domains and click **View** next to your domain name.
    
2.  When your CSR file is ready, click **Download CSR File** to download the file to your computer.
    
    You must submit the CSR file to your Certificate Authority (CA) when you purchase an SSL certificate for your domain. For more information, see [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html).
    
    Warning:
    
    You must generate and download the CSR file on the same day. If you do not do this, you may not be able to upload your certificate in NetSuite.
    
3.  The next step is to add the SSL certificate. However, it typically takes some time for the CA to issue a certificate after you submit the CSR so click **Save** to save the domain record with the existing information.
    
    Note:
    
    The domain is not deployed until you upload the certificate.
    
    Warning:
    
    If you do not click **Save** after you download your CSR file, you may not be able to upload your certificate in NetSuite.
    

### Related Topics

-   [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html)
-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html)
-   [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html)
-   [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html)
-   [Maintenance of Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2489874.html)
-   [Manual Certificates FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
