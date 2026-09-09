---
id: "section_N1446183"
type: "section"
title: "Setting Up Accounting Periods for a Year"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Accounting Period Setup > Setting Up Accounting Periods for a Year"
parent: "section_N1445585"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446183.html"
anchors: ["procedure_N1446207"]
sha256: "635e2dcdd2f6bb8d9c810a19f829d0ad094870c0bc4980bbdd257de8625ce40c"
---

You have the option of setting up a single accounting period at a time or generating all periods for a full year using the Set Up Full Year button. Best practice recommendation is to use Set Up Full Year to generate all periods and the rollup hierarchy for a full year. You must have at least **Edit** level of the **Manage Accounting Periods** permission to set up accounting periods.

Important:

Each day must belong to an accounting period to ensure accuracy in reporting.

#### To set up periods for a full year at a time: {#procedure_N1446207}

1.  Go to _Setup > Accounting > Manage G/L > Manage Accounting Periods_.
    
2.  On the Manage Accounting Periods page, click **Set Up Full Year**.
    
    The Accounting Periods for Full Year page appears.
    
3.  In the **First Fiscal Month** field, select the month your fiscal year starts.
    
    Example: **July**
    
4.  In the **Fiscal Year End** field, enter or accept the four-digit fiscal year for which you want to generate accounting periods.
    
    For example, if you were generating periods for 2013 you would enter 2013 in this field.
    
5.  Select the format you want to use for your accounting periods:
    
    -   **Calendar Months** - This sets up 12 periods, one for each calendar month in the fiscal year.
        
    -   **4 Weeks** - This sets up 13 periods, each for every 4 weeks in the fiscal year.
        
    -   **4-4-5 Weeks** - This sets up a fiscal year so that you have two 4-week periods followed by one 5-week period, repeating this cycle four times for a total of 13 periods in a fiscal year. The first accounting period of the year is from January 1 to January 28, regardless of the day of the week on which January 1 falls. The last accounting period of the year ends on December 31. The behavior is similar when the first period of the year is a different month. For example, when the year begins April 1, the first period ends April 28, and the year ends March 31. Used this way, the 4-4-5 periods shift the ending day of the week from year to year.
        
6.  In the **Year in Period Name** field, select the starting or ending year to include in the period name.
    
    For example, if a fiscal year starts in 2014 and ends in 2015, selecting **Ending Year of Period** would include 2015 in the name of the period.
    
7.  Check **One-Day Year-End Adj. Period** if you want to include a standalone adjustment period for last day of this fiscal year.
    
8.  Click **Save**.
    

For information about managing tax periods, see [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html).

Note:

If you create an accounting period that precedes a locked period, the new period you create is locked upon creation. For example, you have created an accounting period for fiscal year 2013. The period is closed and locked. You have transactions to enter for fiscal year 2012, so you create an accounting period for that fiscal year. When you save the new period, it's saved locked to prevent mismatches and accidental general ledger impact in the periods that follow. You must manually unlock A/R and A/P in each period to enter the transactions.

The Manage Accounting Periods page shows the fiscal period created for the year. To edit a period, click the period name in the list of periods. See [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html).

### Related Topics

-   [Accounting Period Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445585.html)
-   [Manage Accounting Periods Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1445839.html)
-   [Setting Up Single Accounting Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446470.html)
-   [Editing an Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1446881.html)
-   [Accounting Period Deletion Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1448709.html)
-   [Viewing the Status of Accounting Period Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
