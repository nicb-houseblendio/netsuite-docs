---
id: "section_N2659294"
type: "section"
title: "Select and Configure Sort Fields"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Search > Search Settings Overview > Select and Configure Sort Fields"
parent: "section_N2656810"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659294.html"
anchors: ["procedure_N2659356"]
sha256: "5baa877586cb090f75200ad34dfc40f35bd594711176afc3cb75406510534108"
---

Using a sort field, shoppers can sort search results by that field instead of the default relevance field. It's not always clear which fields you should use for sorting, but make sure all your item records have data in the fields you pick-especially if those fields are optional. Items with empty fields show up last when you sort by that field. For example, if you sort by price, items with no price will be at the end.

Note:

Relevance is always the default sort field, and you can't remove it. But you can add other item fields as sorting options for your site. By default, the `onlinecustomerprice` field is already set up as a sort option, so you don't need to do any configuration to let shoppers sort by price. Commerce web stores are pre-configured to display two price sorting options: low to high and high to low.

When you add a Sort Field under Search Index, you turn on sorting for that field. You can use it with the Item Search API, but it only shows up in your web store after you configure it.

#### To add the sort fields: {#procedure_N2659356}

1.  Complete the prerequisite tasks as described in [Prerequisites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html#bridgehead_1499270591).
    
2.  Go to _Commerce > Websites > Website List_.
    
3.  Click **Edit** next to your SuiteCommerce Advanced site.
    
4.  Click the **Search Index** subtab and then **Sort Fields**.
    
    -   **Field Name** - (Required) Select an item record field. Choose the item attributes you want shoppers to use for sorting.
        
    -   **Field ID** - (View only field) Displays the field's internal ID.
        
    -   **Sort Order** - Choose ascending or descending order. This sets how products are sorted in the search results.
        

### Related Topics

-   [Select and Configure Facet Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657346.html)
-   [Configure Sort Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1201012018.html)
-   [Define Field Sets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659559.html)
-   [Search Settings Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html)
-   [Sorting Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530613879.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
