---
id: "section_N2185787"
type: "section"
title: "Generating Price Lists"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Item Pricing > Generating Price Lists"
parent: "chapter_N2180614"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185787.html"
anchors: []
sha256: "5856f7eeb660947c91e1c0738d8bd67fa184b1363e44f45a18f92e6f8f6d1399"
---

You can generate a price list that shows your items and their prices for each customer. Then you can print, fax, or email this price list to your customer.

When you print a price list for a customer, the item prices are based on the price level or group set for that customer. This is the same price that shows up when you add the item to a sales transaction for that customer.

If you use the Multiple Currencies feature, price lists are only generated for a customer's primary currency. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).

The following steps walk you through generating price lists from different NetSuite pages.

#### To generate price lists from the Print Checks and Forms page:

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Price Lists**.
    
3.  On the **Generate Price Lists** page, select the customer accounts you want to generate a price list for.
    
4.  Click **Print**.
    
    Or, click **Email** to send the price list to a contact.
    

#### To generate price lists from a customer record:

1.  Go to _Lists > Relationships > Customers_.
    
2.  Next to the customer record, click **View**.
    
3.  Click **More Actions**, then click **Generate Price List**.
    
4.  Click **Print**.
    
    Or, click **Email** to send the price list to a contact.
    

#### To generate price lists from the Transactions > Customers menu:

1.  Go to Transactions > Customers.
    
2.  Click one of the following:
    
    -   To create price lists for more than one customer, click **Generate Price Lists**.
        
        1.  On the **Customers** subtab, select the customers you want to create a list for.
            
        2.  On the **Items** subtab, choose the items to show in the price list.
            
            You can also click the **Customize** button to filter the lists.
            
            For more information, see [Generating Bulk Price Lists and Customizing Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2187796.html).
            
    -   To create a price list for one customer, click **Individual Price List**.
        
        1.  Select the customer or project you're creating a price list for.
            
        2.  Choose which items to include in the list. For example, you can show only inventory items.
            
            For more information, see [Generating an Individual Price List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188411.html).
            
    
    After you select a filter, it shows up every time you view this page. The selected filter appears on the **Items** subtab on both price list pages.
    
    The customer list doesn't show jobs if you set the Consolidate Projects on Sales Transactions preference.
    
    The standard price list form shows the customer's address, the date the list is generated, item names and descriptions, item prices, and currencies. If you use the Quantity Pricing feature, the price list shows a column for each quantity and the matching prices.
    
3.  Optionally, check the **Round Quantities** box.
    
    -   If checked, the quantity range appears, for example, '1-9, 10-99, 100+.'
        
    -   If cleared, only the minimum quantity appears, for example, '0, 10, 100.'
        
    
    Note:
    
    Items with no price entered on the item record won't show up in the price list document.
    
4.  After the list is set, you can send the lists by email, fax, or print and send them. You can print, fax, or email up to 100 price lists at one time.
    

One price list document is made per customer. If a document needs more than one page, the pages are numbered if you customize price list forms to show page numbers. For more information, see [Customizing Price List Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2188838.html).

The following NetSuite roles can print price lists:

-   A/R Clerk
    
-   Accountant
    
-   Accountant (Reviewer)
    
-   Bookkeeper
    
-   CEO
    
-   CEO (Hands Off)
    
-   CFO
    
-   Customer Center
    

The Price List function isn't meant to show or print a specific price level for all items. To do that, you need to create a pricing search. For more information, see [Working With Pricing Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2189322.html).

### Related Topics

-   [Customize Price List Pages and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2186163.html)
-   [Price List Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2187468.html)
-   [Searching for Price Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171136751.html)
-   [Absolute Pricing for Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163171157590.html)
-   [Setting Up Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181018.html)
-   [Using Multiple Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2181607.html)
-   [Using Quantity Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2183333.html)
-   [Creating Pricing Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184077.html)
-   [Updating Item Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184312.html)
-   [Updating Item Purchase Prices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2184741.html)
-   [Swapping Prices Between Price Levels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185052.html)
-   [Creating Item Coupons](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2185383.html)
-   [Item Pricing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2180614.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
