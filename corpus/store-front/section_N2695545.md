---
id: "section_N2695545"
type: "section"
title: "Customizing Item URLs for SEO"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > SEO & Analytics > Search Engine Optimization (SEO) > Customizing Item URLs for SEO"
parent: "chapter_4053877422"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2695545.html"
anchors: ["subsect_156580422456", "procedure_156580274379", "procedure_N2695590"]
sha256: "06fefb45d7b1e84f82dd9f6beb6a87fc338ca35348f80045521a9be870922ea2"
---

A well-defined item URL provides both shoppers and search engine web crawlers an indication of what the destination page will be about. In NetSuite, you can customize Commerce website URLs for items and facets. Website managers, administrators, and anyone with access to item records and facets can enter URL components and aliases. By default, the item URLs are displayed using URL Components defined on item records. If URL component is not defined for an item, the internal ID of the item is used. For example, you may see something similar to `www.mywebstore.com/product/361` as the URL for an item. To get the most out of SEO, it's better to use URL components, so you'll see URLs like `www.mywebstore.com/namebrandhelmet`.

URL Component Aliases are useful when you update URL components that point to items on your website, and you want to keep a list of the URL aliases that were used in the past. For more information, see [URL Component Aliases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4299068434.html).

## Use URL Components for Item URLs {#subsect_156580422456}

Here's what you should do to use URL Components for item URLs:

1.  Set URL Components on the items records.
    
2.  Add the **URL Component** field to the Search Field Set.
    

#### To set URL Component on an item record: {#procedure_156580274379}

1.  Go to Lists > Accounting > Items.
    
2.  Click **Edit** next to the desired item.
    
3.  Click the **Web Store** subtab.
    
4.  Under the Search Engine and Feeds section, enter the desired URL Component value in the **URL Component** field.
    
5.  Click **Save**.
    
    The URL Component field is now set for the item. To define URL Component Aliases for the item, see [URL Component Aliases](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4299068434.html).
    

#### To add the URL Component field to the Search Field Set: {#procedure_N2695590}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to the desired website.
    
3.  Click the **Field Sets** subtab.
    
4.  For the Search Field set, select **Fields Included in Field Set** details and click the **Set** icon in the lower right corner.
    
5.  In the **Field Set** popup window, select the **URL Component** field from the **Field Name** list and click **Add**.
    
6.  Click **Submit** and then **Done** on the Search field set line item.
    

### Related Topics

-   [SEO and Canonicalization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4411370568.html)
-   [SEO and Page Titles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4280885364.html)
-   [Structured Data Markup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_158032882820.html)
-   [SEO and Meta Descriptions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4285087960.html)
-   [SEO and Images](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4284172461.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
