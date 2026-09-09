---
id: "section_N1767069"
type: "section"
title: "Setting Amortization Preferences"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Setup for Amortization > Setting Amortization Preferences"
parent: "section_N1766651"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767069.html"
anchors: ["procedure_N1767088"]
sha256: "249256377fa921653923bb9e4cf2f67c8aad5da07f6eeb7a6be4dd1c885684ff"
---

After the Amortization feature has been enabled, you can set amortization preferences.

#### To set the amortization accounting preferences: {#procedure_N1767088}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the General subtab.
    
3.  Set the following preferences as desired:
    
    In the Revenue Recognition section:
    
    -   **Use System Percentage of Completion For Schedules** - Check this box to calculate project completion automatically, based on approved time logged against the project. To override the automatic calculation, enter a value in the Rev Rec Override Percent Complete field on the Financial subtab of the project.
        
        If you clear this box, you must enter the percentage of project completion for amortization manually on project records in the Rev Rec Override Percent Complete field. The value in this field can be different from the value in the system-calculated Percent Time Complete field.
        
    
    In the Amortization section:
    
    -   **Allow Users to Modify Amortization Schedule** - Check this box to allow changes in the total amount on an amortization schedule after it's initially created. The total amount of the schedule must always equal the purchase amount of the related line item. Only amounts that have not yet been recognized can be changed.
        
        Clear this box if you prefer that amortization schedules not be changed after they're created.
        
    -   **Allow Foreign Currency Amortization Schedules** - (Available only in NetSuite U.K. editions) Check this box to be able to create amortization schedules using the foreign currency amounts instead of base currency amounts. For information about foreign currency amortization, see [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html).
        
    -   **Default Amortization Journal Date To** - Set the default posting date of amortization journal entries on the Create Amortization Journal Entries page as follows:
        
        -   **Last Day of Period** - The date defaults to the last day of the period you select in the Posting Period field.
            
        -   **Current Date** - The date defaults to the current date.
            
        
        **Default Amortization Journal Entry Form** - Select the journal entry form to use for amortization journal entries. The options are Standard Journal Entry plus any custom journal entry forms created during implementation.
        
    -   **Number of Short-Term Expense Periods** - Enter the number of short-term expense periods to include in the Deferred Expense Waterfall report. Integers from 0 through 52 inclusive are valid values. The default is 12.
        
4.  Click **Save**.
    

### Related Topics

-   [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html)
-   [Enabling the Amortization Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766842.html)
-   [Enabling Auto-Numbered Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767306.html)
-   [Specifying Deferral Accounts for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767540.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
