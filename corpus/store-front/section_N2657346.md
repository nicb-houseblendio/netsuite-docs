---
id: "section_N2657346"
type: "section"
title: "Select and Configure Facet Fields"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Search > Search Settings Overview > Select and Configure Facet Fields"
parent: "section_N2656810"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657346.html"
anchors: ["procedure_1499333743"]
sha256: "787f6bae418385adf3b03f6cf2370116d7aff629e418a94269632f6bf007ec79"
---

Facets let you filter the search results by the values in item fields. When a shopper clicks a facet value, the results show only items with that value. Each extra click keeps narrowing down the search results. Commerce web stores and SCIS use modern faceted navigation for displaying item results.

Usually, you'll use different item attributes as facets. For example, popular facet fields for an apparel website are brand, gender, color, and size.

When you add a Facet Field under Search Index, you turn on faceting for that field. You can then use this facet field with the Item Search API.

Note:

Don't add too many Facets or Facet Values, since it can slow down search. Try to use 40 facets or fewer.

#### To select the facets: {#procedure_1499333743}

1.  Complete the prerequisite tasks as described in [Prerequisites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html#bridgehead_1499270591).
    
2.  Go to _Commerce > Websites > Website List_.
    
3.  Click **Edit** next to your SuiteCommerce Advanced site.
    
4.  Click the **Search Index** sub tab and then **Facet Fields**.
    
5.  From the **Facet Field Name** dropdown, pick the fields you want to use as facets and click **Add**.
    
6.  (Optional) To delete a Facet Field, select the field and click **Remove**.
    
7.  After you have finalized the Facet Fields, click **Save**.
    

After you select the facet fields, you can configure the facet fields for your site using the SuiteCommerce Configuration record. For more details, see [Configure Facet Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156587819021.html).

### Related Topics

-   [Select and Configure Search Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657065.html)
-   [Select and Configure Sort Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659294.html)
-   [Search Settings Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html)
-   [Define Field Sets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659559.html)
-   [Facets as Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1485881926.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
