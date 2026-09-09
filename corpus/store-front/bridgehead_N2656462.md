---
id: "bridgehead_N2656462"
type: "bridgehead"
title: "Search Index Settings"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Web Store Items > Item Availability > Search Index Settings"
parent: "section_N2656387"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2656462.html"
anchors: ["procedure_N2656479", "bridgehead_1501081221", "procedure_1519662254", "procedure_1519662268"]
sha256: "65bd2984bfecfc3e37775ddfe62446edf6dd4d92c32eacb795dd6803271bf61b"
---

Search Index plays a key role in displaying items in Commerce web stores and in SCIS. Items published to your web store are first indexed, and after the search index process is complete, data on the item records can be queried using the Item Search API.

When setting up item records for the Search Index, you might need to create custom fields beyond the standard ones. For example, price and brand are two common facets used on commerce sites. In NetSuite, price is a standard field on item records. Brand would be a custom field that you'll need to create. Include both fields in your field sets to display price and brand information in your Commerce web store and in SCIS. For more information, see [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html).

#### To set up item records for the search index: {#procedure_N2656479}

1.  Go to Lists > Website > Items.
    
2.  Determine the standard fields you want to use as search fields, facet fields, and sort fields.
    
    Note:
    
    You can use a combination of standard and custom item record fields for search fields, facet fields, sort fields, and field sets on your website. Note that only certain field types are supported for these purposes. For more information, see [Field Set Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659559.html#bridgehead_1500648146).
    
3.  Determine the fields on the item record that you need to create field sets for.
    
    For example, for SEO, you can use descriptive URL components in an item template. To do this, enter a value in the **URL Component** field and include the **URL Component** field in a field set.
    
4.  Make sure you have data in all the fields you'll be accessing through the Item Search API.
    
    For information about supported API parameters, see [Item Search API Input Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665676.html).
    
    Note:
    
    Ensure that data is also populated for Matrix Child items.
    
5.  Create custom fields for use as search fields, facet fields, sort fields, and field sets.
    
    For instance, create a custom field called Brand.
    
6.  Enter data in the custom fields you created. For instance, if you created the custom field Brand, enter the value for brand on each item record for display on your site.
    
7.  Check the **Display in Website** box on the item record.
    
8.  Clear the **Inactive** box, as inactive items aren't included in the search index.
    
9.  You can index all item records using the **Show Uncategorized Items** option, or you can individually select the item records you want indexed. For more information, see [Including Item Records in the Search Index](#bridgehead_1501081221).
    

## Including Item Records in the Search Index {#bridgehead_1501081221}

For an item to be included in the Search Index, the following conditions must be met:

-   The **Display in Web Site** box must be checked on the item record.
    
-   The item must be active, so the Inactive box should be cleared on the item record.
    
-   Either check the **Show Uncategorized Items** box on the Web Site Setup page or assign the item to a Site Builder or Commerce Category.
    

Checking the **Show Uncategorized Items** box indexes all active items with the **Display in Website** box checked. This option allows items to appear in search results even if they're not in a category. However, this option might not be suitable for all scenarios. For instance, you might want to display only selected items when you have multiple sites with different item sets.

Alternately, you can clear the **Show Uncategorized Items** option, and configure the item records individually. In this case, only item records assigned to a Site Builder or Commerce Category are indexed. Add each item to a category on the site where you want it to appear. You can do this on the item record, or use the content manager.

Note:

Changing the Show Uncategorized Items setting and saving the Web Site Setup record triggers the Search Index Rebuild process. You'll be redirected to the Job Status page, which displays the Search Index process.

#### To index all the item records: {#procedure_1519662254}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to your SuiteCommerce Advanced site.
    
3.  On the **Setup** subtab, check the **Show Uncategorized Items** box.
    
4.  Click **Save**.
    

#### To index individual item records: {#procedure_1519662268}

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click **Edit** next to your SuiteCommerce Advanced site.
    
3.  On the **Setup** subtab, clear the **Show Uncategorized Items** box.
    
4.  Click **Save**.
    
5.  Go to Lists > Accounting > Items.
    
6.  Click **Edit** next to an item record.
    
7.  On the **Web Store** subtab, select a **Site** and **Site Category** for this item.
    
8.  Click **Save**.
    
9.  Repeat Steps 6 through 8 for each item record you want to index.
    

### Related Topics

-   [Item Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656387.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
