---
id: "section_N2189322"
type: "section"
title: "Working With Pricing Searches"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Generating Price Lists > Working With Pricing Searches"
parent: "section_N2185787"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2189322.html"
anchors: ["subsect_163171434905", "bridgehead_N2189398", "subsect_163171452696", "bridgehead_N2189572", "subsect_163171472479", "bridgehead_N2190890", "subsect_163171559393"]
sha256: "114469288334463ab3a18cf6fba9f8908079ae2e9ab51a7fb0daebbd0f08ba05"
---

A pricing search lets you set up an item search to generate a price list. For example, you can run a pricing search to display the price of items at a certain price level for all items on that level.

There are three ways to run a pricing search:

-   [Running a Standard Pricing Search](#subsect_163171434905)
    
    A standard pricing search defaults to search with filters for Items and Customers.
    
-   [Customizing a Pricing Search](#subsect_163171472479)
    
    A custom pricing search gives you greater flexibility to determine search filters and the results that show.
    
-   [Creating a Saved Search for the Quantity Pricing Feature](#subsect_163171559393)
    
    A saved pricing search enables you to set specific search criteria and results, as well as save the search to use again in the future.
    

## Running a Standard Pricing Search {#subsect_163171434905}

Use the following procedure to run a standard pricing search.

#### To run a standard pricing search: {#bridgehead_N2189398}

1.  To set up a price list search, go to _Reports > New Search_.
    
2.  On the **Search** page, click **Pricing**.
    
3.  In the **Item** field, select **any of** and enter the name of the item.
    
    To search by exclusion, select **none of**.
    
    To select more than one item:
    
    1.  Beside the field, click the **Select Multiple** icon.
        
    2.  Click each item to add to the **Current Selections** column.
        
    3.  After you have selected all your items, click **Done**.
        
4.  To search for prices by customer:
    
    1.  In the **Customer** field, select **any of**.
        
        To search by exclusion, select **none of**.
        
    2.  Enter the customer name.
        
        To select more than one customer:
        
        1.  Click the **Select Multiple** icon.
            
        2.  Click each customer to add to the **Current Selections** column.
            
        3.  When finished, click **Done**.
            
5.  Click **Submit**.
    

The search results show the Item Name, Quantity Range, Sale Unit, and Unit Price for all applicable items. When viewing the search results, you can print, email, or export the results. You can also save the search to run it again if needed.

Note:

If you use the Multiple Currencies feature, results are shown in the customer's currency.

A price list report doesn't show all pricing levels for an item. The report shows only the price level for the specified customers.

If you require more details than provided in the standard pricing search, see the following procedure.

### Creating an Advanced Pricing Search {#subsect_163171452696}

Use the following procedure to create an advanced pricing search.

#### To create an advanced pricing search: {#bridgehead_N2189572}

1.  To set up an advanced price list search, go to _Reports > New Search_. On the Search page, click **Pricing**.
    
2.  On the Pricing Search page, check the **Use Advanced Search** box.
    
    You can show only the price levels set for the customer on the list you generate.
    
    1.  On the **Criteria** subtab, click the **Standard** subtab.
        
    2.  In the **Filter** field, select **Assigned Price Level**.
        
    3.  In the popup window, select **Yes** for **Assigned Price Level**.
        
    4.  Click **Set**.
        
    5.  In the **Filter** field, select **Customer**.
        
    6.  In the popup window, set the customers by selecting **any of** or **none of** and choosing customers to include or exclude.
        
        If you don't select a customer, no search results are returned.
        
    7.  Click **Set**.
        
3.  Set additional criteria and results settings as needed.
    
4.  Click **Submit**.
    

## Customizing a Pricing Search {#subsect_163171472479}

Use the following procedure to customize a pricing search.

#### To customize a pricing search: {#bridgehead_N2190890}

1.  To set up a price list search, go to _Reports > New Search_. On the Search page, click **Pricing**.
    
2.  On the Pricing Search page, click **Personalize Search**.
    
3.  Use the **Available Filters** subtab to limit the set of filters available on the form when you reuse this search. You can also set footer filters for the results, such as when used as a list view.
    
    Select the item and customer information you want to filter the search by.
    
    Note:
    
    Remove all filters to use advanced search.
    
4.  On the **Results** subtab, select the data you prefer to show in the results and determine sorting.
    
5.  You can click **Show More Options** to check the **Show in Menu** box. Then, this search appears in the list of saved searches at _Lists > Search > Saved Searches._.
    
6.  Click **Save**.
    

Your custom search is available to run a pricing search as needed.

## Creating a Saved Search for the Quantity Pricing Feature {#subsect_163171559393}

If you use the Quantity Pricing feature, on the Results subtab you can select to show the item Minimum Quantity and Maximum Quantity. Because fractional quantities are allowed in some cases, the maximum quantity is the same as the minimum quantity of the next level. The Price Range results subtract 1 from the maximum quantity and set the minimum quantity to 1 if it's 0.

Or, you can set up a formula to generate an alternate range, such as '0-99.99' or '0 up to 100'. For more information, see [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html).

The search results list all items grouped by the quantity pricing brackets that apply to each. Within each group, items are sorted as specified in the item sublist. Items with no quantity pricing are shown in the Unit Price column.

You can also create a saved search for pricing.

#### To create a saved search for pricing:

1.  To set up a price list search, go to _Lists > Search > Saved Searches > New._. On the Search page, click **Pricing**.
    
2.  Click **Create Saved Search**.
    
3.  Set the criteria and results for this search:
    
    -   On the **Criteria** subtab, in the **Filter** column, select the item and customer information you want the search to find.
        
    -   On the **Results** subtab, select the data you want to show in the results and determine sorting.
        
    
    For example, to search by price level, on the **Criteria** subtab, set a filter for **Price Level**. Select the price level you want to appear. Then, on the **Results** subtab, include pricing in the data you select to show. The search results will display only customers with the selected price level assigned.
    
4.  If you check the **Show in Menu** box, this search shows in the list of saved searches at _Lists > Search > Saved Searches._.
    
5.  **Preview** or **Save** the search:
    
    -   To see the results, click **Preview**.
        
    -   To save the search without running the results, click **Save**.
        
    -   To save the search and also display the results, click **Save and run**.
        
    -   To save the search and also email the results, click **Save and Email**.
        
    
    If you use the Multiple Currencies feature, the results show in the customer's currency.
    

### Related Topics

-   [Customize Price List Pages and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2186163.html)
-   [Price List Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2187468.html)
-   [Searching for Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171136751.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171157590.html)
-   [Generating Bulk Price Lists and Customizing Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2187796.html)
-   [Generating an Individual Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188411.html)
-   [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
