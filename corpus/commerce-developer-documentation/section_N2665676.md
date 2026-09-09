---
id: "section_N2665676"
type: "section"
title: "Item Search API Input Parameters"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Item Search API > Item Search API Input Parameters"
parent: "chapter_N2665337"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665676.html"
anchors: ["bridgehead_4073492701", "bridgehead_N2666855", "bridgehead_N2667034", "bridgehead_N2666960", "bridgehead_4696127814", "bridgehead_1562859548", "bridgehead_N2666814", "bridgehead_4810205269", "bridgehead_N2666927", "bridgehead_4139347112", "bridgehead_N2666872", "bridgehead_N2667008", "bridgehead_4077931895", "bridgehead_N2666712", "bridgehead_N2666692", "bridgehead_N2666671", "bridgehead_N2666732"]
sha256: "8549f56f63bff622af2f338a1d29cd9c5c0b838ce86299fdb93f86b1bb180c0b"
---

The Item Search API Input Parameters are used to construct query strings that return item record attributes in a JSON response. To create a query string for the Item Search API, you should use the input parameters with the base URL `http://www.mywebstore.com/api/items?{parameters}`. You can also use multiple parameters with the base URL by separating them with an ampersand (`&`).

Note:

Some parameters, when used with the base URL, return the item IDs of the matching items. However, if you want to retrieve additional item details, you can use the parameters listed under the Retrieve Additional Item Details section with these parameters.

The base URL when used without any parameters retrieves the item IDs of all the items. To retrieve only the desired items and item details, you can specify the following input parameters:

