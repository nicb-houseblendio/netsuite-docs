---
id: "section_N1772949"
type: "section"
title: "Creating Amortization Templates"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Amortization Templates > Creating Amortization Templates"
parent: "section_N1767815"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html"
anchors: ["procedure_N1772985"]
sha256: "f94ec8ef0b11ee33f50952566e46ceaf08e4155cfa43984d92c02f920494999c"
---

An amortization template defines the terms of the amortization schedule created by the purchase of an item. For information about the fields in an amortization schedule, see [Viewing an Amortization Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776675.html).

For details and examples of the choices available for templates, see [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html).

The Lists permission Amortization Schedules controls access to amortization templates. For more information, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).

#### To define an amortization template: {#procedure_N1772985}

1.  Go to Lists > Accounting > Amortization Templates > New.
    
2.  On the Amortization Template page, in the **Name** field, enter a name for this template.
    
    For example, you could name a template **12 Month, Equal Distribution**.
    
3.  In the **Type** field, select the kind of template you're creating: **Standard** (used for most templates) or **Variable** (used for percent-complete recognition when the Project Management feature is enabled).
    
4.  In the **Method** field, select a method to set the terms to post the expense from the net purchase amount.
    
    -   For descriptions of the available methods, see [Amortization Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html#bridgehead_N1768215).
        
    -   For examples of how straight-line methods work, see [Straight-Line Amortization Method Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1771014.html).
        
    -   If you select **Custom**, you must manually specify accounts, posting periods, and amounts in the columns at the bottom of the page.
        
        1.  **Account** - select the target expense account to which you want to post deferred expenses.
            
        2.  **Period Offset** - specify the number of periods to postpone the start of the amortization schedule for this line. The first period to amortize has an offset of zero.
            
        3.  **Amount** - enter the expense amount to recognize, either as a percentage or a currency value.
            
        4.  Click **Add**.
            
        5.  Repeat these substeps to define additional terms for this custom method.
            
        
        These fields are accessible only if you select **Custom** in the **Method** field.
        
5.  Select a **Term Source** to control how the amortization period is determined.
    
    For information about the choices for **Term Source**, see [Amortization Term Source](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html#bridgehead_N1768391).
    
6.  Check the **Use Transaction Currency** box if you want to use the foreign currency of a transaction, not your base currency, to generate the amounts on the amortization schedule. This box is part of foreign currency amortization and is available only in NetSuite U.K. editions.
    
    For information about foreign currency amortization, see [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html).
    
7.  In the **Deferral Account** field, select a Deferred Expense type account for posting.
    
    Deferral accounts also can be specified in item and expense account records. See [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html).
    
8.  In the **Contra Account** field, select the account that accumulates amortized balances. This account is most often used for depreciation schedules.
    
9.  In the **Target Account** field, select the account where the expense is amortized over time. Select **Default** to use the expense account indicated on either the transaction or item record.
    
10.  In the **Amortization Period** field, enter the number of periods over which the amount should be amortized. For example, you can enter **60** to amortize the amount over 60 periods starting from the amortization start date.
     
     For examples of how the amortization period value works, see [Amortization Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html#bridgehead_N1768528).
     
11.  Optionally, enter the number of accounting periods to delay the start of amortization after the schedule start date. You can enter the following types of offsets:
     
     -   **Period Offset** moves the entire amortization period ahead by **x** number of periods, keeping the same number of periods, so that the end date is moved forward.
         
         For example, if the schedule dates are 1/1/06 to 6/1/06 with month-long periods and a period offset of **2**, recognition starts on 3/1/06 and continues until 8/1/06.
         
     -   **Start Offset** delays the beginning of amortization. This changes the number of periods and keeps the same end date.
         
         For example, if the schedule dates are 1/1/06 to 6/1/06 with month-long periods and a start offset of **2**, recognition starts on 3/1/06 and continues until 6/1/06.
         
     
     Setting a period offset doesn't change the number of periods in the schedule. Setting a start offset changes the number of periods in the schedule because it postpones the beginning but doesn't change the final period of the schedule.
     
     For more information, see [Amortization Period Offset and Start Offset](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html#bridgehead_N1768558).
     
12.  In the **Residual** field, enter an amount or percentage to remain in the deferral account and not be amortized. A residual amount generally represents the salvage value of a fixed asset.
     
     A residual amount entered on a transaction overrides a residual amount entered on an item record.
     
13.  In the **Initial Amount** field, enter a percentage or amount to be recognized in the first recognition period. The remaining amount is then recognized according to the set recognition method.
     
     For more information, see [Amortization Initial Amount](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html#bridgehead_N1770687).
     
14.  Check the **Inactive** box to inactivate the template. Inactivated templates are saved but don't appear in lists or as choices in your account.
     
     To view inactivated templates or reactivate them, go to Lists > Accounting > Amortization Templates, and check the **Show Inactives** box.
     
15.  All amortization templates are public templates which means they're available to all users, items, and expenses.
     
16.  Click **Save**.
     

Now, this template can be used to defer expenses by associating the template with an item you purchase. This can be done on an item record or on a purchase transaction. See [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html).

To view a list of available amortization templates, go to _Lists > Accounting > Amortization Templates_.

### Related Topics

-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Amortization Template Term Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1768001.html)
-   [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html)
-   [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
