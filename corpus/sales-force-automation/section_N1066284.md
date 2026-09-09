---
id: "section_N1066284"
type: "section"
title: "Creating an Opportunity Record"
branch: "sales-force-automation"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Sales Force Automation > Opportunities and Estimates > Opportunity Records > Creating an Opportunity Record"
parent: "section_N1066171"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066284.html"
anchors: ["procedure_N1066326"]
sha256: "246b8e0665a2cd9f88b6636809c0bf022b381f7117dbd166afc5beb438b7b5b8"
---

When a sales rep creates an opportunity record they indicate which sales items the customer is interested in. The sales rep also enters a probability that the deal will close. NetSuite uses that probability to calculate a projected total. As the negotiations continue, the sales rep can create multiple estimates relating to the deal.

The most critical piece of pipeline information on an opportunity record is the probability that the deal will close. Probability determines the weighted amount of the deal, which shows on pipeline and forecast reports.

NetSuite determines the weighted total by multiplying the probability by the total amount of the items on the opportunity.

NetSuite adds up the total weighted amount for all open estimates and opportunities to show the revenue you'll realize at period end. This amount is the pipeline total.

To delete a saved opportunity, from the Actions menu, click Delete. NetSuite adjusts the forecast data accordingly.

Note:

This is a non-posting transaction.

#### To create an opportunity: {#procedure_N1066326}

1.  Go to _Opportunities > Transactions > Opportunities > New_.
    
2.  If you use custom opportunity forms, select the form you want in the **Custom Form** field.
    
3.  Under Primary Information:
    
    1.  In the **Title** field, enter a name for this opportunity.
        
        NetSuite assigns a number to the opportunity. You can change this number.
        
    2.  Select the customer or prospect in the **Company** field.
        
    3.  Select a status for the opportunity.
        
        If there's a transaction other than an estimate in the opportunity, NetSuite sets the status to **Closed - Won**.
        
    4.  Enter a probability that the deal will close. NetSuite uses this probability to determine the weighted total of the opportunity.
        
        -   If you select the status **Closed Lost**, the probability sets to **0%.**
            
        -   If you select the status **Closed Won**, the probability sets to **100%.**
            
    5.  Enter the date you expect this opportunity to close.
        
    6.  Select a win or loss reason. You can use this list to close an opportunity.
        
    7.  When enabled, select a **Sales Channel**.
        
        To learn more, see [Enabling Sales Channels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161348620247.html).
        
4.  Under Forecasting:
    
    1.  NetSuite calculates the projected opportunity total in one of the following ways:
        
        -   If there are no items selected on the **Items** subtab and no included estimates or transactions, you enter a projected total.
            
            If you enter a projected total, it appears until you click **Update Projected** on the **Estimates** subtab.
            
        -   If there are items selected on the **Items** subtab, but no included estimates or transactions, the total of the selected items is the projected total.
            
        -   If there is one estimate associated with the opportunity and it is marked to include in forecasts, the estimate total is the projected total.
            
        -   If there are multiple estimates associated with the opportunity, the projected total is the sum of all the estimates marked to include in forecasts.
            
    2.  If you use the Advanced Forecasting feature, you can enter a range of amounts this deal might be worth.
        
        First, you must enable the **Multiple Projected Amounts** preference at _Setup > Sales & Marketing Automation > Sales Preferences_ on the **Forecast** subtab.
        
        -   The low amount entered has to be lower than or equal to the projected amount in the **Projected Total** field. This amount is the Worst Case projected total.
            
        -   The high amount has to be greater than or equal to the **Projected Total** amount. This amount is the Upside projected total.
            
    3.  If you use the Advanced Forecasting feature, in the **Forecast Type** field, select the forecast category you want this opportunity included in. For more information about forecast types, refer to [Opportunities in the Forecast and Pipeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1047903.html).
        
        The weighted total of the opportunity shows in the **Weighted Total** field.
        
        NetSuite calculates the weighted total by multiplying the projected total by the probability of close.
        
