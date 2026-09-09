---
id: "section_N481482"
type: "section"
title: "Analytics Personal Preferences"
branch: "setting-personal-preferences"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Setting Personal Preferences > Analytics Personal Preferences"
parent: "chapter_N475297"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N481482.html"
anchors: []
sha256: "011529a9ff52f365cf56fdbc78194b32a97292a3f62332acdc57a7441c62d4a4"
---

In the Analytics subtab, you can set preferences such as report by period, default bank account, search, PDF orientation and font size, CSV export, and other.

Go to _Home > Set Preferences_ and click the Analytics subtab to set any of the preferences in the following table.

The following fields are available, based on the features in your NetSuite account, and the permissions associated with your NetSuite role.

| **Field Name** | **Function** |
| --- | --- |
| **Reporting** |
| Report by Period | Select what type of reports you want to view by period. **All Reports** - Select this option to view all applicable reports by period. When this option is selected, reports that support reporting by period include a period filter in the report footer. **Financials Only** - Select this option if you want specific financial reports reported by period. For a list of these financial reports, see [Report by Period: Financials Only Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3851329956.html). **Never** - Select this option if you don't want to exclude reports that can be run in both by date and by period mode. Note: When you select **Financials Only** or **Never**, you may encounter problems with data for KPI scorecards that use accounting periods. Note: In OneWorld accounts, if you post transactions with dates outside posting periods, best practice is to run all reports by period. Select **All Reports**. This option requires the Accounting Periods feature to be enabled. For details, see [Accounting Period Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1445226.html). |
| Show Reports in Grid | Check this box to show reports in the grid. |
| Customize Font on Financial Reports | Check this box to configure the font settings on custom financial reports. |
| Print Company Logo | Check this box to include your company logo on all printed reports. |
| Display Report Title on Screen | Check this box to display the report title, company name, and date or period range at the top of all reports displayed on your screen. Even when this preference isn't enabled, this title information still prints on reports. To display report title information only on selected reports, don't check this box. Instead, click Options in the footer of each report, and check the Display Title box. |
| Display Report Description | Check this box to display customization details as part of report title for all reports. These details are from the Description field in the More Options step of the Report Builder. To disable the display of customization details for selected reports, click Options in the footer of each report, and clear the Print Description box. |
| Default Bank Account | Select the bank account to use as the default account for the Bank Register listed on the Reports page and the Bank Balance snapshot on the Home page. |
| Calculate Forecasts as Weighted | Check this box to show the weighted forecast value instead of total projected forecast values on reports. You can set this preference at both _Home > Set Preferences_, and at _Setup > Sales > Sales Preferences_, on the Forecasts subtab. The setting you select for this preference on the Set Preferences page overrides the company wide setting for this preference on the Sales Preferences page. |
| **Search** |
| Show List When Only One Result | Check this box to list search results, even when there's only one result. If you clear this box and there's only one result from a search, the record or transaction automatically opens. |
| Quick Search Uses Keywords | Check this box so that the Quick Search portlet returns records with names that **start with** AND records with names that **contain** the keywords you enter. If you clear this box, the Quick Search portlet displays **Starts With** and **Contains** buttons. Searches can return records with names that start with keywords OR records with names that contain keywords, based on the button you select. |
| Popup Search Uses Keywords | You use popup searches when you type a keyword and press Tab to make a selection in a field on a transaction or form. Check this box to base search results for popup lists only on keywords that start with and include all the search terms entered. Note: Enabling this preference removes the Starts With and Contains options from the Quick Search portlet. |
| Include Inactives in Global & Quick Search | Check this box to include inactive records in results returned for keywords entered in the Search field or in the Quick Search portlet. By default, only active records and transactions are searched with these fields. |
| Popup Auto Suggest | Check this box to have NetSuite suggest matches for the text you enter in fields as you type. You can select from the list of matching records to select the record you need. |
| Global Search Auto Suggest | This box is checked by default. NetSuite suggests matches for the text you enter in the Search field, automatically as you type. You can select from the list of suggested records to go directly to the record you need. |
| Page Search | Enable the Current Page Results feature to see enhanced results in the global search. This option is enabled by default. For more information, see [Current Page Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161899349589.html#bridgehead_28162751354). |
| Global Search Sort by Name/ID | Check this box to sort global search results by name, instead of by record type and then by name within each record type. |
| Global Search Customer Prefix Includes Leads and Prospects | By default this box is cleared, and when you type the **cu** prefix in the Search field, only customer records display in search results. Check this box to display leads, prospects, and customers in your search results when you type the **cu** prefix in the Search field. |
| Global Search Includes Transaction Numbers | By default, when searching for a number in Global Search, the search results only include results by document number. When this box is checked, search results include results whose document number AND transaction number match the number searched. |
| **PDF** |
| PDF Page Orientation | Select landscape or portrait orientation for your PDF output when you export a report or search results as a PDF. |
| PDF Font Size | Select a font size for the PDF output when you choose to export a report or search results as a PDF. |
| **Export** |
| CSV Export Character Encoding | Select an alternate character encoding for CSV exports of lists, reports, and searches. Default encoding is UTF-8. Other options are Windows 1252, the default format for Microsoft Excel, and Shift-JIS, the most widely used format in Japan. |
| **KPI and Snapshot** |
| Accounting Book | If you use the Multi-Book Accounting feature, select the Accounting Book you would like to use for reporting. |
| KPI Scorecard with Period Specific Consolidation Rates | Select the accounting period that provides the consolidation rates you would like to use in the KPI Scorecard report. The period consolidation rates you choose affect these KPIs:
-   Bank Balance
-   Credit Card Balance
-   Receivables
-   Payables
-   Other Current Assets
-   Other Current Liabilities

Note: If Multi-Book Accounting is provisioned in your NetSuite OneWorld account, the accounting book selected on the user preference reflects the accounting book currency. This preference doesn't affect standard KPIs. This preference is available for all NetSuite user roles. |

### Related Topics

-   [Setting Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N475297.html)
-   [General Personal Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N475661.html)
-   [Personal Preferences for Appearance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N479574.html)
-   [Personal Preferences for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N480873.html)
-   [Personal Preferences for Activities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N482375.html)
-   [Personal Preferences for Alerts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N483440.html)
-   [Personal Preferences for Telephony](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484162.html)
-   [Personal Preferences for Restricting Views](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N484545.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
