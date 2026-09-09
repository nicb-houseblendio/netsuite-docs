---
id: "bridgehead_N2662753"
type: "bridgehead"
title: "Designate a Primary Domain"
branch: "system-management"
category: "commerce"
breadcrumb: "Commerce > System Management > Domains > Set Up Domains for Web Stores > Designate a Primary Domain"
parent: "section_N2484898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2662753.html"
anchors: ["bridgehead_N2662821", "bridgehead_N2662856", "bridgehead_4859021523"]
sha256: "c75f645acf3d41b6dc1234190bebfc9339e478929c45e65a4ab17828d9627dbf"
---

When you designate a Primary Web Site URL, any domain you set up in NetSuite will redirect to the one you marked as the Primary Web Site URL. The domain name marked as the Primary Web Site URL appears on your list of websites as the Primary Domain.

For example, you might set up two shopping domains such as **www.mystore.com** and **shop.mystore.com**. If you set www.mystore.com as the primary domain, then customers who type **shop.mystore.com/item** in their browser are redirected to the same page on the primary domain, **www.mystore.com/item**.

**Primary Domain Notes:**

-   If you have a secure Web Store Only domain, only that domain can be set as Primary.
    
-   If your site uses a Single Domain for Web Store and Checkout, only that domain can be set as Primary.
    
-   If your site uses multiple Single Domains for Web Store and Checkout, you can't set any domain as Primary.
    
-   All domain types available in NetSuite must be secured.
    

You can set a domain as your website's Primary Web Site URL from the Domains subtab on the Web Site Setup record.

Note:

Selecting a Primary Web Site URL is optional for Commerce web stores, but required for Site Builder.

## Sticky Domains {#bridgehead_N2662821}

In a Commerce web store, if you don't designate a primary domain, then each domain name persists as users move around your site. You can change the shopping experience for users by linking different domains to different SSP applications.

## Best Practice for Using Sticky Domains {#bridgehead_N2662856}

You can use an SSP application with multiple shopping domains in one Commerce web store. In this case, use the Touch Points subtab to link an SSP application with a touch point for the site. Next, use the Domains setup to link a domain with an SSP application.

## Touch Points {#bridgehead_4859021523}

Touch points defined on a domain override those set on the **Touch Points** subtab on the **Web Site Setup** page. However, you always need to define touch points on the Web Site Setup page, since domain-only touch point setup isn't supported. For information about using touch points, see [Link a Website or Domain to an SSP Application](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2495714.html).

### Related Topics

-   [Set Up a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1526632554.html)
-   [Convert a Web Store Only Domain to a Single Domain for Web Store and Checkout](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4837415242.html)
-   [Link a Checkout Domain with Your Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_157953243614.html)
-   [Point Your Domain Name at Your Domain (DNS Settings)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2479403.html)
-   [Troubleshoot Domain Setup Errors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1516105912.html)
-   [Delete a Domain](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158167571615.html)
-   [Set Up Domains for Web Stores](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2484898.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
