---
id: "section_N1678834"
type: "section"
title: "Setting Revenue Recognition Accounting Preferences"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Revenue Recognition > Setting Up the Revenue Recognition Feature > Setting Revenue Recognition Accounting Preferences"
parent: "section_N1678353"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678834.html"
anchors: ["procedure_N1678930"]
sha256: "3ee24d4b17dae8359638c19e68874cdd675e38c690b4dad56565b334c0eddd52"
---

Note:

This topic applies to the Revenue Recognition feature. Revenue Recognition is the key feature of NetSuite classic revenue recognition. Classic revenue recognition features aren't available in new NetSuite implementations. Classic revenue recognition (also called legacy revenue recognition) is still supported for customers who previously enabled it. NetSuite currently offers the Advanced Revenue Management (Essentials) feature to automate revenue deferral and recognition. For the equivalent information for Advanced Revenue Management (Essentials), see [Setting Advanced Revenue Management (Essentials) Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4331941758.html).

The following preferences are available when you enable the Revenue Recognition feature:

-   **Create Revenue Recognition Journals in GL** - Choose how revenue recognition journal entries are posted:
    
    -   **Detail** - A separate journal entry is created for each revenue recognition schedule.
        
    -   **Summary** - Revenue recognition schedules are summarized for posting. The summaries are based on matching attributes. For details, see [Using Summarized Revenue Recognition Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4041530082.html).
        
-   **Default Revenue Recognition Journal Date to** - Select the default transaction date of revenue recognition journal entries when you open the Create Revenue Recognition Journal Entries page.
    
    -   **Last Day of Period** - The date defaults to the last day of the period you select in the Posting period field.
        
    -   **Current Date** - The date defaults to the current date.
        
-   **Use System Percentage of Completion For Schedules** - Check this box to calculate project completion automatically, based on approved time logged against the project. To override the automatic calculation, enter a value in the Rev Rec Override Percent Complete field on the Financial subtab of the project. For more information, see [Using Percent-Complete Revenue Recognition for Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1694795.html)
    
    If you clear this box, you must enter the percentage of project completion manually for revenue recognition on project records in the Rev Rec Override Percent Complete field. The value in this field can differ from the value in the system-calculated Percent Time Complete field.
    
-   **Allow Users to Modify Revenue Recognition Schedule** - Check this box to permit changes to be made to existing standard revenue recognition schedules. You can change the revenue recognition amount on a schedule only by changing the schedule to generate the new amount. You can't modify variable revenue recognition schedules.
    
    If you prefer that revenue recognition schedules can't be changed after they're created, disable this preference.
    
    Note:
    
    The schedule amount **must always equal** the line amount. You can only change amounts that haven't been recognized.
    
-   **Prorate Revenue Recognition Dates for Partially Billed Sales Orders** - This preference applies only to revenue recognition schedules that have Rev Rec Date Specified on Sales Order as the Term Source. The preference affects only the revenue recognition start and end dates for the invoices. Amounts and periods on the revenue recognition schedules aren't affected.
    
    Check the box to divide the period established by the sales order revenue recognition start and end dates proportionally for each partial invoice. This is the default.
    
    Clear the box to use the same revenue recognition start and end dates for each invoice as the start and end dates on the sales order.
    
-   **Adv. Billing: Use Sales Order Amount** - Use this preference to determine the source of the revenue amount when billing schedules and variable revenue recognition schedules are used.
    
    Check this box to recognize revenue based on the percent complete in relation to the sales order. For example, if the sales order amount is $1,000, the invoice amount is $500 and the project is 50% complete, then 50% of the sales order amount is recognized ($500).
    
    Clear this box to recognize revenue based on the invoice amount. For example, if the sales order amount is $1,000, the invoice amount is $500 and the project is 50% complete, then 50% of the invoice amount is recognized ($250).
    

Depending on the other revenue features enabled, additional revenue recognition preferences may be available. For more information, see [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html).

#### To set revenue recognition accounting preferences: {#procedure_N1678930}

1.  Go to _Setup > Accounting > Preferences > Accounting Preferences_.
    
2.  Click the **General** subtab, and scroll down to the Revenue Recognition and Classic Revenue Recognition Only sections of the page.
    
    When the Automated Intercompany Management feature is also enabled, the **Items/Transactions** subtab includes the accounting preference **Default Intercompany Deferred Revenue Account**. For information about this preference, see [Items/Transactions Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1387022.html).
    
3.  Set preferences as desired, and click **Save**.
    

### Related Topics

-   [Setting Up the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678353.html)
-   [Enabling the Revenue Recognition Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1678611.html)
-   [Enabling Auto-Numbered Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679074.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [General Accounting Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1385293.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
