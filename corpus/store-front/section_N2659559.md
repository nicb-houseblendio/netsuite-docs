---
id: "section_N2659559"
type: "section"
title: "Define Field Sets"
branch: "store-front"
category: "commerce"
breadcrumb: "Commerce > Store Front > Search > Search Settings Overview > Define Field Sets"
parent: "section_N2656810"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659559.html"
anchors: ["procedure_N2659652", "bridgehead_1500648146"]
sha256: "93dcec87e5b75288c8c27e0bbfeb771176f4ad83eec23c08653256ce55e1a495"
---

You can show information from your NetSuite item records to your website by defining field sets. After you define the field sets, a web developer can use the Item Search API to access field values in the field sets.

For example, you might make a field set for the product details page with fields like product name, images, description, availability, and price. You could also create a different field set for the search results page, which includes fields that display an image thumbnail, product name, and price.

Note:

Field Sets are made public on the internet. Since you can pick any field type, make sure you're careful about which fields you expose.

You can use the Field Set Setup Script to quickly add the required Field Sets to your site. To run a script to create the field sets, see [Set Up Initial Field Sets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3716578295.html).

You can also define your own field sets on the Web Site Setup page. To define your own field sets, follow the inline procedure.

#### To define your own field sets: {#procedure_N2659652}

1.  Complete the prerequisite tasks as described in [Prerequisites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html#bridgehead_1499270591).
    
2.  Go to _Commerce > Websites > Website List_.
    
3.  Click **Edit** next to your SuiteCommerce Advanced site.
    
4.  Click the **Field Sets** subtab.
    
5.  In the **Name** field, enter a name for the new Field Set. This name is only displayed internally on the Field Sets list page and in dropdown lists on the Web Site Setup page. Name each Field Set based on the product views you create for your site.
    
    Important:
    
    The Field Set to return item details is typically named **details**. If you use a different name, you'll need to update the `searchApiMasterOptions` property. See [Search Results Subtab](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4667044776.html) for more details on configuring this property.
    
6.  In the **Field Set ID** field, enter an ID you'll use later with the Item Search API as an input parameter to specify the field set. The ID has to be alphanumeric, lowercase, and can't have spaces or special characters. The Field Set ID is displayed internally, on the Field Sets list page and in dropdown lists on the Web Site Setup page.
    
7.  The **Record Type** field is pre-populated with the value Item as only item records are supported.
    
8.  The **Description** field is an optional. You can add a description if you want, and it'll only show on Field Set records, the Field Set list, and the Web Site Setup page.
    
9.  To populate the **Fields Included in Field Set** field, click the Set icon next to this field. A Field Set window opens.
    
    Important:
    
    When defining a field set for a merchandising zone, include the following fields in your field set to ensure it appears correctly on your web store.
    
    -   Internal ID
        
    -   Matrix Child Items (Detail)
        
    -   Store Display Name 2 or Display Name
        
    -   Price for Current Customer (Formatted)
        
    -   URL Component
        
    -   Item Images (Detail)
        
    
    For more information about merchandising zones see, [Merchandising Zone Content](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159561426850.html).
    
10.  In the Field Set window, select the item record field from the **Field Name** field and click **Add**.
     
11.  Repeat Step 10 for each item record field you want to include in the field set.
     
12.  After you have selected all the fields, click **Submit**. The values of the **Field ID** and **Field Type** fields are auto populated for the selected field. You can use the field ID to refer to specific fields when writing SuiteScript. This is also the field ID returned in the JSON response when using the Item Search API. The field type refers to the NetSuite field type. Field types provide information about the type of data web developers can expect in the JSON response to Item Search API queries.
     
13.  Click **Add** on the Web Site Setup page to add the new field set.
     
14.  Click **Save** to save your changes.
     

Defining field sets is the last step in configuring item search settings. When you click Save on the Web Site Setup page, the item search indexing process starts. For more information, see [Search Index Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2659979.html) and [Check the Search Index Job Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1500035318.html).

## Field Set Reference {#bridgehead_1500648146}

We've provided a Microsoft Excel worksheet with all the fields you can use in field sets. You can use this list to find field IDs, field types, and see which fields are available for faceting, sorting, and keyword search. The worksheet also shows additional fields with derived values, called Synthetic fields.

To access the worksheet, click this link: [FieldSetsList.xls](https://system.netsuite.com/core/media/media.nl?id=14901011&c=NLCORP&h=39759c97a3a915a0a132&_xt=.xls)

Note:

Depending on what features you have enabled, some fields in the spreadsheet might not show up in your account.

### Related Topics

-   [Derived Fields for Field Sets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3923307567.html)
-   [Search Settings Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2656810.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
