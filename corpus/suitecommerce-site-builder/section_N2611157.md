---
id: "section_N2611157"
type: "section"
title: "Website URL Parameters"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Customization > Website URL Parameters"
parent: "chapter_N2601007"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611157.html"
anchors: ["bridgehead_N2611291", "bridgehead_N2611312", "bridgehead_N2611392", "bridgehead_N2611462"]
sha256: "19d4abf8a1b4c8e745a5e393af521b55ac1497ea8291c0497db24212191a6edf"
---

This section describes the parameters exposed on your web store URLs and describes how web store managers and website designers can use these parameters to display specific pages in a NetSuite web store.

The following topics are discussed in this section:

-   [URL Parameters for Displaying Shopping Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2611580.html) - Describes how to display search results as well as specific tab, category, and item pages, on your web store.
    
-   [URL Parameters for Adding Items to the Cart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2612472.html) - Includes information about how to construct a URL for adding items to the shopping cart in a OneWorld account.
    
-   [URL Parameters for Passing Marketing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2613194.html) - Describes how to construct URLs for tracking partners and for use in marketing your web store.
    
-   [URL Parameters for Setting Values in Your OneWorld Web Store](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2614795.html) - Describes URL parameters for use with a OneWorld web store.
    
-   [URL Parameters for Setting the Currency on your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2615184.html) - Identifies the URL parameters you can use to set the currency for prices displayed on a page of your web store.
    

## Anatomy of a Website Shopping URL {#bridgehead_N2611291}

Before you can start working with URL parameters, it is important to understand how NetSuite web store URLs are formed. Whether you use the NetSuite shopping domain (shopping.netsuite.com) or your own domain, understanding how to add parameters to your website URLs gives you more options for customization. For more information about domains, see [Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2478982.html).

## Forming the Base Domain of a URL {#bridgehead_N2611312}

The base domain of a NetSuite web store consists of the following variables: the domain for your website, your NetSuite account number (if you use the NetSuite shopping domain), and variables indicating which website page to display, such as internal IDs for item and category records.

Note:

The NetSuite shopping domain used to construct the base domain for your site varies according to the host data center for your NetSuite account. You can always find the shopping domain for your site on the Domains list page or on the Domains subtab on the Web Site Setup page.

You may notice that NetSuite shopping URLs appear in two different formats:

-   http://shop.netsuite.com/s.nl/c.123456/id.12/.f?category=123
    
-   http://shop.netsuite.com/s.nl?c=123456&id=12&category=123
    

The first format above is more favorable for SEO. However, when you are constructing a URL for a process, such as adding an item to the shopping cart, both formats work equally well. Note that custom domains also appear in both formats:

-   http://www.wolfeelectronics.com/s.nl/id.12/.f?category=123
    
-   http://www.wolfeelectronics.com/s.nl?id=12&category=123
    
    Important:
    
    If you use your own custom domain, you should never use the NetSuite shopping domain to construct URL parameters for your website.
    

Alternating between the NetSuite shopping domain (shopping.netsuite.com), and your own custom domain (www.mysite.com) can cause cookie and session information to get lost as visitors click through the pages of your site.

## Required Web Site URL Parameters {#bridgehead_N2611392}

If you use the NetSuite shopping domain, the `c` parameter is required to identify your NetSuite account. The `n` parameter, which identifies the internal ID for the site, is also required. For example, the URL below points to a tab on site 3 `(n.3)` in NetSuite account number 123456.

`http://shop.netsuite.com/s.nl/c.123456/n.3/sc.13/.f`

If you use custom domains for your web stores, however, the `c` and **n** parameters are not required because your custom domain is mapped to the correct NetSuite account and website at the database level. The URL below uses a custom domain to show the same page as the URL above.

`http://www.wolfeelectronics.com/s.nl/sc.13/.f`

All website URLs from your NetSuite account use `/s.nl/` in the path to indicate an e-commerce page request. Note that URLs which contain `/.f?` before additional parameters are more favorable for SEO.

## Adding Parameters to a URL {#bridgehead_N2611462}

In addition to identifying the domain and the website page, the URL includes parameters which can be used in a query string.

By adding a query string to the URL of a NetSuite web page, you can display specific information on the page. A query string contains name and value pairs, with the name and value in each pair separated by an equal sign (=).

For example, when a shopper clicks on one of the URLs below, they are taken to a web store tab presenting a list of results for the search term, 'electronics.' Note that the first example uses the NetSuite shopping domain and identifies the NetSuite account number (c.123456).

-   http://shop.netsuite.com/s.nl/c.123456/sc.2/.f?search=electronics
    
-   http://www.wolfeelectronics.com/s.nl/sc.2/.f?search=electronics
    

The tab's internal ID is defined in the sc parameter. You can find the internal ID for any record in NetSuite in the address bar of your browser when you go to that record. For more information, see [Finding Internal IDs of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0416030736.html)

The first parameter (in this case 'search=electronics') ialways comes after a question mark (?), and subsequent parameters are added with ampersands (&). The URLs below display items 1 through 5 in a list of 10 search results for 'electronics.'

-   http://shop.netsuite.com/s.nl/c.123456/sc.2/.f?search=electronics&range=1,5,10
    
-   http://www.wolfeelectronics.com/s.nl/sc.2/.f?search=electronics&range=1,5,10
    

### Related Topics

-   [Basic Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2602412.html)
-   [Advanced Site Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603624.html)
-   [Site Builder Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2601007.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
