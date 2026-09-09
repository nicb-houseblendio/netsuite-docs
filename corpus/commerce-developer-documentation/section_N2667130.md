---
id: "section_N2667130"
type: "section"
title: "Sample Item Search Query and Results"
branch: "commerce-developer-documentation"
category: "commerce"
breadcrumb: "Commerce > Commerce Developer Documentation > Commerce APIs > Item Search API > Sample Item Search Query and Results"
parent: "chapter_N2665337"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2667130.html"
anchors: ["bridgehead_3746291217", "bridgehead_4696130354", "bridgehead_4798303265", "bridgehead_4798317988", "bridgehead_4798322399"]
sha256: "e0eeacd278a6cf46ff02e3c0cf8005b1738edf2446a61bf04aa5ae9b8de9082c"
---

This section provides sample Item Search API queries and their response data.

-   [Sample Search Query for Returning Item Quantity](#bridgehead_3746291217)
    
-   [Sample Search Query for Returning Categories](#bridgehead_4696130354)
    
-   [Sample Search Query for Returning Items Available for Store Pickup](#bridgehead_4798303265)
    

## Sample Search Query for Returning Item Quantity {#bridgehead_3746291217}

If you use the Multi-Location Inventory feature, you can access item inventory per location using fields specifically designed to return item location details. You can use these fields to retrieve the Item Quantity details:

-   Quantity Available (quantityavailable\_detail)
    
-   Quantity Backordered (quantitybackordered\_​detail)
    
-   Quantity Committed (quantitycommitted\_​detail)
    
-   Quantity On Hand (quantityonhand\_detail)
    
-   Quantity On Order (quantityonorder\_detail)
    

By using these fields with the Item Search API, you can retrieve the item inventory data. You can also create a field set that includes these fields, and then use that field set in a query to the Item Search API. For information about creating field sets, see Define Field Sets.

Important:

When the Sales Channel Allocation feature is enabled, the item quantity details retrieved using the Quantity Available (quantityavailable\_detail) field with the Item Search API might not match the value displayed in the Quantity Available field on the item record.

This behavior occurs because the Quantity Available (quantityavailable\_detail) field is returning the sum of Quantity Available and Quantity Allocated to Order Reservation instead of just Quantity Available.

The following example shows a query string that returns data from the Quantity Backordered field on the item record:

`http://www.mywebstore.com/api/items?pricelevel=5&fieldset=myfieldsetwithqtybackordered`

The item quantity information is written to the JSON response, which includes internal ID of the location and quantity back ordered for each item:

          `items: [ {       qtybackordered_detail:{          qtybackordered:10          locations:[                      {                         internalid:1,                         qtybackordered:6                      },                      {                         internalid:2,                         qtybackordered:4                      }                      ]                                  } } ]` 
        

## Sample Search Query for Returning Categories {#bridgehead_4696130354}

The following query returns items where the comcat fieldset is configured with a commerce category ID 3. Facet information is also returned in the response. For each item returned, category details are returned including:

-   The URL fragments defined for that category.
    
-   The commerce category name used in the facet.
    

Note:

To successfully run this query, the Commerce Category facet field and field set must be configured in the Web Site Set Up record. For more details on working with Categories, see [Commerce Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4673202005.html).

`http://www.mywebstore_suite.com/api/items?fieldset=comcat&include=facets&commercecategoryid=3`

          `{   "total": 4,   "items": [     {       "internalid": 388,       "commercecategory": {         "primarypath": [           {             "urls": [               "/apparel/partywear/shoes"             ],             "name": "Shoes",             "id": 3           },           {             "urls": [               "/apparel/partywear"             ],             "name": "Partywear",             "id": 2           },           {             "urls": [               "/apparel"             ],             "name": "Apparel",             "id": 1           }         ],         "categories": [           {             "urls": [               "/apparel/partywear/shoes"             ],             "name": "Shoes",             "id": 3           }         ]       },       "storedisplayname2": "Shoes - Reebok 9K"     },     ...   ],   "facets": [     {       "id": "commercecategoryname",       "values": [         {           "url": "Shoes"         }       ]     },     ...  ],   "links": [],   "corrections": [],   "locale": {     "country": "US",     "language": "en",     "currency": "USD",     "region": 1   },   "volatility": "unique",   "code": 200,   "warnings": {} }` 
        

## Sample Search Query for Returning Items Available for Store Pickup {#bridgehead_4798303265}

When you use the `isstorepickupallowed` field with the Item Search API and set it to true, the Item Search API returns the item IDs of all the matching items for which store pickup is enabled. When this field is set to false, the Item Search API returns the item IDs of all the matching items for which store pickup is not enabled.

If you enable the Multi-Location Inventory feature, you can access the item quantity per location. If you use the `quantityavailableforstorepickup_detail` field with the Item Search API, you can also access the item quantity available for store pickup per location.

The following example shows a query string that returns data from the Quantity Available and Quantity Available For Store Pickup fields on the item record. Alternatively, you can create a field set that includes Quantity Available and Quantity Available For Store Pickup fields, and then use that field set in a query to the Item Search API.

`http://www.mywebstore.com/api/items?isstorepickupallowed=true&fields=quantityavailable_detail,quantityavailableforstorepickup_detail`

Note:

To successfully run this query, the Store Pickup Allowed facet field must be configured in the Web Site Setup record. You must also define the Available For Store Pickup (Detail) field in the Web Site Setup record field sets. For more information, see [Accessing Item Quantity Available for Store Pickup Per Location](#bridgehead_4798317988).

For each item returned in the JSON response, the data includes the internalid of the item, total item quantity available, item quantity available by location, and item quantity available for store pickup by location:

          `"items":[       {             "internalid":388,             "quantityavailable_detail":{                   "quantityavailable":90.0,                   "locations":[                         {                               "internalid":2,                               "quantityavailable":39.0                         },                         {                               "internalid":3,                               "quantityavailable":51.0                         }                   ]                },                "quantityavailableforstorepickup_detail":{                      "locations":[                            {                                  "internalid":2,                                  "qtyavailableforstorepickup":39.0                            },                            {                                  "internalid":3,                                  "qtyavailableforstorepickup":51.0                            }                      ]                }       },       {             "internalid":387,             "quantityavailable_detail":{                   "quantityavailable":150.0,                   "locations":[                         {                               "internalid":2,                               "quantityavailable":150.0                         }                   ]             },             "quantityavailableforstorepickup_detail":{                   "locations":[                         {                               "internalid":2,                               "qtyavailableforstorepickup":150.0                         }                   ]             }       },       {             "internalid":107,             "quantityavailable_detail":{                   "quantityavailable":4.0,                   "locations":[                         {                               "internalid":2,                               "quantityavailable":3.0                         },                         {                               "internalid":3,                               "quantityavailable":1.0                         }                   ]             },             "quantityavailableforstorepickup_detail":{                   "locations":[                         {                               "internalid":2,                               "qtyavailableforstorepickup":3.0                         }                   ]             }       } ],` 
        

In the above JSON response, we can see the following:

-   The first item with internal ID 388 is available at two locations, and both locations allow store pickup for the quantity available at the respective locations.
    
-   The second item with internal ID 387 is only available at one location, and that location allows store pickup for the quantity available.
    
-   The third item with internal ID 107 is available at two locations, but only one location allows store pickup for the quantity available at that location.
    

## Accessing Item Quantity Available for Store Pickup Per Location {#bridgehead_4798317988}

To access the quantity available for Store Pickup per location using the Item Search API, you need to create a field set that includes fields listed under [Item Fields Related to Store Pickup](#bridgehead_4798322399).

#### To create a field set that includes information about item quantity available for store pickup:

1.  Go to _Commerce > Websites > Website List_.
    
2.  Click the **Field Sets** subtab.
    
    1.  Enter a **Name** for the field set. For example, enter **Store Pickup**.
        
    2.  Enter a **Field Set ID** for the field set. For example, enter **storepickup\_details**.
        
    3.  Select **Item** for **Record Type**.
        
    4.  (Optional) Enter a description for the field set.
        
    5.  In the Field Set popup window, select the store pickup related field names listed in the subsequent table.
        
    6.  Click **Add**.
        
3.  Click **Save**.
    
4.  Use the field set in a query to the Item Search API. For example,
    
    `http://www.mywebstore.com/api/items?fieldset=storepickup_details`
    

The store pickup related information is returned in the JSON response.

## Item Fields Related to Store Pickup {#bridgehead_4798322399}

The following table shows the item record fields that correspond with fields exposed to field sets:

| **Field Label on the Locations Subtab of the Item Record** | **Field Set Field Name** | **Field ID** |
| --- | --- | --- |
| Allow Store Pickup | Store Pickup Allowed | isstorepickupallowed |
| Quantity Available For Store Pickup | Available For Store Pickup (Detail) | quantityavailableforstorepickup\_detail |

### Related Topics

-   [Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2665337.html)
-   [Items Available to the Item Search API](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1520340184.html)
-   [The Base URL](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665502.html)
-   [Item Search API Input Parameters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2665676.html)
-   [Item Search API Output Response](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1509454056.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
