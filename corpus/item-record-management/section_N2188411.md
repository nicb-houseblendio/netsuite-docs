---
id: "section_N2188411"
type: "section"
title: "Generating an Individual Price List"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Generating Price Lists > Generating an Individual Price List"
parent: "section_N2185787"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188411.html"
anchors: ["procedure_N2188448", "bridgehead_N2188669"]
sha256: "ea829fc069bc4af3873c7efca1b7e9c4826afc1aa2a07adee76c3888d0f9388d"
---

You can generate a price list for one customer at a time. You can also customize to filter the items list. For more information, see [Customizing to Filter the Items List](#bridgehead_N2188669).

#### To generate an individual price list: {#procedure_N2188448}

1.  Go to _Transactions > Customers > Individual Price List_.
    
2.  Select the customer whose price list you want to generate.
    
3.  If you use the Multiple Currencies feature, select the currency you want to generate this price list in.
    
    For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
4.  Enter or select the date you want to show on the price list.
    
5.  Check the **Assigned Price Levels Only** box to show only the price levels set for the customer on the list you generate. Clear this box to show all price levels.
    
6.  You can choose an option for column headings by checking or clearing the **Round Quantities** box.
    
    -   If you check this box, the quantity range shows up, like '1-9, 10-99, 100+'
        
    -   If you clear this box, only the minimum quantity shows up, like '0, 10, 100'
        
    
    After you set this box, the same setting is used by default every time you view this page, until you change the selection.
    
    This setting is used by default on both the individual price list page and the bulk generate price lists page.
    
7.  Select a form to use for generating the list. For more information, see [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html).
    
    Select **System Preference** to use the default form for this transaction. Default forms are set by checking the **Form is Preferred** box on the custom form record. You can also check the box in the **Preferred** column next to the form on the Custom Transaction Form page.
    
8.  In the **Type** field, select an item type to filter the list and print prices only for that item type. For example, select **Inventory Item** to only print price lists for inventory items.
    
    Press and hold the **Ctrl** key to select multiple item types.
    
    After you select a filter, it shows up every time you view this page, until you change the selection. The filter shows by default on the Items subtab on both the individual and bulk price list pages.
    
9.  Generate the price list:
    
    -   Click **Print** to print the price lists.
        
    -   Click **Email** to email the price lists.
        
        To email the price lists, each customer needs to have an email address entered in their customer record.
        
    -   Under **Actions**, click **Fax** to fax the price lists.
        
        Note:
        
        An administrator needs to set up fax service first. Go to Setup > Company > Set Up Company > Preferences > Printing & Fax on the Fax subtab. Each customer also needs a fax number in their record.
        

## Customizing to Filter the Items List {#bridgehead_N2188669}

When you generate individual price lists, you can customize the items list to filter by specific fields. This lets you generate price lists only for specific items.

#### To customize to filter the items list:

1.  On the Generate Price List page, above the items list, click **Customize**.
    
2.  On the Customize Sublist page, click the **Additional Filters** subtab.
    
3.  Next to fields you want to sort by, check the **Include** box.
    
4.  Click the **Additional Columns** subtab.
    
5.  Next to the columns you want to show, check the **Include** box.
    
6.  Click **Save**.
    

Note:

When you customize the list filters, the custom results won't show up on the price list you create. You'll need to customize the price list form to show these results. For more information, see [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html).

### Related Topics

-   [Customize Price List Pages and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2186163.html)
-   [Price List Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2187468.html)
-   [Searching for Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171136751.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171157590.html)
-   [Generating Bulk Price Lists and Customizing Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2187796.html)
-   [Working With Pricing Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2189322.html)
-   [Generating Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
