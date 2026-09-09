---
id: "section_N2646187"
type: "section"
title: "Displaying an HTML Site Map on Your Website"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Using the Sitemap Generator in Site Builder > Displaying an HTML Site Map on Your Website"
parent: "section_N2645633"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646187.html"
anchors: ["procedure_N2646238", "procedure_N2646317"]
sha256: "d926e8b8294e76083e6d7fee57da81a49b3ea2eee8ecc017fc8758d494513a2e"
---

When you use the Sitemap Generator to create an HTML version of your site map, the file is placed in the hosting root folder you selected on the Sitemap Generator page. You can create a hosted tab on your website to display the HTML site map, or you can create a link to the HTML site map by adding an href on your website that targets the HTML file.

Note that the HTML version of your site map only shows the top three levels in the hierarchy of categories displayed on your site. For example, the HTML site map would show:

-   the parent category
    
    the first subcategory
    
    the second subcategory
    

Subcategories beyond the third level are not included in the HTML site map. URLs that point to all subcategories are included in the XML version of your site map.

#### To display an HTML site map on a website tab: {#procedure_N2646238}

1.  Go to _Commerce > Site Builder > Content Management > Tabs_.
    
2.  Click **New**.
    
3.  Click the **New Hosted** subtab.
    
4.  In the **Label** field, enter a name for the tab.
    
5.  In the **Web Site Page** list, select the HTML site map file from the hosting root folder in the file cabinet.
    
    After you choose a file in the **Web Site Page** list, the **Link URL** field automatically displays a relative URL for the file.
    
6.  Click **Save**.
    

Now you can click the new tab in your website to see the HTML page with links to each tab and category on your site.

#### To display a link to the HTML site map: {#procedure_N2646317}

1.  Go to the hosting root folder where your site map exists in the file cabinet, for example, Web Site Hosting Files > Live Hosting Files.
    
2.  Click **Edit** next to the HTML site map file.
    
3.  Use one of the URLs that begin with **http://** to create a hyperlink.
    
    For example, `<a href='http://www.wolfeelectronics.com/Sitemap.html'>View Sitemap</a>`
    

To display the link to the site map in the footer on every page of your website, paste the link in the Footer Template field of the site theme applied to your site, at _Commerce > Site Builder > Appearance > Themes_. For more information about site themes, see [Customizing Site Themes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2603752.html).

### Related Topics

-   [Generating a Site Map in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645823.html)
-   [Notifying Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646495.html)
-   [Assigning Site Map Priority and Excluding URLs from the Site Map](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646626.html)
-   [Using the Sitemap Generator in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645633.html)
-   [Keyword Marketing With Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639275.html)
-   [Working with Robots.txt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469279.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
