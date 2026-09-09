---
id: "section_N1686978"
type: "section"
title: "Defining a Revenue Recognition Template"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Creating Revenue Recognition Templates > Defining a Revenue Recognition Template"
parent: "section_N1679446"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1686978.html"
anchors: ["procedure_N1686998"]
sha256: "f3e9f55ea3ea4d6350b68568815e68394b4dadb53a14e3fdb8cc96fe753a6ddc"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For the equivalent information for Advanced Revenue Management (Essentials), see [Defining a Revenue Recognition Rule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4356114812.html).

A revenue recognition template defines the terms of the revenue recognition schedule created by the sale of an item.

#### To define a revenue recognition template: {#procedure_N1686998}

1.  Go to _Lists > Accounting > Revenue Recognition Templates > New_.
    
2.  On the New Revenue Recognition Template page, in the **Name** field, enter a name for this template.
    
    For example, you could name a template **12 Month, Equal Distribution**.
    
3.  In the **Type** field, select the kind of template you're creating.
    
    -   **Standard** - select for most templates
        
    -   **Variable** - select for percent-complete recognition when the Project Management feature is enabled. You can't set **Method**, **Term Source**, **Recognition Period**, **Period Offset**, **Start Offset**, and **Initial Amount** for Variable templates. You can save the template at this point or skip to Step 9.
        
        For information about variable revenue recognition schedules, see [Working with Variable Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3791187429.html).
        
4.  In the **Method** field, choose a method to set the terms to post income from the net sales amount.
    
    -   For descriptions of the available methods, see [Revenue Recognition Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1679836).
        
    -   For examples of how straight-line methods work, see [Straight-Line Revenue Recognition Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html).
        
    -   If you select **Custom**, you must manually specify accounts, posting periods and amounts in the columns in the lower portion of the page. Make sure the currency on the account matches the intended transaction currency.
        
        1.  **Account** - select the income account you want to post deferred revenue into.
            
        2.  **Period Offset** - specify the number of periods to postpone the start of the recognition schedule for this line. The first period to recognize has an offset of zero.
            
        3.  **Amount** - enter the revenue amount to recognize, as a percentage or a currency value.
            
        4.  Click **Add**.
            
        5.  Repeat steps above to define additional terms for this custom method.
            
        
        These fields are available only if you select **Custom** in the **Method** field.
        
5.  Select a **Term Source** to control how the recognition period is determined.
    
    For information about the choices for **Term Source**, see [Revenue Recognition Term Source](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1680012).
    
6.  In the **Recognition Period** field, enter the number of accounting periods over which the schedule will recognize revenue. For example, if you enter **12**, then the schedule runs for 12 periods starting from the Rev Rec Start Date.
    
    For examples of how the recognition period value works, see [Revenue Recognition Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683147).
    
7.  Optionally, enter the number of accounting periods to delay the start of recognition after the schedule start date. You can enter the following types of offsets:
    
    -   **Period Offset** moves the entire recognition period ahead by **x** number of periods, keeping the same number of periods, so that the end date is moved forward.
        
        For example, if the schedule dates are 1/1/06 to 6/1/06, with month-long periods and a period offset of **2**, recognition starts on 3/1/06 and continues until 8/1/06.
        
    -   **Start Offset** delays the beginning of recognition, changing the number of periods, and keeping the same end date.
        
        For example, if the schedule dates are 1/1/06 to 6/1/06, with month-long periods and a start offset of **2**, recognition starts on 3/1/06 and continues until 6/1/06.
        
    
    Setting a period offset doesn't change the number of periods in the schedule. Setting a start offset changes the number of periods in the schedule because it postpones the beginning, but doesn't change the final period of the schedule.
    
    For more information and examples, see [Revenue Recognition Period Offset and Start Offset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683393).
    
8.  In the **Initial Amount** field, enter a percentage or amount to be recognized in the first recognition period. The remaining amount is then recognized according to the set recognition method. This field isn't available for Variable templates.
    
    For more information, see [Revenue Recognition Initial Amount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html#bridgehead_N1683713).
    
9.  Check the **Public** box to make the template available to other users.
    
10.  Check the **Inactive** box to inactivate the template. Inactivated templates are saved, but don't appear in lists or as choices in your account.
     
     To view inactivated templates or reactivate them, go to _Lists > Accounting > Revenue Recognition Templates_, and check the **Show Inactives** box.
     
11.  Click **Save**.
     

Now this template can be used to defer revenue by associating the template with an item you sell. This can be done on an item record or on a sales transaction. See [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html).

Revenue recognition templates can be edited. If you change any of the values in a revenue recognition template, all **future** revenue recognition schedules created from the template use the new values. Existing revenue recognition schedules created from the template aren't affected. The best practice is to create a new revenue recognition template instead of editing an existing template after it has been used.

To view a list of available revenue recognition templates, go to _Lists > Accounting > Revenue Recognition Templates_.

### Related Topics

-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Understanding Revenue Recognition Template Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html)
-   [Straight-Line Revenue Recognition Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1684020.html)
-   [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
