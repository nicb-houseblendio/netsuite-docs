---
id: "bridgehead_N258183"
type: "bridgehead"
title: "Email Domains (DKIM) Preferences"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Company Settings > Setting Email Preferences > Email Domains (DKIM) Preferences"
parent: "section_4375043929"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N258183.html"
anchors: []
sha256: "932324cbafa31cf447c0799833f5371fdff04ee91d43714451afabcfee76ba80"
---

Users with the Administrator role can set up DomainKeys Identified Mail (DKIM) for the domains you want to send email from in NetSuite. Go to _Setup > Company > Email > Email Preferences_ and click the **Email Domains (DKIM)** subtab.

When you set up domain keys for your email domains, your DKIM headers are applied to outgoing email messages from your NetSuite account. This code header contains information to authenticate the email with the receiving server but doesn't add any text to your messages.

Note:

The procedure for setting up DKIM changed in the 2024.1 release.

| Column | Description |
| --- | --- |
| Domain Name | Enter the domain name you want to send email from, one domain per row. |
| Status | After you save the domain name, NetSuite displays its status: Pending Verification, Ready, or Requires Action. |
| Details | Review the messages displayed for informational or if you need to take more action. |

Enter your email domains in NetSuite and use the information generated in NetSuite to add DNS records at your domain provider's website to finish your DKIM setup.

For more information, see [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html) and [Procedures to Set Up DKIM in Your Production Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1536091217.html).

### Related Topics

-   [NetSuite Company Settings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N239909.html)
-   [General Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N256658.html)
-   [Transaction Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N256994.html)
-   [Email Template Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N257259.html)
-   [Sandbox and Release Preview Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4369903537.html)
-   [Email Spam Guidelines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504103104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
