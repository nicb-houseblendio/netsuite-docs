---
id: "section_N2645823"
type: "section"
title: "Generating a Site Map in Site Builder"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Using the Sitemap Generator in Site Builder > Generating a Site Map in Site Builder"
parent: "section_N2645633"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645823.html"
anchors: ["procedure_N2645836", "bridgehead_N2646082"]
sha256: "7c9abfbdce3a8b7dcb941ccc406b376622beaadd6c731610dffaf9a429f7f048"
---

For Site Builder, the Sitemap Generator can create a site map in XML and HTML file formats. After the site map is generated, it is placed in the Web Site Hosting Files folder that you designate. If your website has more than 50,000 URLs, multiple site map files are created with an index file that points to each of them.

#### To generate a site map: {#procedure_N2645836}

1.  Go to _Commerce > Site Builder > Marketing/Upsell > Sitemap Crawler_.
    
2.  Select the site in the **Web Site** field.
    
3.  In the **Destination Folder** list, select a folder to hold your site map.
    
    This list only includes subfolders of the Web Site Hosting Files folder. Place the site map in the root folder (highest level folder) of your website. By default, the root folder of a NetSuite website is **Web Site Hosting Files : Live Hosting Files**.
    
    If you have multiple websites, the site map for each website belongs in each site's root folder.
    
4.  In the **File Name** field, enter a name for your site map file.
    
5.  In the **Index File Name** field, enter the name for your site map index file.
    
6.  Choose a file format for your site map or check both boxes to generate the site map in both XML and HTML format at the same time.
    
    -   **XML Format** - Generates a site map in XML format to submit to search engines.
        
    -   **HTML Format** - Generates a site map in HTML format for hosting on your website. Note that only links to tabs and categories are included.
        
7.  Check the box, **Include Hosted Pages** to include HTML pages displayed on your site:
    
    -   The XML site map includes all hosted pages, tabs, and categories you display on your website.
        
    -   The HTML site map includes your hosted home page, hosted tabs, presentation tabs, and categories displayed on your website.
        
8.  Use the **Number of Columns in HTML Format** field to designate how many columns you want to display in the HTML version of the site map for display on your website.
    
9.  In the XML Options section, select the appropriate attributes for your XML site map.
    
    -   **Change Frequency** - Sets the attribute in the <changefreq> tag which defines how often you change your website pages. Search engines scan for this information when they index your site.
        
        Note:
        
        You must click Submit on the Site Generator page to update your site map.
        
    -   **Last Modified** - Sets the attribute in the <lastmod> tag which defines, for search engines, the date each page most recently changed.
        
        Note:
        
        The Last Modified Date attribute defines the most recent date that a change occurred on a page. This value includes changes to items and categories on a page.
        
    -   **Priority** - Sets the attribute in the <priority> tag which defines the relative importance of each page as compared to other pages of your site. You can select a priority ranging from 0.0 to 1.0 on item, category, and tab records. For more information, see [Assigning Priority to Certain URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646626.html#bridgehead_N2646674).
        
10.  In the **Email Address** field, enter the email address where you want to be notified after the generator completes.
     
11.  Click **Submit**.
     

The Sitemap Generator sends an email message after your site map files are created. The message contains a list of the site map files that were generated and indicates where they are located in your file cabinet.

Also included in the email message are the links you must click to notify search engines that your site map has changed. Note that Google, Bing, and Yahoo! require that you register with them before they accept updates to your site map. For more information, see [Notifying Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646495.html).

## Customizing Your Site Map {#bridgehead_N2646082}

Note that after your site map files appear in the file cabinet, you can modify them. For example, you might want to customize the HTML site map so the look and feel is consistent with the rest of your website.

To edit a site map file, download the file on to your computer, and use your favorite XML or HTML file editing application to modify the file. When you are finished, click Add File in the hosting root folder of the file cabinet to replace the original site map file.

Note:

For more customization options, you can use Web site attribute tags in the HEAD element of site map files in HTML format. You can use any attribute from the item or site category record. Use the syntax in the example below: `<%=getCurrentAttribute('item','canonicalurl')=%>`

### Related Topics

-   [Displaying an HTML Site Map on Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646187.html)
-   [Notifying Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646495.html)
-   [Assigning Site Map Priority and Excluding URLs from the Site Map](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646626.html)
-   [Using the Sitemap Generator in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645633.html)
-   [Keyword Marketing With Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639275.html)
-   [Working with Robots.txt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469279.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
