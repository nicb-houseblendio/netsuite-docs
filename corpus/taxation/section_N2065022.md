---
id: "section_N2065022"
type: "section"
title: "Formatting Dates and Numbers for VAT Reports"
branch: "taxation"
category: "accounting"
breadcrumb: "Accounting > Taxation > Legacy Tax > VAT and GST Reporting > VAT/GST Reports > Generating VAT/GST Reports > Formatting Dates and Numbers for VAT Reports"
parent: "section_N2064551"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065022.html"
anchors: ["procedure_N2065049"]
sha256: "57573b6a9ea311ea725b6dddd8210b313071c25a49063ffb7bb1155a13de1e39"
---

For each nexus linked to your subsidiaries, define how dates and numbers are displayed on VAT reports. The formats that you set up apply to the VAT form, PDF, and drilldown reports. Note that Microsoft Excel follows your computer's regional settings, not your browser. Your computer's regional settings control how numbers, dates, and currencies are displayed in Excel.

If you have a OneWorld account, all amounts are reported in the base currency of the subsidiary. If you don't have a OneWorld account, amounts are reported based on the currency in the Company Information page. The applicable currency symbol is shown on the PDF, drilldown report, and Excel file.

The Formatting setup page for dates and numbers can be accessed from the VAT report page at Reports > VAT/GST > Tax Reports (International).

Anyone who has access to the VAT report page for a particular nexus can set up the date and number formats for that nexus. When set, the formats apply to all VAT reports of that nexus, regardless of subsidiary.

If you haven't set up the formats for the VAT dates and numbers, NetSuite uses the logged in user's preferences for date, long date, number, negative number, and reporting period defined on the following preference pages:

-   For NetSuite accounts without OneWorld, go to Setup > Company > General Preferences.
    
-   For NetSuite OneWorld accounts, it is found in the Preferences subtab of the subsidiary record. Go to Setup > Company > Subsidiaries.
    

#### To set up date and number formatting for a VAT report: {#procedure_N2065049}

1.  Go to Reports > VAT/GST > Tax Reports (International).
    
2.  On the Tax Reports page, select a subsidiary.
    
3.  Select a country form.
    
4.  On the VAT form, click **Setup**, and then click **Formatting**.
    
5.  On the Formatting setup page, select the formats of the dates and numbers to display on the VAT report.
    
    1.  **Date Format** - Select a format for the short form of the date. The date appears on the Detailed Report page (drilldown report) and on the System Notes.
        
    2.  **Long Date Format** - Select a format for the long form of the date. The long date appears on the footer of the PDF.
        
    3.  **Negative Number Format** - Select a format for negative numbers.
        
    4.  **Number Format** - Select a format for numbers and decimal indicators.
        
    5.  **Use Tax Period Name** - Check this box to use the tax period names from the Tax Period fields of the VAT form. These are the period names defined in your tax period setup. If this box checked, the Reporting Period Separator, Monthly Format, Quarterly Format, and Year Format preferences are disabled.
        
    6.  **Reporting Period Separator** - Select a format for the separator between the start and end dates. The separator applies to monthly and quarterly periods.
        
    7.  **Monthly Format** - Select a format for the monthly reporting period.
        
    8.  **Quarterly Format** - Select a format for the quarterly reporting period.
        
    9.  **Year Format** - Select a format for the annual reporting period.
        
6.  Click **Save**.
    

### Related Topics:

-   [Viewing VAT Report Transaction Details](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2065235.html)
-   [Making Adjustments on a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067438.html)
-   [Flagging Tax Periods in a VAT Return](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721526384.html)
-   [Viewing the VAT Return Submission History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3721544005.html)
-   [Multi-Book Accounting for International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4108426899.html)
-   [Generating VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2064551.html)
-   [VAT/GST Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2063644.html)
-   [International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2051341.html)
-   [Automatic Tax Code Provisioning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053451.html)
-   [Electronic Tax Filing Using NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2053770.html)
-   [Setting Up Tax Filing Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2053829.html)
-   [Creating or Customizing Roles to Use the International Tax Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2054151.html)
-   [Sales and Purchase Reports Grouped by Tax Code](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2067748.html)
-   [International Tax Reports Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2072942.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
