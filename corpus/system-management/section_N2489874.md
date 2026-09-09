---
id: "section_N2489874"
type: "section"
title: "Maintenance of Manual Certificates"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Advanced Domain Setup > Manual Certificates > Maintenance of Manual Certificates"
parent: "section_N2485854"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2489874.html"
anchors: ["bridgehead_N2489900", "bridgehead_N2489916", "procedure_N2489935", "bridgehead_N2490036", "bridgehead_N2490048"]
sha256: "0ec128580642848612cca6f38369015b78321a66166fa85b366e445b29455826"
---

If you use a manual certificate to secure your web store, you are responsible for renewing and maintaining your SSL certificates with your certificate provider, as well as configuring DNS for your secure domains with your domain provider. Maintaining your certificates also includes updating information in NetSuite.

NetSuite is only responsible for allocating CNAME records for your checkout domain and the DNS verification, providing you with a CSR for your domain, and binding your SSL certificates to the CNAME.

Note:

This section is about maintenance tasks associated with your manual certificate. For information about purchasing certificates, generating CSRs, and securing domains with manual certificates, see [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html).

You are responsible for the following maintenance tasks associated with your secure domain:

-   [Renewal](#bridgehead_N2489900)
    
-   [Update Certificates in NetSuite](#bridgehead_N2489916)
    
-   [Upgrade](#bridgehead_N2490036)
    
-   [Revocation](#bridgehead_N2490048)
    

## Renewal {#bridgehead_N2489900}

Manual SSL certificates are valid for a certain period of time. You are responsible for keeping track of the date when it is time to renew your certificate with your certificate provider. NetSuite displays the valid dates for your certificate on your domain records.

Warning:

Ensure you use only valid (unexpired) certificates for your secure websites, including websites used for testing. If you do not renew the certificate, the website will become inaccessible seven days after the certificate expires, even if the user has previously accepted a security exception in the browser.

#### To view valid dates for an SSL certificate:

1.  Go to _Commerce > Hosting > Domains_.
    
2.  Click **View** for the desired domain.
    
3.  Review the **Certificate Status** field.
    

Contact your SSL certificate provider for more information about the maintenance tasks associated with your certificates.

## Update Certificates in NetSuite {#bridgehead_N2489916}

After you complete each of the maintenance tasks with your certificate provider, you must update the certificate information in NetSuite. This involves adding, deleting, and updating certificate files on the Domain record page.

Note:

Some certificate vendors, such as GoDaddy, may revoke an old certificate 72 hours after issuing a new one.

#### To update your certificate files in NetSuite: {#procedure_N2489935}

1.  Go to _Commerce > Hosting > Domains_.
    
2.  Click **Edit** next to the domain name whose certificate you want to update.
    
3.  Generate and download a new CSR file for the domain as described in [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html).
    
4.  Obtain a new SSL certificate from your certificate authority (CA) as described in [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html) and [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html).
    
5.  Click **Change Certificate** in the Certificate section.
    
6.  Click **Upload Certificate** and upload the certificate files provided to you by the CA. You can also drag and drop the certificate file into the specified area on the form.
    
    If your CA has given you an intermediate certificate (for example, secure.domainname\_ca.crt) as well as the SSL certificate (for example, secure.domainname.crt), make sure you select all the files at the same time during upload. You cannot upload them one at a time.
    
7.  Click **Save**.
    

Your existing secure domain is continuously served until the new certificate is deployed. NetSuite often deploys domains during the day. During this time, checkouts made through your secure domain are not interrupted. You will receive a notification email message when your new certificate is live.

## Upgrade {#bridgehead_N2490036}

You may be allowed to upgrade your SSL certificates based on the options provided by your certificate authority.

## Revocation {#bridgehead_N2490048}

You may need to revoke your certificate if it becomes compromised. When revoked, the certificate remains in NetSuite for seven days, after which it is removed. Before removal, the revoked certificate still allows customers to access the website after accepting a security exception offered by the browser. After removal, the website is no longer accessible.

### Related Topics

-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Manual Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2485854.html)
-   [Select Type of SSL Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486083.html)
-   [Generate a CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2486648.html)
-   [Submit Your CSR](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488102.html)
-   [Retrieve Your Certificates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2488299.html)
-   [Secure Domain Using Manual Certificate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158028805768.html)
-   [Manual Certificates FAQ](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2490138.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
