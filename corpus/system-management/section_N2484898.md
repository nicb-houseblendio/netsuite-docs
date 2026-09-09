---
id: "section_N2484898"
type: "section"
title: "Set Up Domains for Web Stores"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Set Up Domains for Web Stores"
parent: "chapter_N2478982"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2484898.html"
anchors: []
sha256: "d056f8df0c2b1ed17729a8e86f14b0f1bc8f06887fc99a9efaaad30260720115"
---

Before you start setting up domains for your online store, you need to know which types you want to use. The possibilities are:

-   **Single secure domain for both shopping and checkout** - follow the steps in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html) for the domain type **Single Domain for Web Store and Checkout**.
    
    This type of domain lets you run both shopping and checkout on one secure HTTPS domain. A single domain gives your customers a seamless buying experience.
    
    Note:
    
    The following requirements and limitations apply:
    
    -   If you're using SuiteCommerce MyAccount, set the Domain Type to **Single Domain for Webstore and Checkout**.
        
    -   You can't use Single Domain for Web Store and Checkout domains in Site Builder.
        
    
-   **Secure shopping domain combined with separate secure checkout domain**
    
    -   For the shopping domain, follow the steps in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html) for the domain type **Web Store Only**. Make sure you follow the steps in [Secure Your Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603043411.html) to secure the domain.
        
    -   For the secure checkout domain:
        
        -   If you want to use a preset checkout domain, this is set up automatically when you set up a Web Store Only domain.
            
        -   If you'd rather use a custom checkout domain, follow the steps in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html) for the domain type **Checkout Only**.
            
        
        To link a custom checkout domain or an unbranded NetSuite checkout subdomain with the secure shopping domain, follow the steps in [Link a Checkout Domain with Your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157953243614.html).
        

For more information about these domain types, see [Types of Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1521107777.html) and [Domain Options for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1521216758.html).

After you have set up the domains you need, you must [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html). Doing so makes it available to your customers.

To add to your web store, you can also set up the following types of domain as described in [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html).

-   **Hosted Web Page**\- Hosted web page domains aren't linked to a Web Site Setup record and don't offer web store features like checkout. However, you can use them for any static website, like a promotional site.
    
-   **Redirect URL**\- Redirect URL domains send visitors to a different website or page. See [SEO and Redirects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637891.html) for more information.
    
-   **Promotional URL**\- Promotional URL domains send visitors to a promotional URL you create at Setup > Other Setup > Promotional URLs > New. See [Promotional URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1016228.html) and for more information.
    
-   **Email Campaign Domain**\- Email campaign domains replace references to `netsuite.com` in your email and marketing templates with your own domain. You'll need this if you send more than 10,000 emails a month with campaigns or email merge operations. See [Website Domains and Email Hosting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4322255829.html) and for more information.
    

You'll need to set up all of these domains as secure. See [Secure Your Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0603043411.html).

After you've set up your domain, the Domain Health Status feature shows you if the setup has been done correctly and provides guidance on how to fix any errors. See [Troubleshoot Domain Setup Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1516105912.html) for details.

### Related Topics

-   [Convert a Web Store Only Domain to a Single Domain for Web Store and Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4837415242.html)
-   [Designate a Primary Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2662753.html)
-   [Delete a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158167571615.html)
-   [Introduction to Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1521794882.html)
-   [Advanced Domain Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1521812758.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
