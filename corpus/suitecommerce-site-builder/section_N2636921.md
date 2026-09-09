---
id: "section_N2636921"
type: "section"
title: "Using Canonical URLs in NetSuite Websites"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Using Canonical URLs in NetSuite Websites"
parent: "chapter_N2635817"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636921.html"
anchors: ["bridgehead_N2636963", "procedure_N2636988"]
sha256: "04f4c4da5818a6efbee422e47ef1c0bec415a8f310e514ccf9c982e7b37a9425"
---

NetSuite builds a canonical, or normalized, URL based on the preferred category you select for each item published online.

A canonical URL is useful in SEO because it creates a single preferred path to each item on your website, which eliminates the perception of duplicate content. Although an item may display in multiple categories or tabs, NetSuite uses the canonical URL to point to item pages in product feeds and site maps.

If you do not select a preferred category on the item record, NetSuite will determine the preferred category based on the most prominent category or tab on your site where the item is published.

To select a preferred category on an item record, check the box in the Preferred Category column on the Store subtab. For more information about displaying items online, see Setting Up Items for the Web Site .

## Canonical URLs and Custom Item/Category Templates {#bridgehead_N2636963}

The canonical URL tag exists in the <head> element of the NetSuite basic **item drilldown** and **category list** templates.

Note that you may need to add a canonical URL tag if you have already customized the NetSuite basic site templates.

#### To add a canonical URL to a customized Item/Category Template: {#procedure_N2636988}

1.  Go to _Commerce > Site Builder > Appearance > Item/Category Templates_.
    
2.  Click **Edit** next to the template you want to modify.
    
3.  In the **Addition to <head>** field, enter the following:
    
    -   For item drilldown templates:
        
        <link rel='canonical' href='<%=getCurrentAttribute('item','canonicalurl')%>'/>
        
    -   For category list templates:
        
        <link rel='canonical' href='<%=getCurrentAttribute('sitecategory','canonicalurl')%>'/>
        
4.  Click **Save**.
    

### Related Topics

-   [Adding Page Titles in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636435.html)
-   [Adding META Tags in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636604.html)
-   [Adding Alt Text to Website Images in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2636773.html)
-   [Descriptive URLs in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2637101.html)
-   [Keyword Marketing With Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639275.html)
-   [Using the Sitemap Generator in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645633.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
