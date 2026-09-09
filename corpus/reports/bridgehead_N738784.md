---
id: "bridgehead_N738784"
type: "bridgehead"
title: "Adding Report Columns"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Report Customization > Adding, Removing, or Reordering Report Columns > Adding Report Columns"
parent: "section_N738669"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N738784.html"
anchors: ["bridgehead_N738794", "bridgehead_4078557215", "bridgehead_3830033769"]
sha256: "339084b3032480f0188277f00a345b6a309c6d2ebe1e3bf0da0a7a76e2472a80"
---

Before you add a new column to a report, ensure that you understand what information the new column will provide. Columns with similar names can provide different values. For example, the Est. Gross Profit (transaction) column provides results that are different from the Est. Gross Profit (Line) column. The Est. Gross Profit (transaction) column finds lines that meet the criteria and then sums the transaction-level gross profit for each line. The Est. Gross Profit (Line) column finds lines that meet the criteria and then sums the line-level gross profit for each line.

#### To add columns to your report : {#bridgehead_N738794}

1.  Click **Customize** in the footer of the report.
    
2.  On the Report Builder (or Financial Report Builder) page, click **Edit Columns**.
    
3.  In the Add fields pane, choose the field for the column you want to add. The list of fields is organized by report component.
    
    Click the field name to add it as the last column or drag it from the Add Fields pane to the order you want in the Report Preview pane.
    
4.  In the Report Preview pane, enter a new heading for your column or keep the default heading.
    
5.  (Optional) Choose from the following column options:
    
    -   Add a **Grand Total, Running Balance**, **Percent of Total, Dollar Variance** or **Percent Variance** column to the right of the column you're adding.
        
    -   Choose a **Units of Measure** to display your data in Base Units, Stock Units, Purchase Units, or Sales Units.
        
    -   Select from **Summary** options to display the minimum or maximum, provide a count, present the average, and sum any set of amounts. You can't use summary options on Detail reports. For more information about summary options, see [Arranging Data on Summary Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4353206428.html).
        
    -   Select an **Alternate Date Range** for this column only. All other columns will use the range selected in the footer of the report.
        
    
    The column options available depend on the field you selected in step 3.
    
6.  Repeat steps 3-5 to add more columns.
    
7.  Click **Save**.
    
    New columns are always added at the end of the report.
    

Warning:

For performance reasons, a report can't include more than 30 data columns. If you try to add a 31st column on the Edit Columns page, you'll get an error. It's OK for report results to include more than 30 columns if matrix columns are added at run time. See [Adding Matrix Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741181.html).

For more information about adding specific types of columns, see the following topics:

-   [Adding Time-Based Comparison Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N739328.html)
    
-   [Adding Formula Fields to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N740229.html)
    
-   [Adding Matrix Columns to Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N741181.html)
    
-   [Adding a Percent of Expense Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2107074.html)
    
-   [Adding a Percent of Income Column to an Income Statement](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2109173.html)
    

## Adding a Name or Name (Group) Column {#bridgehead_4078557215}

For reports that have the Customer/Project component, you can add a Name or Name (Group) field as a report column. There's a difference between the full name and the name of the company. The full name of a company is the parent of the company and the location. For example, the full name could be NetSuite San Mateo, whereas the name is San Mateo. The Name is the full company name, but the Name (Group) creates a company hierarchy in your report. You can use the Group box to create hierarchy by company.

## Adding an Amount (U.S. Style) Column {#bridgehead_3830033769}

For reports with the Account Balance component (Revenue reports), you can add an Amount (US Style) field as a column instead of the Amount field. The Amount (US Style) field is helpful for reports run in non-U.S. editions of NetSuite or for non-U.S. subsidiary contexts in OneWorld accounts. When you use this field, the sign matches the Amount field in the U.S. edition. If you use the Amount field, the signs of these values may be reversed.

### Related Topics

-   [Adding, Removing, or Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N738669.html)
-   [Removing Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N739059.html)
-   [Reordering Report Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N739142.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
