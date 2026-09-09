---
id: "section_N2486083"
type: "section"
title: "Select Type of SSL Certificate"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Advanced Domain Setup > Manual Certificates > Select Type of SSL Certificate"
parent: "section_N2485854"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html"
anchors: []
sha256: "08f936155cfb7e1e0819557ce14e33ad9233a4d6dc8e3ae6ff6654a060d86c4a"
---

The first step to acquiring a manual SSL certificate is to identify what type you need. You might want a manual certificate instead of the automatic one from NetSuite if you need an Extended Validation (EV) certificate for your domain. EV certificates require a more thorough validation process before they're issued.

You can select an SSL certificate from the vendor of your choice, but it must meet the following requirements:

-   All SSL certificates you want to use with NetSuite require:
    
    -   A 2048-bit RSA (private and public) key. 4096-bit key lengths are not supported.
        
    -   The private key must use the PKCS#1 RSA Cryptography Standard.
        
        Note:
        
        The PKCS#8 Private-Key Information Syntax Standard isn't supported. See [How can I change the private key from PKCS#8 to PKCS#1?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html#question_1505752578) if the private key issued to you uses the PKCS#8 standard.
        
    -   Must be Apache-compatible and PEM-encoded.
        
-   You need to buy SSL certificates that use the SHA-2 hash function or better. For more information, see [Supported TLS Protocol and Cipher Suites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1554220186.html).
    
-   The following are **not supported**:
    
    -   Wildcard certificates
        
    -   Self-signed certificates
        
    -   ECC (Elliptic Curve Cryptography) SSL certificates
        
    -   Subject Alternative Name (SAN) fields on an SSL certificate (that is, adding multiple domain names to a single certificate). Only the Subject Name on a certificate is considered. In cases where SANs are specified on a certificate (using a subjectAltName field), they are ignored.
        

For a list of certificate authorities, see the [Mozilla Included CA Certificate List](https://wiki.mozilla.org/CA/Included_Certificates).

Note:

To test if a certificate is trusted by your selected web browser, click the link in the **URL to Test Website or Example Cert** column of the [Mozilla Included CA Certificate List](https://wiki.mozilla.org/CA/Included_Certificates). You can buy certificates from providers not on the Mozilla Included CA Certificate list, but they might not be trusted by all browsers or by NetSuite. Check with your certificate provider for more information.

### Related Topics

-   [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html)
-   [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html)
-   [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html)
-   [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html)
-   [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html)
-   [Maintenance of Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2489874.html)
-   [Manual Certificates FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
