---
id: "section_N2656810"
type: "section"
title: "Search Settings Overview"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Search > Search Settings Overview"
parent: "preface_1518478010"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html"
anchors: ["kaltura_player_219", "bridgehead_1499270591"]
sha256: "56abcd27f22553d55de97656e88111dd3aa2a70122abca3afadeba2ec8fa56a0"
---

<a id="kaltura_player_219"></a>

You can enhance the item search capabilities of your website by configuring the item search settings with your preferences. The following illustration shows how item search settings relate to your web store:

![Item Search Settings example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Commerce/StoreFront/Search/SearchSettingsOverview.png)

-   **Search Fields** influence the default sort order of the search results, which is relevance. For more information, see [Select and Configure Search Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657065.html).
    
-   **Facet Fields** help a shopper narrow down the search results. For more information, see [Select and Configure Facet Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657346.html).
    
-   **Sort Fields** define how results can be sorted beyond relevance to a search query. For more information, see [Select and Configure Sort Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659294.html).
    
-   **Field Sets** are a grouping of item fields taken from item records, used to display information to your shoppers. For more information, see [Define Field Sets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659559.html).
    

## Prerequisites {#bridgehead_1499270591}

Before you configure the item search settings, you should:

-   Complete [Item Availability](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656387.html), which includes setting up item records for display on your web store, setting up item records for search index, and setting up item inventory in web stores.
    
-   Review the [FieldSetsList](https://system.netsuite.com/core/media/media.nl?id=14901011&c=NLCORP&h=39759c97a3a915a0a132&_xt=.xls) spreadsheet, which lists all the fields that are available for keyword search, faceting, sorting, and for use in field sets.
    
    Note:
    
    When the Multiple Vendor feature is enabled, do not use the Preferred Vendor field (Field ID: vendor) as a sort field, facet field, or search field as it will not return any values.
    
-   Review the [Sample Search Field Configuration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1510159801.html).
    
-   Read the best practices to [Improve Relevance of your Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1499342355.html).
    
-   Identify the item record fields that contain keywords, which shoppers might use to search for products on your website.
    
    Important:
    
    For every website, the total number of fields included in the Field Sets, Sort Fields, and Facet Fields and should not exceed the limit of 1200.
    
-   Identify the item record fields shoppers might use to quickly narrow down search results.
    
-   Identify the item record fields shoppers might use to sort the search results.
    
-   Identify the item record fields you want to include in each field set.
    
-   Create any custom fields you want to add to field sets or use as search, facet, or sort fields.
    
    Important:
    
    If you use a custom item field in a field set or as a search field, facet field, or sort field, the custom item field gets locked and cannot be edited until unlocked.
    
    To unlock a custom item field, remove it from all field sets, search fields, facet fields, and sort fields on every Commerce website, then wait for the Search Index to rebuild.
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
