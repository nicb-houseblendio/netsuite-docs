---
id: "section_N1780615"
type: "section"
title: "Using Percent-Complete Amortization for Projects"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Expense Amortization > Using Percent-Complete Amortization for Projects"
parent: "chapter_N1765678"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1780615.html"
anchors: ["procedure_N1780649", "bridgehead_N1780767", "procedure_N1780780", "bridgehead_N1780846", "bridgehead_N1780902"]
sha256: "cf24ad1db075bbc8fd2eb32dc09986b1ac7c2bf7c7a32215515eb09c4c2965ce"
---

If you have a projects based business, you can amortize expenses based on the percentage of completed project work by using variable amortization schedules. You can coordinate the recognition of deferred expenses with the completion of stages for your projects.

You can set up items and expense accounts to be associated with a variable amortization template and with projects you track. Then purchases of these items or expenses charged to these accounts generate amortization schedules based on the template and the linked project completion.

Note:

Variable amortization schedules don't include forecast amounts.

As time worked is logged against the project and portions of the project are marked complete, journal entries are created to recognize the related expenses.

Important:

This feature is available only if you use Project Management.

#### To amortize expenses based on project completion: {#procedure_N1780649}

1.  Enable the Amortization feature. See [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html).
    
2.  Create a variable type amortization template. See [Creating Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1772949.html).
    
3.  Associate the variable type amortization template with items and expense accounts used for the project. See [Configuration for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1773475.html), and [Associating Amortization Templates with Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1775784.html).
    

See the following topics for more details:

-   [System Percentage of Completion Preference](#bridgehead_N1780767)
    
-   [Percent-Complete Based Amortization Journal Entries](#bridgehead_N1780846)
    
-   [Variable Schedule Amortization Example](#bridgehead_N1780902)
    

## System Percentage of Completion Preference {#bridgehead_N1780767}

You can set a preference for NetSuite to automatically determine the percentage of a project that's been completed.

#### To automatically calculate the percent completion for a project: {#procedure_N1780780}

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the **General** subtab.
    
3.  Check the **Use System Percentage of Completion For Schedules** box.
    
4.  Click **Save**.
    

If you don't enable this preference, you must enter the percentage of project completion manually on project records in the Percent Complete field.

## Percent-Complete Based Amortization Journal Entries {#bridgehead_N1780846}

The Create Amortization Journal Entries page includes expense amounts due to post from variable schedules based on project completion.

For the period you select, NetSuite determines the amount due to be amortized for each schedule based on project completion. It calculates project completion based on entered and approved project time entries. The Project record shows the percentage of completion for the project in that period, and NetSuite uses that percentage to determine the expense due to post.

A variable schedule does **not** show in the list if:

-   It has a zero balance to amortize for the selected period.
    
-   It has already amortized an amount for the selected period.
    

Amortization journal entries typically credit a deferred expense account and debit an expense account. In some cases, however, a journal entry may decrease the expense recognized. In these cases, the amortization journal entries debit a deferred expense account and credit an expense account. For an example of this case, see the [Variable Schedule Amortization Example](#bridgehead_N1780902).

## Variable Schedule Amortization Example {#bridgehead_N1780902}

Variable schedules are used to amortize expenses associated with projects. Time logged against the project toward completion determines the percentage complete. Then the percent complete figure determines how much is amortized that period.

In the example below, vendor bills and payroll amounts contribute to the total cost for a project. The % Complete column shows the status of the project at the end of each period. The amount to be amortized is shown in the Amortization Period column.

| Period | % Comp. | Bills | Pay-roll | Total costs | Amortization Periods |
| --- | --- | --- | --- | --- | --- |
|  |  |  |  |  | **1** | **2** | **3** | **4** | **5** | **6** |
| 1 | 25% | 1000 | 160 | **1160** | 290 | 580 | 348 | 580 | 812 | 1160 |
| 2 | 50% | 200 | 160 | **360** | 180 | 180 | 108 | 180 | 252 | 360 |
| 3 | 30% | 300 | 160 | **460** | 138 | 230 | 138 | 230 | 322 | 460 |
| 4 | 50% | 250 | 160 | **410** | 205 | 205 | 123 | 205 | 287 | 410 |
| 5 | 70% | 230 | 200 | **430** | 301 | 215 | 129 | 215 | 301 | 430 |
| 6 | 100% | 600 | 180 | **780** | 780 | 390 | 234 | 390 | 546 | 780 |
| Total |  | **2580** | **1020** | **3600** | **1894** | **1800** | **1080** | **1800** | **2520** | **3600** |

Sometimes when projects are reassessed after they begin, the percentage complete can regress. An example of this is shown in Period 3 above, where the completion changes to 30%, down from 50% in Period 2.

To continue this example, the chart below shows the net amount, rather than the total amount, to be amortized per period.

|  | Amortization Periods | Total |
| --- | --- | --- |
|  | **1** | **2** | **3** | **4** | **5** | **6** |  |
| Amortized Balance | 290 | 580 | 348 | 580 | 812 | 1160 |  |
| Amortized Portion per Period | 290 | 290 | (232) | 232 | 232 | 348 | **1160** |
| Amortized Balance |  | 180 | 108 | 180 | 252 | 360 |  |
| Amortized Portion per Period |  | 180 | (72) | 72 | 72 | 108 | **360** |
| Amortized Balance |  |  | 138 | 230 | 322 | 460 |  |
| Amortized Portion per Period |  |  | 138 | 92 | 92 | 138 | **460** |
| Amortized Balance |  |  |  | **205** | **287** | **410** |  |
| Amortized Portion per Period |  |  |  | 205 | 82 | 123 | **410** |
| Amortized Balance |  |  |  |  | 301 | 430 |  |
| Amortized Portion per Period |  |  |  |  | 301 | 129 | **430** |
| Amortized Balance |  |  |  |  |  | 780 |  |
| Amortized Portion per Period |  |  |  |  |  | 780 | **780** |

### Related Topics

-   [Expense Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1765678.html)
-   [Setup for Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1766651.html)
-   [Amortization Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1767815.html)
-   [Amortization Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1776086.html)
-   [Amortization Journal Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1777836.html)
-   [Foreign Currency Amortization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1784814.html)
-   [Amortization Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1789982.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
