---
id: "section_N2490138"
type: "section"
title: "Manual Certificates FAQ"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Advanced Domain Setup > Manual Certificates > Manual Certificates FAQ"
parent: "section_N2485854"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html"
anchors: ["question_N2490158", "question_N2490220", "question_1505752578", "question_158098696197"]
sha256: "591ff414cd2fa6a44f6f4a95399ab15b60b5aed8f311b957636b43c2cdf25130"
---

### How do I generate a Certificate Signing Request (CSR)? {#question_N2490158}

See [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html) for information about what you need to do to generate a CSR in NetSuite. Next, follow the instructions for generating a CSR provided on the website of your certificate authority (CA). If you cannot find these instructions, contact your CA for details.

### What are the requirements for the SSL certificates I buy for the custom checkout domain I use with NetSuite? {#question_N2490220}

You can select an SSL certificate from the vendor of your choice, but it must meet the following requirements:

-   All SSL certificates you use with NetSuite require:
    
    -   A 2048-bit RSA (private and public) key. 4096-bit key lengths are not supported.
        
    -   The private key must use the PKCS#1 RSA Cryptography Standard.
        
        Note:
        
        The PKCS#8 Private-Key Information Syntax Standard is not supported. If the private key issued to you uses the PKCS#8 standard, see [How can I change the private key from PKCS#8 to PKCS#1?](#question_1505752578).
        
    -   Compatibility with Apache and encoded in PEM-format.
        
-   You are required to purchase SSL certificates that use the SHA-2 hash function or better. For more information, see [Supported TLS Protocol and Cipher Suites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1554220186.html).
    
-   The following are **not supported**:
    
    -   Wildcard certificates
        
    -   Self-signed certificates
        
    -   ECC (Elliptic Curve Cryptography) SSL certificates
        
    -   Subject Alternative Name (SAN) fields on an SSL certificate (that is, adding multiple domain names to a single certificate). Only the Subject Name on a certificate is considered. In cases where SANs are specified on a certificate (using a subjectAltName field), they are ignored.
        

Note:

To test if a certificate is trusted by your selected web browser, click the link in the **URL to Test Website or Example Cert** column of the [Mozilla Included CA Certificate List](https://wiki.mozilla.org/CA/Included_Certificates). You can purchase certificates from providers not listed in the Mozilla Included CA Certificate list. However, they may not be trusted by your browser. Contact your certificate provider for more information.

### How can I change the private key from PKCS#8 to PKCS#1? {#question_1505752578}

Some certificate providers generate the private key encrypted in the unsupported PKCS#8 key format. The unsupported PKCS#8 key starts with the following line:

              `-----BEGIN PRIVATE KEY-----` 
            

You can convert this unsupported PKCS#8 key to the PKCS#1 key format using the following command:

              `$ openssl rsa -in <my-key-filename>.key -out <my-key-filename>-rsa.key` 
            

The PKCS#1 formatted key starts with the following line:

              `-----BEGIN RSA PRIVATE KEY-----` 
            

### What happens if my manual SSL certificate expires? {#question_158098696197}

An expired certificate is automatically deleted 30 days after the expiration date, and makes your website inaccessible.

To avoid this, make sure your certificates are always valid (unexpired) for all your secure websites, including test websites.

### Related Topics

-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html)
-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html)
-   [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html)
-   [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html)
-   [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html)
-   [Maintenance of Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2489874.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