5.  Under Classification:
    
    If you track departments, classes, or locations, make the appropriate selections for this opportunity.
    
    Note:
    
    If you use NetSuite OneWorld and the selected customer is shared with multiple subsidiaries, you can choose any subsidiary assigned to that customer. For information about sharing customer records with multiple subsidiaries, see [Assigning Subsidiaries to a Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276747.html).
    
6.  On the **Items** subtab, this customer or prospect's currency appears in the **Currency** field.
    
    If you use the Multiple Currencies feature, select the currency you want to use for this transaction. Only the currencies set on the customer's record are available in this field. The customer's primary currency appears by default. For more information, see [Customers and Multiple Currencies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1398493.html).
    
    If you change the currency on the record, NetSuite updates prices and amounts to the currency you select.
    
7.  The exchange rate for this currency appears in the **Exchange Rate** field. You can enter a new exchange rate for this transaction, or you can update the currency's record with the exchange rate you enter here.
    
8.  In the Item column, select the item the customer is interested in, and then enter the quantity and other information for this item.
    
    NetSuite calculates the sales amount and alternate sales amount (ASA) automatically. The ASA column appears only if you use the Alternate Sales Amount feature. For more information, see [Alternate Sales Amounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1049780.html).
    
9.  Click **Add**.
    
10.  Repeat these steps for each item.
     
11.  Click the **Relationships** subtab:
     
     1.  Select a contact in the **Contact** field.
         
     2.  In the **Decision Maker** field, select the contact associated with this customer who is responsible for approving this purchase.
         
     3.  Click **Add**.
         
     4.  Repeat these steps for each contact you want to associate with this opportunity.
         
12.  Click the **Partners** subtab.
     
     The partner associated with this customer or prospect appears in the **Partner** field. However, you can choose a different partner for this opportunity.
     
     If you use the Multi-Partner Management feature, you can associate multiple partners with this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
     
13.  Click the **Competitors** subtab.
     
     1.  In the **Name** column, select a company that's competing with yours for the deal.
         
         You can create new competitor records at Lists > Competitors.
         
     2.  Click **Add**
         
     3.  Repeat these steps for each competitor.
         
14.  Click the **Communication** subtab.
     
     1.  Create any events, tasks, or phone calls you want to associate with this opportunity.
         
     2.  On the **Files** subtab, attach any files you want to associate with this opportunity.
         
     3.  On the **User Notes** subtab, enter any internal notes related to this opportunity.
         
15.  Click the **Sales** subtab.
     
     1.  The lead source associated with this customer or prospect appears in the **Lead Source** field. However, you can select a different lead source.
         
     2.  Associate sales reps with this transaction in one of the following ways:
         
         -   If you don't use the Team Selling feature, select the sales rep or sales group in the **Sales Rep** field.
             
             The sales rep or sales group associated with the customer on this transaction appears by default.
             
         -   If you use the Team Selling feature, click the **Sales Team** subtab.
             
             Select the sales team for this transaction. For more information, see [Associating Sales Teams with Customers and Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1038639.html).
             
     3.  On the **Qualification** subtab, enter information about the customer's ability and interest in making the purchase. For more information, see [Lead Qualification](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1086481.html).
         
16.  Click **Save**.
     

After you save an opportunity record you can attach tasks, events, and other information related it. You can also create estimates, sales orders, cash sales, and invoices to associate with the opportunity.

If you use the inline Edit feature, you can also edit opportunity records from the Opportunities list page. Click the information you want to change and make your changes. NetSuite automatically saves your changes on the opportunity record. For more information about editing inline, see [Using Inline Editing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495192.html).

As you work with opportunities, you can refine the projected total of the deal. You can add or remove items, and change the probability, status, and competitors for the deal. For more information about opportunity records, see [Using Opportunities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1067079.html).

Open opportunities appear on sales forecast reports, open opportunities reports, and sales forecast by quota reports.

### Related Topics

-   [Sales Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1045230.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
