---
id: "section_N630437"
type: "section"
title: "Creating Custom Report Snapshots"
branch: "dashboards"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Dashboards > Report Snapshots > Adding a Report Snapshot Portlet > Creating Custom Report Snapshots"
parent: "section_N626371"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630437.html"
anchors: ["procedure_N630471"]
sha256: "4a8b1e765398d96badbe4944fdacb0ca45c9b7c3055810812fe52ce35b005f39"
---

If standard report snapshots aren't providing the information that you need, you can create custom report snapshots to be displayed in dashboard portlets. To create a custom snapshot, customize a standard report that currently generates snapshots, and create a snapshot of the customized report when you run the report.

You can create custom report snapshots only from reports that currently are used to generate standard report snapshots. For a list of these reports, see [Reports Available for Custom Report Snapshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630892.html).

#### To create a custom report snapshot: {#procedure_N630471}

1.  Open the report you want to customize.
    
    For a list of reports you can use, see [Reports Available for Custom Report Snapshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630892.html).
    
    -   Go to Reports > Reports Overview, find the report to customize, point to it and click **Customize** next to its name.
        
    -   If the report is displayed in a report snapshot portlet, click **View Report** in the portlet's menu, and then click **Customize** in the report's footer area.
        
2.  Use the Report Builder to customize the report.
    
    For information about how to customize a report, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).
    
    Important:
    
    By default, when users click a custom report snapshot link to view detailed data, drilldown goes to the standard detail report, not to a customized detail report.
    
3.  Click **Save** or **Run Report**.
    
4.  On the report results page, click the **Create Snapshot** icon ![Create Report Snapshot icon](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Dashboards/create_report_snapshot_icon.png).
    
    Note:
    
    The **Create Snapshot** icon is always visible, but is only enabled for custom reports that display results data.
    
5.  On the Customize Report Snapshot page, define layout options for portlets displaying this custom report snapshot.
    
    1.  Enter a **Portlet Title** that will be displayed in the header bar of this snapshot's portlet.
        
        The title must be unique.
        
    2.  On the **List** subtab, select at least two columns you want to display for each version of the portlet, narrow and wide, by checking the box next to each label name.
        
        The narrow version of the portlet can display only two columns.
        
        The wide version shows only when the portlet is positioned in the center column of the dashboard. For more information about dashboard columns, see [Dashboard Layouts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4072488196.html).
        
    3.  On the **Graph** subtab, select the columns of data to show in the graph's X and Y axes.
        
6.  Click **Save**.
    

This snapshot is now available for you to add to a dashboard portlet. For more information about adding and setting up the portlet, see the following topics:

-   [Adding a Report Snapshot Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N626371.html)
    
-   [Setting Up a Report Snapshot Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N632502.html)
    

When a custom snapshot is displayed in a portlet, you can click **Edit** to make changes.

Note:

If you receive the error message 'This record already exists' when you click **Save**, it means there's a previously created custom snapshot that has the same name. You can change your report snapshot title or delete the previously created snapshot. See [Deleting a Custom Report Snapshot from a Report Snapshot Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630756.html).

### Related Topics

-   [Adding a Report Snapshot Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N626371.html)
-   [Standard Report Snapshots Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N626685.html)
-   [Setup Options for Comparative Sales Report Snapshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N629979.html)
-   [Deleting a Custom Report Snapshot from a Report Snapshot Portlet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630756.html)
-   [Reports Available for Custom Report Snapshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N630892.html)
-   [Sales Management Snapshots](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N631397.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
