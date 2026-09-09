---
id: "section_N2187796"
type: "section"
title: "Generating Bulk Price Lists and Customizing Lists"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Generating Price Lists > Generating Bulk Price Lists and Customizing Lists"
parent: "section_N2185787"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2187796.html"
anchors: ["bridgehead_1493668377", "procedure_N2187834", "subsect_163171300997"]
sha256: "bcd3fd2412b53af0495472fb827cb96a6fd0d7d3e41f687611f5215bb892f844"
---

You can generate price lists for lots of customers at one time. See the following for more information.

-   [Generating Price Lists in Bulk](#bridgehead_1493668377)
    
-   [Customizing the Customer List or Items List Filters](#subsect_163171300997)
    

## Generating Price Lists in Bulk {#bridgehead_1493668377}

If you use the Multiple Currencies feature, price lists are only generated for a customer's primary currency. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

#### To bulk generate price lists: {#procedure_N2187834}

1.  Go to _Transactions > Customers > Generate Price Lists_.
    
    Or, you can go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Price Lists**.
    
3.  Enter or select the date you want to appear on the price list.
    
4.  If you use the Multiple Currencies feature, in the **Currency** field, select one of the following:
    
    -   **All** - Prices are printed for every transaction currency for each customer you select.
        
    -   **Primary** - Prices are printed only in each customer's primary currency.
        
5.  Check the **Assigned Price Levels Only** box to show only the price levels set for the customer on the list you generate. Clear this box to show all price levels.
    
6.  You can choose an option for column headings by checking or clearing the **Round Quantities** box.
    
    -   If you check this box, the quantity range shows up, like '1-9, 10-99, 100+'
        
    -   If you clear this box, only the minimum quantity shows, like '0, 10, 100'
        
    
    After you set this box, the same setting is used by default every time you view this page, until you change it.
    
    The setting is used by default on both the individual price list page and the bulk generate price lists page.
    
7.  Select a form to use for generating the lists. For more information, see [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html).
    
    Select **System Preference** to use the default form for this transaction. Default forms are set by checking the **Form is Preferred** box on the custom form record. You can also check the box in the **Preferred** column next to the form on the Custom Transaction Form page.
    
8.  On the **Customers** subtab, check the box in the **Print** column next to the customers you want to generate a price list for. Click **Mark All** to print lists for all the customers in the list.
    
    The customer list doesn't show jobs if you set the **Consolidate Projects on Sales Transactions** preference. It also respects any restrictions on users' roles and only shows the right records.
    
9.  Click the **Items** subtab.
    
10.  In the **Type** field, select an item type to filter the list and print prices only for that item type. For example, select **Inventory Item** to only print price lists for inventory items.
     
     Hold down the **Ctrl** key to select multiple item types.
     
     After you select a filter, it applies every time you view this page until you change the selection. The filter shows up by default on the **Items** subtab on both the individual and bulk price lists pages.
     
11.  Generate the price lists:
     
     -   Click **Print** to print the price lists.
         
     -   Click **Email** to email the price lists.
         
         To email the price lists, each customer needs to have an email address entered in their record.
         
     -   Click **Fax** to fax the price lists.
         
         Each customer needs a fax number entered on their customer record.
         
         Note:
         
         An administrator needs to set up fax service first. Go to Setup > Company > Set Up Company > Preferences > Printing & Fax on the Fax subtab. Each customer also needs a fax number entered on their customer record.
         

## Customizing the Customer List or Items List Filters {#subsect_163171300997}

When you bulk generate price lists, you can customize the customer and items lists to filter by individual fields. This lets you generate price lists only for specific customers and items.

#### To customize list filters:

1.  Go to _Transactions > Customers > Generate Price Lists_.
    
2.  To customize filters for lists, select one of the following options:
    
    -   To customize filters for the customer list, click the **Customers** subtab, then click **Customize**.
        
    -   To customize the filters for the items list, click the **Items** subtab, then click **Customize**.
        
    
    Note:
    
    When you customize the list filters, the custom results won't show up on the price list you create. You'll need to customize the price list form to show these results. For more information, see [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html).
    
3.  On the Customize Sublist page, click the **Additional Filters** subtab.
    
4.  Check the **Include** box next to fields you want to sort by.
    
5.  Click the **Additional Columns** subtab.
    
6.  Check the **Include** box next to columns you want to show.
    
7.  Click **Save**.
    

### Related Topics

-   [Customize Price List Pages and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2186163.html)
-   [Price List Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2187468.html)
-   [Searching for Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171136751.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171157590.html)
-   [Generating an Individual Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188411.html)
-   [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html)
-   [Working With Pricing Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2189322.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
