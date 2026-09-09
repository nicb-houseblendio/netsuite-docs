---
id: "section_N1458877"
type: "section"
title: "Running Reports for Subsidiaries with Different Accounting Periods"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Accounting Period Management > Reporting by Accounting Period > Running Reports for Subsidiaries with Different Accounting Periods"
parent: "section_N1458661"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458877.html"
anchors: ["bridgehead_N1458893", "bridgehead_N1459026", "procedure_N1459039"]
sha256: "bb4b2c920016095dc521ac6e07534ee233196a504de6c0723eabacdb20fc80c9"
---

## Running Reports for Subsidiaries without Multiple Calendars {#bridgehead_N1458893}

In NetSuite OneWorld, different subsidiaries may use different fiscal periods. In these cases, accounting periods are usually set up to map to the root parent subsidiary's calendar, so that consolidated reports that report by period fit the internal management reporting calendar.

These default reporting periods may not meet the fiscal reporting requirements for lower level subsidiaries that use different fiscal periods from the root parent subsidiary. When you run these subsidiaries' reports, you can select **Custom** in the **Period** list, and select beginning and ending periods that correspond to the range you need, or for reports such as the Balance Sheet, the **As of** period you need.

If none of the listed periods fit a subsidiary's date requirements, you can change the Report by Period preference, at _Home > Set Preferences_ on the **Analytics** subtab, to **Never**. Rerun the report, select **Custom** in the **Date** list, and enter the exact beginning and ending dates, or **As of** date that you need.

If further modifications are needed to meet reporting requirements for a subsidiary, you can use the Financial Report Builder to create customized financial statements for individual subsidiaries. For more information, see [Financial Report Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2105415.html). For reports other than financial statements, you can use the Report Builder for customization. For more information, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).

Note:

By default, each report displays data for the top-level, or root-parent, subsidiary. Select from the **Subsidiary Context** list to display data for the subsidiary you want. See [Subsidiary Context for a Financial Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2123544.html).

## Running Reports for Subsidiaries with Multiple Calendars {#bridgehead_N1459026}

With Multiple Calendars feature enabled, you can have more than one fiscal calendar to roll up accounting periods for reporting purposes.

#### To view a report using the accounting period rollup for a subsidiary: {#procedure_N1459039}

1.  Select a subsidiary on the footer for a report.
    
2.  Select an option for **Period** or **Date**, depending on the type of report you're running and your **Report by Period** preference.
    

The dates for the report range selected are based on the accounting period rollup in the context the fiscal calendar assigned to the subsidiary.

For consolidated reporting, when you run reports for a single subsidiary, the associated fiscal calendar applies. When you run a report at the consolidated level, the fiscal calendar associated with the highest level consolidated subsidiary determines the accounting period hierarchy.

### Related Topics

-   [Reporting by Accounting Period](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1458661.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
