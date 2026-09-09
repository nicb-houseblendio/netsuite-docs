---
id: "section_N649095"
type: "section"
title: "Using When Ordered By Field for Search Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining an Advanced Search > Search Results Display Options > Using When Ordered By Field for Search Results"
parent: "section_N648053"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649095.html"
anchors: ["procedure_N649166"]
sha256: "4f1394580fdb8e24fe717d1ffeba4d40337dc3b9eb2cb460571fad9636f8a02c"
---

The **When Ordered By** field option gets results for a field when another field is at its lowest or highest value. For example, you can use it to return the:

-   amount for the most recent sales order by each customer
    
-   contact for the most recent case filed by a customer
    
-   sales rep for the top transaction by month
    
-   item with the largest transaction per month
    

The **When Ordered By** field is available when you select Minimum or Maximum for a Summary Type on the **Results** subtab.

Usually, the **When Ordered By** field is a date or a number. Maximum finds the record with the most recent date or largest quantity, and Minimum finds the record with the earliest date or smallest quantity. (All of the examples above use Maximum).

Important:

If your **When Ordered By** field has NULL values, these records appear last in results (or first if you use Maximum). To avoid this, don't use Maximum with the **When Ordered By** field set to NULL.

#### To return the value of a search results field when another value is minimal or maximal: {#procedure_N649166}

1.  On the **Results** subtab, select the field you want a value for in the **Field** column.
    
2.  In the **Summary Type** column, select Minimum or Maximum, depending on if you want the value from the record where the **When Ordered By** field is lowest or highest.
    
3.  Select the field that you want to minimize or maximize in the record returned.
    

For example, to get the amount for each customer's most recent transaction, create a Customer search, set **Formula (Date)** as the results field, **Summary Type** to **Maximum**, and **When Ordered By** to **Date Created**.

![Custom search results example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/custom3.png)

Note:

The **When Ordered By** field doesn't support **Long Text** or **Rich Text** fields, so you can't see them in the dropdown list.

**When Ordered By** in NetSuite works like Oracle's analytic 'keep dense\_rank'. For example, if you have these transactions:

| **Name** | **Amount** | **Date** |
| --- | --- | --- |
| John | 123 | 01/23/2024 |
| Mike | 10 | 05/12/2024 |
| Peter | 777 | 05/12/2024 |
| Peter | 777 | 06/12/2024 |
| John | 15 | 12/12/2024 |
| Mike | \-13 | 05/12/2024 |
| John | 456 | 12/11/2023 |

If you want to see when the last transaction with the highest amount was created, go to the **Results** tab and add these fields:

| **Field** | **Summary Type** | **When Ordered By** |
| --- | --- | --- |
| Date | Maximum | Amount |

The result is 06/12/2024.

If you want to get the highest amount for each customer's most recent transaction, go to the **Results** tab and add these fields:

| **Field** | **Summary Type** | **When Ordered By** |
| --- | --- | --- |
| Name | Group | \- |
| Amount | Maximum | Date |

The results are shown in the table below:

| **Name** | **Amount** |
| --- | --- |
| John | 15 |
| Mike | 10 |
| Peter | 777 |

If you want the lowest amount for each customer's earliest transaction, go to the **Results** tab and add these fields:

| **Field** | **Summary Type** | **When Ordered By** |
| --- | --- | --- |
| Name | Group | \- |
| Amount | Minimum | Date |

The results are shown in the table below:

| **Name** | **Amount** |
| --- | --- |
| John | 456 |
| Mike | \-13 |
| Peter | 777 |

### Related Topics

-   [Search Results Display Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648053.html)
-   [Selecting Fields to Display in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648349.html)
-   [Entering Custom Labels for Search Results Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648659.html)
-   [Defining Summary Types to Roll Up Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N648820.html)
-   [Showing Totals in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649366.html)
-   [Applying Functions to Search Results Columns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N649633.html)
-   [Defining Order and Overall Formatting for Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N651604.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
