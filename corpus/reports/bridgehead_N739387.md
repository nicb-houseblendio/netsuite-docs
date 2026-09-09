---
id: "bridgehead_N739387"
type: "bridgehead"
title: "Alternate Range Types"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Adding, Removing, or Reordering Report Columns > Adding Time-Based Comparison Columns to Reports > Alternate Range Types"
parent: "section_N739328"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N739387.html"
anchors: []
sha256: "58073cf2da79465e8e522cbd4d93ba8c615ddcecc34ac511f78959a16969340d"
---

After you add a column to a report, you can select one of the following alternate range types:

-   **Relative to report date**
    
-   -   Defined in relation to the overall date range set for the report.
        
    -   Changes when the overall report date range changes.
        
    -   Most commonly used type.
        
    -   Example: In December 2009, you add a column with an alternate date range of **last month** to a report and run it. It displays December 2009 data for most columns, and November 2009 data for the alternate date range column. When you change the report date range to January 2010, it displays January 2010 data for most columns and December 2009 data for the alternate date range column.
        
-   **Relative to today's date**
    
    -   Defined in relation to the current date when the report is run
        
    -   Does not change when the overall report date range changes.
        
    -   This type is provided for backward compatibility with the alternate date range functionality available before Version 2010 Release 1.
        
    -   Example: In December 2009, you add a column with an alternate date range of **last month** to a report and run it. It displays December 2009 data for most columns, and November 2009 data for the alternate date range column. When you change the report date range to January 2010, it displays January 2010 data for most columns and still displays November 2009 data for the alternate date range column.
        

Note:

For an alternate range that is 'to date', such as **this fiscal year to date**, you should select an alternate range type of **Relative to today's date**.

For example, define an alternate range type of **Relative to report date**. Select an alternate range such as **this fiscal year to date**. The alternate date range column uses the **From** date of the overall report range, so comparisons with other report columns are not meaningful.

### Related Topics

-   [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