| Parameters | Usage |
| --- | --- |
| `c` `n` `region` | [Retrieve Items by NetSuite Account Number, Commerce Site ID, Subsidiary ID](#bridgehead_4073492701) |
| `id` | [Retrieve Items by Item ID](#bridgehead_N2666855) |
| `url` | [Retrieve Items by Item URL](#bridgehead_N2667034) |
| `q` | [Retrieve Items by Keyword Search](#bridgehead_N2666960) |
| `commercecategoryid` `commercecategoryurl` `commercecategoryname` | [Retrieve Items by Commerce Categories](#bridgehead_4696127814) |
| `use_pcv` `pcv_entity` `pcv_groups` | [Retrieve Items from Personalized Catalog for a specific customer or one or more customer groups](#bridgehead_1562859548) |
| `fields` `fieldset` | [Retrieve Additional Item Details](#bridgehead_N2666814) |
| `matrixchilditems_fieldset` `correlateditems_fieldset` `relateditems_fieldset` | [Flexibility in Specifying the Field Sets of Related Items](#bridgehead_4810205269) |
| `limit` `offset` | [Pagination of Query Results](#bridgehead_N2666927) |
| `<field_name>` `<numeric_facet_field_ID>.ranges` `<numeric_facet_field_ID>.from` `<numeric_facet_field_ID>.to` | [Facet and Filter Items](#bridgehead_4139347112) |
| `include` `facet.exclude` | [Include or Exclude Item Attributes](#bridgehead_N2666872) |
| `sort` | [Sort Items](#bridgehead_N2667008) |
| `pricelevel` | [Specify Price Level](#bridgehead_4077931895) |
| `currency` | [Specify Currency](#bridgehead_N2666712) |
| `language` `country` | [Specify Language and Country](#bridgehead_N2666692) |
| `callback` | [Callback Function](#bridgehead_N2666671) |
| `ssdebug` | [Retrieve Debug Information](#bridgehead_N2666732) |

## Retrieve Items by NetSuite Account Number, Commerce Site ID, Subsidiary ID {#bridgehead_4073492701}

-   `c` - You can use the parameter `c` to specify the NetSuite account and retrieve all the items in the specified NetSuite account. For example, if your NetSuite account is 3925062, you can use the following query string to retrieve all the items that belongs to your NetSuite account:
    
    `http://www.mywebstore.com/api/items?c=3925062`
    
-   `n` - You can use the parameter `n` to specify the ID of your Commerce web store and retrieve all the items in the specified Commerce web store. For example, if the ID of your Commerce web store is 3, you can use the following query string to retrieve all the items that belongs to this Commerce web store:
    
    `http://www.mywebstore.com/api/items?n=3`
    
-   `region` - You can use the parameter `region` to specify the Subsidiary in a NetSuite OneWorld account and retrieve all the items in the specified Subsidiary. For example, if your Subsidiary ID is 4, you can use the following query string to retrieve all the items that belongs to this Subsidiary:
    
    `http://www.mywebstore.com/api/items?region=4`
    

You can also use these parameters together to further refine the search results. For example, if have more than one Commerce web store in a NetSuite account and you would like to retrieve items belonging to a particular site, you can use the following query string:

`http://www.mywebstore.com/api/items?c=3925062&n=3`

Note:

If you specify an incorrect NetSuite account number, an incorrect Commerce Site ID, an incorrect or inactive Subsidiary ID, or if your website is not reachable, no items are returned and an error message is displayed.

## Retrieve Items by Item ID {#bridgehead_N2666855}

You can use the parameter `id` to specify the item record ID and retrieve information for a particular item. For example, you can use the following query string to retrieve the item with Item ID 123:

`http://www.mywebstore.com/api/items?id=123`

To return multiple items in response data, list multiple item IDs separated by commas. For example, you can use the following query string to retrieve the items with Item ID 123, 456, 789:

`http://www.mywebstore.com/api/items?id=123,456,789`

Note:

If the item is marked as Inactive or if the Display in Web Store box is not selected on the item record, no items are returned. If you specify an invalid item ID, an error message is displayed. In case of Matrix items, active child items are returned only if the parent item is active and the Display in Web Store box is selected.

## Retrieve Items by Item URL {#bridgehead_N2667034}

You can use the parameter `url` to specify the value in the URL Component field on the item record. The url parameter returns the Item ID of item that matches the URL component value in the request.

`http://www.mywebstore.com/api/items?url=Vok-500-Cellular-Phone`

You can specify other parameters along with the `url` parameter to retrieve other item details. For example, you can use the `fields` parameter to retrieve associated images:

`http://www.mywebstore.com/api/items?url=Vok-500-Cellular-Phone&fields=itemimages_detail`

You can also use a field set that contains image information:

`http://www.mywebstore.com/api/items?url=Vok-500-Cellular-Phone&fieldset=details`

Note:

If the item is marked as Inactive or if the Display in Web Store box is not selected on the item record, no items are returned. If you specify an invalid item URL, an error message is displayed. In case of Matrix items, active child items are returned only if the parent item is active and the Display in Web Store box is selected.

## Retrieve Items by Keyword Search {#bridgehead_N2666960}

You can use the parameter `q` to retrieve all the items that match the specified keyword. For example, `q=jeans` searches for that keyword in the fields listed on the Search Fields subtab.

`http://www.mywebstore.com/api/items?q=jeans`

Note:

Matching items are returned only if the specified keyword exists in the search fields that you selected on the Web Site Setup page. For information about selecting Search Fields, see [Select and Configure Search Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2657065.html).

To do a multi-term search, specify two or more terms in the URL separated by whitespace. For example, `q=denim jeans` searches for these keywords in the fields listed on the Search Fields subtab.

`http://www.mywebstore.com/api/items?q=denim jeans`

Note:

Relevance is the default sort order when you use the q parameter to query the Item Search API. Your preferred sort order specified on the Sort Fields subtab is overridden. For information about selecting and configuring Sort Fields, see Select and Configure Sort Fields.

## Retrieve Items by Commerce Categories {#bridgehead_4696127814}

-   `commercecategoryid` - You can use the parameter `commercecategoryid` to retrieve items that belong the specified Commerce Category ID.
    
    `http://www.mywebstore.com/api/items?commercecategoryid=12345`
    
-   `commercecategoryurl` - You can use the parameter `commercecategoryurl` to retrieve items that belong the specified Commerce Category URL.
    
    `http://www.mywebstore.com/api/items?commercecategoryurl=/apparel/partywear/shoes`
    
-   `commercecategoryname` - You can use the parameter `commercecategoryname` to retrieve items that belong the specified Commerce Category.
    
    `http://www.mywebstore.com/api/items?commercecategoryname=Summer Sale`
    
    This parameter is dependent on the Commerce Category facet field being defined in the Web Site Setup record. For more information, see [Add Commerce Categories to Website Search Index](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4696324780.html).
    

Note:

For a sample search query and response on Commerce Categories, see [Sample Search Query for Returning Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2667130.html#bridgehead_4696130354).

## Retrieve Items from Personalized Catalog for a specific customer or one or more customer groups {#bridgehead_1562859548}

Important:

To be able to use the `pcv_entity` and `pcv_groups` parameters, the user must have a valid NetSuite user account and be assigned a role that provides edit website or list items permissions. For more information, see [Personalized Catalog Views Roles and Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1560331283.html). Note that these parameters are intended for administrative interfaces only and not for building web pages that display a personalized catalog.

-   `use_pcv` - For the Personalized Catalog Views feature to take effect while retrieving items, you must use the `use_pcv` parameter with the Item Search API. When the `use_pcv` parameter is set to true, the Item Search API returns tailored selection of catalog items from the user's customer groups. The Item Search API query without the `use_pcv` parameter has the same effect as `use_pcv=F`. Therefore, when the `use_pcv` parameter is set to false, the Item Search API serves items for anonymous users regardless of whether the user is logged in or recognized.
    
    For example, a NetSuite user with sufficient permissions for PCV posts the following query:
    
    `http://www.mywebstore.com/api/items?use_pcv=T`
    
    The Item Search API lists all the items but only shows the items which should be visible for this user.
    
    Note:
    
    By default, the Item Search API response data has a volatility of Short or Medium. Volatility refers to the CDN cache settings for your Commerce implementation. If the `use_pcv` parameter is set to true, the Item Search API always serves non-cacheable responses, which is evident in the Item Search API response where volatility=unique. The Item Search API query without the `use_pcv` parameter has the same effect as `use_pcv=F`. Therefore, if the `use_pcv` parameter is set to false, the Item Search API uses the existing caching behavior.
    
-   `pcv_entity` - You can use the `pcv_entity` parameter to specify a single entity ID to be used as the basis for customer groups to apply query filtering. For the `pcv_entity` parameter to take effect while retrieving items, you must also specify `use_pcv=T` with the `pcv_entity` parameter.
    
    For example, let's consider there are items on the site assigned to these four customer groups: ALL\_USERS, GUEST\_USERS, RECOGNIZED\_USERS and VIP\_USERS. Items assigned to the VIP\_USERS customer group are exclusive items and are not available for customers in other customer groups. There is a customer, say CUSTOMER1, with Customer ID 111 who belongs to the VIP\_USERS customer group. A NetSuite user with sufficient permissions for PCV posts the following query:
    
    `http://www.mywebstore.com/api/items?use_pcv=T&pcv_entity=111`
    
    The Item Search API returns all the items available for customer with customer ID 111 in the response, which includes items from ALL\_USERS, RECOGNIZED\_USERS and VIP\_USERS customer group.
    
    Note:
    
    If you specify an invalid entity ID (for example, a string) or an incorrect entity ID (for example, a valid number but a non-existent entity ID) with the `pcv_entity` parameter, no items are returned in the Item Search API response. If you specify more than one entity ID with the `pcv_entity` parameter, an error message is displayed.
    
-   `pcv_groups` - You can use the `pcv_groups` parameter to specify one or more customer group IDs to apply query filtering. For the `pcv_groups` parameter to take effect while retrieving items, you must also specify `use_pcv=T` with the `pcv_groups` parameter.
    
    For example, let's consider there are items on the site assigned to these three customer groups: ALL\_USERS (Customer Group ID= 1), GUEST\_USERS (Customer Group ID= 2) , RECOGNIZED\_USERS (Customer Group ID= 3). A NetSuite user with sufficient permissions for PCV posts the following query:
    
    `http://www.mywebstore.com/api/items?use_pcv=T&pcv_groups=3`
    
    The Item Search API returns all the items assigned to the group RECOGNIZED\_USERS.
    
    Note:
    
    If you specify an invalid group ID (for example, a string) or an incorrect group ID (for example, a valid number but a non-existent group ID) with the `pcv_groups` parameter, no items are returned in the Item Search API response. If you specify two group IDs with the `pcv_groups` parameter with one existing group ID and one non-existent group ID, only the items for the existing group are returned in Item Search API response.
    

## Retrieve Additional Item Details {#bridgehead_N2666814}

If you do not specify any input parameters with the Item Search API base URL, only the Item IDs of the items are returned. You can use the following parameters to retrieve additional item details:

-   `fields` - You can use the parameter `fields` to retrieve additional item record fields in the API response. Your request can include a valid field ID, or multiple field IDs separated by commas to return multiple fields.
    
    `http://www.mywebstore.com/api/items?fields=custitem1,upccode`
    
-   `fieldset` - You can use the parameter `fieldset` to retrieve all the item fields associated with a field set.
    
    `http://www.mywebstore.com/api/items?fieldset=details`
    

Note:

When the Commerce Category field is defined in the Web Site Setup record field sets, the Commerce Category details for a given item are returned.

## Flexibility in Specifying the Field Sets of Related Items {#bridgehead_4810205269}

-   `matrixchilditems_fieldset` - You can use the parameter `matrixchilditems_fieldset` to specify the field set that overrides the reserved `matrixchilditems` field set. The `matrixchilditems` field set is used by the `matrixchilditems_detail` derived field by default to retrieve the item fields of all the matrix child items. In the following example, the default `matrixchilditems` field set is overridden with a field set named `mini` using the Item Search API parameter `matrixchilditems_fieldset`.
    
    `http://www.mywebstore.com/api/items?fieldset=search&matrixchilditems_fieldset=mini`
    
-   `correlateditems_fieldset` - You can use the parameter `correlateditems_fieldset` to specify the field set that overrides the reserved `correlateditems` field set. The `correlateditems` field set is used by the `correlateditems_detail` derived field by default to retrieve the item fields of all the correlated items. In the following example, the default `correlateditems` field set is overridden with a field set named `mini` using the Item Search API parameter `correlateditems_fieldset`.
    
    `http://www.mywebstore.com/api/items?fieldset=search&correlateditems_fieldset=mini`
    
-   `relateditems_fieldset` - You can use the parameter `relateditems_fieldset` to specify the field set that overrides the reserved `relateditems` field set. The `relateditems` field set is used by the `relateditems_detail` derived field by default to retrieve the item fields of all the related items. In the following example, the default `relateditems` field set is overridden with a field set named `mini` using the Item Search API parameter `relateditems_fieldset`.
    
    `http://www.mywebstore.com/api/items?fieldset=search&relateditems_fieldset=mini`
    

## Pagination of Query Results {#bridgehead_N2666927}

You can use the parameter `offset` in combination with another parameter `limit` to paginate Item Search API query results. The `offset` parameter specifies the offset from the first result and the `limit` parameter specifies the number of items that can be displayed on each page. For example, you can retrieve query results from the eleventh item to the fifteenth item using the following query string:

`http://www.mywebstore.com/api/items?offset=10&limit=5`

You can click next at the bottom of the query result to increment the offset parameter by the value of limit. Note that the value of limit remains unchanged. In the above example, when you click next, the value of offset changes to 15 and the next five items are displayed. Also, you can click prev at the bottom of the query result to decrease the value of the offset parameter by the value of limit. In the above example, when you click prev, the value of offset changes to 5 and the previous five items are displayed.

Note:

The Item Search API is not designed for deep pagination. Therefore, using offset and limit to page through sorted results works well if you only need to access the first few pages of the search results.

The default value of the offset parameter is 0 and that of the limit parameter is 50. Therefore, when you do not specify offset and limit, the first 50 items are displayed in the query results.

## Facet and Filter Items {#bridgehead_4139347112}

-   `<facet_field_name>` - You can specify the facet field name and facet values to retrieve the item IDs of the items associated with the specified facets and facet values. For example, you can filter items for the specified facets and facet values:
    
    `http://www.mywebstore.com/api/items?color=red,blue&gender=women`
    
    If you are unsure about the facet value or if special characters are included in the facet value you want to specify in the query, you can call the Search API requesting all facets. For example, you can request all facets using the following query string:
    
    `http://www.mywebstore.com/api/items?pricelevel=5&include=facets`
    
    You can then use the appropriate value that is contained in the response to construct your API query.
    
    Note:
    
    If you create a custom list intended for use as a facet, do not include a comma in any of the list values. In an API request, the comma is interpreted as a separator between multiple options.
    
-   `<numeric_facet_field_ID>.ranges` - You can use the parameter `<numeric_facet_field_ID>.ranges` to define range buckets for numeric facets fields such as price. Use the suffix `ranges` on the field ID to perform the search. For example, you can retrieve an array of range buckets with the number of items in each bucket using the following query string:
    
    `http://www.mywebstore.com/api/items?pricelevel5.ranges=1-10,10-20,20-*`.
    
    The range buckets in this example are 1 to 10, 10 to 20, and 20 or more.
    
    The range buckets used to compute range faceting are inclusive of their lower bounds and exclusive of their upper bounds. In the above example, 10 is considered in the range bucket 10 to 20 and not in the range bucket 0 to 10.
    
    Note:
    
    Facet ranges do not filter, but instead show additional data in the facet section of the JSON response pertaining to how many items are in each range.
    
-   `<numeric_facet_field_ID>.from&<numeric_facet_field_ID>.to` - To specify a range of values to search for on item records, you can use the parameters `<numeric_facet_field_ID>.from` and `<numeric_facet_field_ID>to`. Use the suffix from and to on the field ID to perform the search. Both from and to are required, and excluding one results in an error. Also, you can only use the field ID of the facet field in facet range filters, and not the URL component of the facet.
    
    For example, you can retrieve all the items with a price between 10 and 20 (both inclusive) using the following query string:
    
    `http://www.mywebstore.com/api/items?pricelevel5.from=10&pricelevel5.to=20`
    
    Note:
    
    When the **Prices Include Tax** preference is set, tax is included in the price of each item. However, the Item Search API does not support the Tax Inclusive Pricing feature. Therefore, tax exclusive prices are used when you filter the items using any price-related facet.
    

## Include or Exclude Item Attributes {#bridgehead_N2666872}

-   `include` - You can use the parameter `include` to specify an item attribute in the API request and retrieve additional data in the JSON response. For example, the following sample query includes facet fields in the JSON response:
    
    `http://www.mywebstore.com/api/items?include=facets`
    
-   `facet.exclude` - You can use the parameter `facet.exclude` to exclude fields from faceting in Item Search API calls. Excluding facet fields that are not essential can help speed up the API calls. The `facet.exclude` parameter accepts comma delimited facet field names.
    
    In the following example, the API call specifies a facet value for filtering (`custitem_categories=Kitchen-Utensils`), while excluding the field from faceting (`facet.exclude=custitem_categories`).
    
    `http://www.mywebstore.com/api/items?include=facets&fieldset=search&language=en&country=US&currency=USD&pricelevel=5&c=1234567&n=2&custitem_Utensils&sort=pricelevel5&asc&limit=24&offset=0&c=1234567&facet.exclude=custitem_categories`
    

## Sort Items {#bridgehead_N2667008}

You can use the parameter `sort` to define the sort order of search results on your website. By using the field ID you want to sort by in the API request, you can retrieve item record data sorted by the field ID included in the API request. You can find the field ID on the Sort Fields subtab on the Web Site Setup page. An Item Search API request overrides your settings on the Search Fields tab. Supported sort orders are ascending (`asc`) and descending (`desc`).

For example, you can sort the items by their store display name using the following query string:

`http://www.mywebstore.com/api/items?sort=storedisplayname:asc`

Items are sorted by category when the value of `commercecategory` and either `commercecategoryid` or `commercecategoryurl` are specified. This is dependent on the Commerce Category sort field being defined in the Web Site Setup record.

For more information about setting up web site preferences for sorting in NetSuite, see [Select and Configure Sort Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659294.html).

Note:

If you are sorting by a field which is empty for a particular item, the item is excluded from sorting and is displayed at the end of the list.

## Specify Price Level {#bridgehead_4077931895}

You can use the parameter `pricelevel` to specify the price level ID for items. The price level ID can be different depending on how price levels are configured in your NetSuite account. Typically, the default online price in NetSuite is `pricelevel=5`.

`http://www.mywebstore.com/api/items?pricelevel=4&include=facets`

Note:

If you have set up multiple price levels for items, ensure that you add all the price level fields as sort fields. For more information, see [Select and Configure Sort Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659294.html). Also, if Alternate Price is not defined for an item but is set to be displayed in a field set, then the value of Alternate Price defaults to the Online Price. If Online Price is also not defined for the item, then the value of Alternate Price defaults to the Base Price.

When a customer with a custom price level is logged in on the web store, the price level assigned to that customer is retrieved instead of the default online price level. For example, the default online price is `pricelevel=5`, but the price level assigned to a certain customer may be `pricelevel=4`. When this customer is browsing in the web store, the customer's assigned price, `pricelevel=4` is sent in the search API call. Consequently, the custom price (`pricelevel=4`) is displayed to this customer for all the products in the web store.

Note:

The pricelevel parameter is only usable when a user with permissions to see the requested pricelevel is logged in. In all other cases, the pricelevel displayed is in accordance with the default setting in the Web Site Set Up record.

## Specify Currency {#bridgehead_N2666712}

Prices are usually displayed in the default currency that you have set up for your website. In an account that uses the Multiple Currencies feature, you can use the parameter currency with the ISO Country Code to specify the currency format in which you want to display prices for the items.

`http://www.mywebstore.com/api/items?fields=onlinecustomerprice_formatted,pricelevel5&currency=USD`

If you are using the Multiple Currencies feature, ensure that you select the correct default locale on the currency record to avoid any errors related to currency mismatch. For example, select New Zealand (English) as the default locale for New Zealand Dollar. For more information, see [Creating Currency Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1395911.html).

Note:

If you specify a currency that is not associated with your website or if the Online box is not checked for that currency on the Web Site Setup record, an error message is returned.

## Specify Language and Country {#bridgehead_N2666692}

A shopper on your website can use their local language to search and browse products on your website. The translated text that shoppers see in product views is based on the translated text you set up on item records. The JSON response data includes item attributes and field set fields in the languages you have set up in your NetSuite account. You must add the corresponding fields to a field set and also check that the field set is included in the Reference ShopFlow SuiteApp. By default, items are returned with fields containing the default language. You can use the language and country parameter to specify the translated text you set up in NetSuite.

In the following example, the search results are displayed in Spanish:

`http://www.mywebstore.com/api/items?fieldset=search&country=ES&language=es`

Note:

You must always use the language and country parameters together. The country code that you specify should be in uppercase and the langue code should be in lowercase.

All ISO country and language codes are valid if the language is set up for use on your website. To affect the language displayed in a product view, the site template must be localized. For more information about localizing site templates and using multiple languages, see [Localization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3825631277.html).

## Callback Function {#bridgehead_N2666671}

You can use the parameter `callback` to define the JavaScript callback function to wrap the JSON response.

For example, you can create a variable name `mycallback` by using the callback parameter as shown in the following sample query:

`http://www.mywebstore.com/api/items?callback=mycallback`

## Retrieve Debug Information {#bridgehead_N2666732}

You can use the parameter `ssdebug` and set its value to `true` to retrieve the debug information in the JSON response.

`http://www.mywebstore.com/api/items?ssdebug=true`

### Related Topics:

-   [Items Available to the Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520340184.html)
-   [The Base URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665502.html)
-   [Sample Item Search Query and Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2667130.html)
-   [Item Search API Output Response](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509454056.html)
-   [Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2665337.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
