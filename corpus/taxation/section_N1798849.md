---
id: "section_N1798849"
type: "section"
title: "Closing Tax Periods"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > Working with Tax Periods > Closing Tax Periods"
parent: "section_N1797157"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1798849.html"
anchors: ["procedure_N1798876", "bridgehead_N1798910", "procedure_N1798922"]
sha256: "63c7c3b6608a78370025d6dfcd293d1f3901afe341d9a9808355a35d9df8208f"
---

To prevent posting to tax periods that have already been filed, you should close the tax periods for which you intend to generate a tax report.

Closing a tax period closes all prior tax periods. Opening a tax period also opens all the subsequent tax periods that have been set up.

#### To close a tax reporting period if you don't have a OneWorld account: {#procedure_N1798876}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click the Status icon of the posting period that you want to close.
    
3.  Click **Close Period**.
    

## Closing Tax Periods Per Subsidiary {#bridgehead_N1798910}

If you're using OneWorld (either with or without the Multiple Calendars feature enabled), you can close tax periods for some subsidiaries, and leave them open for other subsidiaries. The **Note** subtab on the Close Tax Period page shows a history of when the period was closed or reopened, and for which subsidiaries.

Closing a tax period for a subsidiary closes prior tax periods for that subsidiary. To reopen a subsidiary's closed tax period, clear the **Close** box of the subsidiary. Opening a tax period for a subsidiary opens subsequent tax periods that have been set up for that subsidiary.

The Manage Tax Periods page displays the following icons to indicate the status of the tax period:

-   ![Open icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/taxperiod_open.png) Open - The tax period is open for all subsidiaries.
    
-   ![In Progress icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/taxperiod_someclosed.png) In progress - The tax period is closed for one or more subsidiaries. Position your mouse pointer over the icon to see the number subsidiaries that have closed this tax period.
    
-   ![Closed icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/Taxation/LegacyTax/taxperiod_closed.png) Closed - The tax period is closed for all subsidiaries.
    

#### To close tax periods per subsidiary: {#procedure_N1798922}

1.  Go to Setup > Accounting > Taxes > Manage Tax Periods.
    
2.  Click the Status icon of the posting period that you want to close.
    
3.  On the Close Tax Period page, select the subsidiaries that this closed tax period applies to.
    
4.  Click **Submit**.
    

### Related Topics

-   [Working with Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797157.html)
-   [Tax Periods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4454154841.html)
-   [Setting Up Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1797599.html)
-   [Editing and Deleting Tax Periods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799174.html)
-   [Assigning a Tax Fiscal Calendar to a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799451.html)
-   [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html)
-   [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html)
-   [Reporting by Tax Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1803024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
