---
id: "section_N711076"
type: "section"
title: "Creating a New Report"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Reporting Overview > Ad Hoc Reports > Creating a New Report"
parent: "section_N708927"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N711076.html"
anchors: ["subsect_0412015141", "procedure_N711108", "procedure_N711147"]
sha256: "713c29ee3f0b6788efe8031e245cc255e3750a8ef6f7c77abd8aec6a0180aebd"
---

NetSuite offers a variety of standard reports that are available from the Reports page. These reports can be further customized using the Report Builder. For a list of standard reports, see [Standard Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N701428.html). To learn how to create a custom report, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).

If no standard report fits your needs, you can create a new ad hoc report. For information about ad hoc reports, see [Ad Hoc Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N708927.html).

## Creating New Reports {#subsect_0412015141}

To create an ad hoc report, you must first choose the data on which you want to report, called the metric. Then you set report criteria to choose the specific fields from which data will be calculated and the report format. For information about these choices, see [Choices for Ad Hoc Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N709168.html).

#### To select the type of data you want to report on: {#procedure_N711108}

1.  On the Reports page or Reports tab menu, click New Report.
    
2.  On the New Report list, select the Metric on which you want to report.
    
    After you select the metric you want to report on, you are taken to a page with criteria specific to that metric. For example, if you choose to report on Forecast data, you are taken to a page entitled "New Forecast Report" that contains criteria related to forecast data only.
    

#### To set the criteria for your report: {#procedure_N711147}

1.  In the **Report Title** field, a default title appears. This default title is based on the metric you chose and the default format.
    
    For example, if you chose to report on Forecast data, the default title is Custom Forecast Summary.
    
    Note:
    
    You can enter a custom title in this field but after you make any changes to this field (entering a custom description, adding or removing a space, etc.), it is no longer updated automatically.
    
2.  The criteria on this page are broken down into the following steps:
    
    -   **Step 1: Select the field you want to report on**
        
        This list of fields contains only fields associated with the type of data you chose to report on. For example, if you clicked Forecast on the New Report page, the list of fields contains only fields associated with forecast transactions.
        
    -   **Step 2: Select the format of the report**
        
        You can choose to create a summary, detail or matrix report.
        
    -   **Step 3: Select how you want to subtotal the report**
        
        Select the field you want to subtotal your report by. For example, if you want to see your forecast grouped by location, select Location as the component and **Name** as the field.
        
    -   **Step 4** : **Select how you want to summarize the data across columns**
        
        This step appears only if you chose to build a matrix report. You can then choose to view your matrix report divided into multiple columns based on the column you select. The report will then be summarized by that column across all columns. For example, if you are building a report based on forecast data and you want to view monthly forecast totals, select Month in the **Column** field. Your report will then have a column listed for each month for the date range selected in the footer.
        
    
    For more information about these criteria choices, see [To Choose Report Title, Field, Format, Subtotal Grouping, and Matrix Column](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160700524893.html#procedure_N710682).
    
3.  When you've selected all criteria, you can:
    
    -   Click Run Report to view the results of your new report. You can then use the options in the footer to further customize your report. For more information, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).
        
    -   Click Save to both run the report and save the report. You can access the saved report by going to _Reports > Saved Reports > All Saved Reports_.
        
    -   Click More Customization to display the Report Builder, where you can add more filters and sorting options, reorder or add columns to your ad hoc report, or choose display options for your report. For more information, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).
        
    
    After you run your report, you can modify report formatting by selecting options in the report's footer. For information, see [Setting Report Footer Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N720025.html). You can also click the Customize button in the footer of the report to access the Report Builder.
    

### Related Topics

-   [Ad Hoc Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N708927.html)
-   [Choices for Ad Hoc Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N709168.html)
-   [Example Ad Hoc Report Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N710892.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
