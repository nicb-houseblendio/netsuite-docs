---
id: "section_N2646626"
type: "section"
title: "Assigning Site Map Priority and Excluding URLs from the Site Map"
branch: "suitecommerce-site-builder"
category: "commerce"
breadcrumb: "Commerce > SuiteCommerce Site Builder > Site Builder Search Engine Optimization (SEO) > Using the Sitemap Generator in Site Builder > Assigning Site Map Priority and Excluding URLs from the Site Map"
parent: "section_N2645633"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646626.html"
anchors: ["bridgehead_N2646638", "bridgehead_N2646674"]
sha256: "40d1e81a25fbab0059eddefe7739124c5fcd5d84f29f3ed459572ebdc64391d5"
---

You can define the relative importance of each URL in your website as compared to other URLs in your site. In this way you can guide search engine web crawlers to the most important pages as they index your site. Alternatively, you can exclude certain URLs from your site map, when those pages are under construction.

## Excluding Certain URLs from the Site Map {#bridgehead_N2646638}

You might want to exclude a tab, category, or item page from the site map while you are finalizing the layout. You can do this by checking the **Exclude from Sitemap** box. This checkbox helps with with mass update and saved search, so you can update several records at the same time.

## Assigning Priority to Certain URLs {#bridgehead_N2646674}

Use the **Sitemap Priority** list to indicate the relative importance of your website URLs. You can select a priority ranging from 0.0 to 1.0 on item, category, and tab records.

NetSuite assigns a default priority 'Auto' to all new and existing tab, category and item records in your account. The Sitemap Generator translates the default priority into a number for the priority attribute when you generate your site map. The priority is calculated based on the position of the item or category in the hierarchy of your website.

For example, your website tabs automatically generate a default priority value of 1.0 because they are top level pages. A category published to a tab gets a priority of 0.5. An item published to a category on a tab gets a priority of 0.3.

You can select a different value in the Sitemap Priority list to override the default 'Auto' priority. NetSuite uses the value you set when you generate the site map. Sitemap Priority is also available to use with mass update and saved search, so you can change the value on several records at the same time.

Assigning a high priority to all of the URLs on your site is not likely to affect the ranking of your site in a search engine's result pages. Search engines may use the priority you set when indexing URLs as they crawl your site. Set a Sitemap Priority to increase the probability that your most important pages are indexed.

### Related Topics

-   [Generating a Site Map in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645823.html)
-   [Displaying an HTML Site Map on Your Website](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646187.html)
-   [Notifying Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2646495.html)
-   [Using the Sitemap Generator in Site Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2645633.html)
-   [Keyword Marketing With Search Engines](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2639275.html)
-   [Working with Robots.txt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2469279.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
