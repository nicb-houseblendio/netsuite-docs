---
id: "bridgehead_N1449653"
type: "bridgehead"
title: "Editing a Fiscal Calendar"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Fiscal Calendars > Creating a Fiscal Calendar > Editing a Fiscal Calendar"
parent: "section_N1449559"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449653.html"
anchors: ["procedure_N1449704"]
sha256: "d1a3cb5da2f715f36c13638dfe40f9cefa6a6a5f6864971348fd8e02ee8d1cb5"
---

You can change the name and first month for a fiscal calendar. Changing the first month doesn't change any existing accounting period rollups created for the fiscal calendar. This means you can edit a fiscal calendar record to create tax years and accounting years for a subsidiary that begin on different dates. For example, the fiscal year for a Subsidiary A runs from July 1 to June 30, but tax report filings are filed based on the calendar year, January to December. Because you can assign only one fiscal calendar to a subsidiary, you can set up the accounting period hierarchy first with the First Fiscal Month of the fiscal calendar set to July. Then edit the fiscal calendar and set the First Fiscal Month to January. Use Set Up Full Year to generate tax periods and their rollup as needed. Remember to change the fiscal calendar record accordingly before you use Set Up Full Year. For information about tax periods, see [Setting Up Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1799689.html) and [Setting Up Historical and Transitional Tax Periods Using a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1800348.html).

#### To edit a fiscal calendar: {#procedure_N1449704}

1.  Go to _Setup > Accounting > Manage G/L > Fiscal Calendars_.
    
2.  On the Fiscal Calendars page, select the calendar you want to change.
    
3.  Click **Edit** and make your changes.
    
    Note:
    
    The **Subsidiaries** field lists the subsidiaries that use this fiscal calendar to roll up accounting periods and tax periods. The **Tax Calendar Subsidiaries** field lists the subsidiaries that share this tax calendar.
    
    If you change the setting for **Default Fiscal Calendar**, the change applies only to the new subsidiaries you create.
    
4.  Click **Save**.
    

### Related Topics

-   [Creating a Fiscal Calendar](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1449559.html)
-   [Assigning Fiscal Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449741.html)
-   [Moving Subsidiaries to a New Fiscal Year](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1449790.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
