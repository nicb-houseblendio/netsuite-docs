---
id: "section_N2638072"
type: "section"
title: "Setting Up a URL Redirect"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > SEO & Analytics > Search Engine Optimization (SEO) > SEO and Redirects > Setting Up a URL Redirect"
parent: "section_N2637891"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638072.html"
anchors: ["bridgehead_1493821118", "procedure_N2638089", "bridgehead_1492030207", "bridgehead_4303408253", "bridgehead_4819280118", "bridgehead_4819282247"]
sha256: "a7c8c122d29b8753207d67aab5dc96410ddcf69eca977c81f6565645c44abb36"
---

This section covers how to set up one URL redirect at a time.

You can set up redirects for any shopping domain you've added in NetSuite. First, select the domain, then enter the URL parameters you want to redirect from, and finally display in the URL for the right page. The domain and the URL you're redirecting from have to be different from the URL you're redirecting to.

Note:

If you use Site Builder, you must enable the Descriptive URLs feature. You cannot redirect from Site Builder URL parameters such as, **/s.nl/sc.26/category.321802/.f**. You must use a descriptive URL such as **/Product-Catalog/office-accessories**.

## Wildcards in URL Redirects {#bridgehead_1493821118}

If you need to redirect from a URL with parameters, you can use the wildcard to stand in for the parameters in the URL. For example, if you have the URL **http://mysite.com/womens/blouses?parameter1=a&parameter2=b**, you can create a redirect from **/womens/blouses\*** to **/womens/newcat/blouses**. When you use the wild card in the redirect, all parameters are passed to the redirect URL so that the final URL is **http://mysite.com/womens/newcat/blouses?parameter1=a&parameter2=b**.

Warning:

You cannot use a wildcard to redirect from one descriptive URL to another.

#### To set up a redirect: {#procedure_N2638089}

1.  Go to _Commerce > Hosting > Redirects > New_.
    
2.  Select a domain in the **Domain Name** field. The domains listed are the ones you set up at Setup > Website > Domains.
    
    Note:
    
    If you have set one of your custom domains as the Primary Web Site URL, then make sure you create a redirect with that domain, as well as other domains. For more information, read [Using the Primary Web Site URL in Redirects](#bridgehead_1492030207).
    
3.  In the **Redirect From URL** field, enter the URL that points to the page you want to redirect. Do not include the domain and instead use a relative URL.
    
4.  In the **Redirect To URL** field, enter the URL that points to the page where you want visitors to go. Here, you can enter any of the following:
    
    -   a relative URL that points to a page on your NetSuite site
        
    -   an absolute URL that points to a page on your NetSuite site
        
    -   a descriptive URL that points to a tab, category, or item detail page
        
    -   an absolute URL that points to another site
        
    
    For more information, read [Relative vs. Absolute URLs](#bridgehead_4303408253)
    
5.  Click **Save**.
    
    Note:
    
    Redirects go into effect immediately when you save them.
    

After you save the redirect record, you can visit the Redirects list page to see all the redirects set up for your web site.

## Using the Primary Web Site URL in Redirects {#bridgehead_1492030207}

If you use one of your custom domains as the Primary Web Site URL, you need to pick that domain when you create a redirect. For example, say your site has two custom domains: [www.mysite.com](http://www.mysite.com) (the Primary Web Site URL) and mysite.com (the secondary). To make the redirect work, you have to use [www.mysite.com](http://www.mysite.com). Choose [www.mysite.com](http://www.mysite.com) as the domain for a redirect that goes from /tshirt to /special-tshirt. If you set up the redirect on the secondary domain and go to mysite.com/tshirt, you'll first be redirected to [www.mysite.com/tshirt](http://www.mysite.com/tshirt), so the secondary redirect won't work.

## Relative vs. Absolute URLs {#bridgehead_4303408253}

When you create URL redirects, it's important to figure out if the URL should be relative or absolute. A relative URL uses the path to the page without the domain, for example /office-furniture. An absolute URL includes both the domain and the path, like mysite.com/office-furniture.

## When to use Relative URLs {#bridgehead_4819280118}

When you want to create a redirect from one page to another on the same domain, you can use a relative URL. Since you pick the domain on the Redirect page in NetSuite, you can use relative URLs for both the Redirect From and Redirect To fields. The redirect is created using the domain you selected.

![Redirect relative URL example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/SEOandAnalytics/RedirectPage_RelativeURL.png)

This is the method you should use when you retire a page on your site, restructure your site, or change the name of a page.

## When to use Absolute URLs {#bridgehead_4819282247}

When you move from one domain to another, it's important to use absolute URLs instead of relative URLs. Consider the following example:

Your domain has changed from **myoldsite.com** to **mynewsite.com**. You'll want to redirect traffic from myoldsite.com/office-furniture.html to mynewsite.com/office-furniture.html.

When you set up the redirect, you pick your old domain (in this case, myoldsite.com) as the domain. For the Redirect From URL, you enter the relative path from the old domain. For the Redirect To URL, you use the absolute path to the new domain page.

![Redirect absolute URL example](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/SEOandAnalytics/RedirectPage_AbsoluteURL.png)

Consequently, when a visitor goes to **myoldsite.com/office-furniture.html**, they are redirected to **mynewsite.com/office-furniture.html**.

### Related Topics

-   [Updating Redirect Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638305.html)
-   [Importing Website Redirects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638492.html)
-   [Delete Web Site Redirects Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2638981.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
