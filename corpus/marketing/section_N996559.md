---
id: "section_N996559"
type: "section"
title: "Campaign Email Domains"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Campaign Email Domains"
parent: "chapter_N992514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996559.html"
anchors: []
sha256: "dd463cb85a78332b04267dfb5da4b409840f17bad49328b8abfd471c4b94f46f"
---

To send more than 100,000 email messages through marketing campaigns in a 30 day period, you must set up a campaign domain. Similarly, to send more than 10,000 email messages in any single campaign event (blast), you must also set up a campaign domain.

See the following for more information about domains and your website:

-   [Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2478982.html)
    
-   [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html)
    
-   [Set Up Domains for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2484898.html)
    
-   [Campaign Email Limits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993465.html#bridgehead_N993205)
    

When you set up a campaign email domain, all links and other references to **netsuite.com** are instead replaced with your domain.

Important:

If you don't host your web store with NetSuite, you shouldn't use your web store or site domain as your email domain.

Note:

A campaign email domain is different from a DKIM. For information about DKIM, see [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html).

To make sure the links in your email work properly, your sender domain must match the domain in your links and tracking pixels return responses.

To set up a campaign email domain, configure Domain Name System (DNS) settings to point your email domain name to hosting servers at NetSuite. Your domain provider can redirect your email domain using a CNAME record (Canonical Name record). This makes your email domain an alias of the NetSuite hosting domain assigned to your account. NetSuite uses the CNAME (Alias) domain whenever a secure (HTTPS) connection is **not** required. For example, with website hosting and email campaigns.

#### To set up your email domain name in NetSuite:

1.  Go to _Commerce > Hosting > Domains_.
    
2.  In the **Domain Name** column, enter the domain name you have registered to send campaign email messages.
    
3.  In the **Hosted As** column, select **Email Campaign**.
    
4.  Click **Add**.
    
5.  Repeat these steps for each email domain you want to add.
    
6.  Click **Save**.
    
    Warning:
    
    After you create a new domain or update an existing domain, **you must wait two hours** before you configure DNS settings with your domain provider. See [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html).
    
7.  After two hours, return to the Domain Setup page, and then copy the **CNAME (Alias)** NetSuite assigned to you. You will use this CNAME to complete DNS setup with your domain name provider.
    
    Go to _Commerce > Hosting > Domains_.
    
    Note:
    
    Each time you add or edit a domain name in NetSuite, the CNAME (Alias) displayed for that domain changes. You must configure DNS settings with your domain provider to point your domain name to the correct CNAME (Alias).
    
8.  (Required) Visit your domain provider's website to complete the CNAME record setup. See [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html).
    
9.  Select the campaign domain on the **Marketing** subtab of your email template or campaign template records.
    
    You can set a default domain for your templates. Go to _Setup > Marketing > Preferences > Marketing Preferences (Administrator)_ > **Default Campaign Domain** field.
    

After you set up domain names in NetSuite, and configure DNS settings with your domain provider, your domains should begin redirecting. **The time frame for domain redirecting depends on your DNS provider. Generally, this process takes between two to 48 hours.**

In addition to email domains, you can also upload your own email domain keys to increase your delivery rates. For more information, see [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html).

### Related Topics

-   [Creating a Campaign Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986170.html)
-   [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html)
-   [DomainKeys Identified Mail (DKIM)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N999544.html)
-   [Marketing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1017620.html)
-   [Campaign Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N985787.html)
-   [Creating a Campaign Email Address Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1000747.html)
-   [Campaign Subscription Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996344.html)
-   [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
