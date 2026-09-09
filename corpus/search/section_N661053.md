---
id: "section_N661053"
type: "section"
title: "Using a Formula in Search Criteria"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Using a Formula in Search Criteria"
parent: "article_5143710889"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html"
anchors: ["procedure_N661066"]
sha256: "0fb826b550a6e9378b2ec0ad4e943c3783f7ffa7919e43c1c72eef865321c83a"
---

#### To use a formula in search criteria: {#procedure_N661066}

1.  On the **Criteria** subtab of an advanced or saved search page, in the **Filter** column, select the required Formula type.
    
    The following options are available (they are listed in alphabetical order, intermingled with field names in the **Filter** column dropdown list):
    
    -   Formula (Date)
        
    -   Formula (Numeric)
        
    -   Formula (Text)
        
    
    The best choice for a formula type depends upon the calculation the formula will perform, because validation varies according to the formula type. For example, to do character manipulation using regular expressions, you should select **Formula (Text)**. To do numeric calculations, **Formula (Numeric)** is likely a better choice.
    
    Important:
    
    Saved and advanced searches show only up to 13 characters for Integer Number type fields. Use **Formula (Text)** to display Integer Number type fields with values of 14 digits or more. For more information, see [Integer Number Fields in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0220051223.html).
    
    To include both positive and negative values in search results when using Quantity, set **Formula (Numeric)** in the **Filter** field and `{Quantity}` in the **Formula** field. If you use **Quantity** in the **Filter** field, you will receive only positive values in search results. All negative results are automatically filtered out.
    
    Important:
    
    To avoid cross-scripting (XSS) vulnerabilities, results for **Formula (Text)** fields that contain <script> tags do not display script output. Do not use <script> tags in **Formula (Text)** fields.
    
2.  In the Formula popup window, define your formula, and click **Set**.
    
    Note:
    
    For details about supported SQL functions, refer to [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html) . For tables of NetSuite field IDs, you can also refer to [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html).
    
    -   Options vary depending on the type of formula selected. For example, date formulas can be filtered based on whether the date occurs before or after a specified date, whereas numeric formulas can be filtered based on whether the resultant value is greater than or equal to the specified criteria.
        
    -   Select from the Function dropdown list to include a SQL function in the formula expression.
        
    -   Select a field name from the Filter dropdown list to include its ID in the formula expression.
        
    -   There is a 1000 character limit per formula expression. You may be able to preview a search with a formula containing more characters, but when you run the search invalid expression errors occur.
        
    -   Remember that search records are dynamically filtered based on the **calculated** value of the formula at the time the search is performed.
        
3.  Click **Submit** to view your search results.
    

For example, select **Formula (Numeric)** and enter the formula **{today} - {startdate}**, then set the criteria as greater than or equal to **3**, as shown in the following figure.

![Example custom formula.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/SearchFormulaNumeric.png)

### Related Topics

-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
