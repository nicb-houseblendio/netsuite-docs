---
id: "section_N661334"
type: "section"
title: "Using a Formula in Search Results"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Using a Formula in Search Results"
parent: "article_5143710889"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html"
anchors: ["procedure_N661347"]
sha256: "c1089fef888275207df928940844681b14c789964ecb568aaa43a8e0503ebb02"
---

#### To use a formula as a search result: {#procedure_N661347}

1.  On the **Results** subtab of an advanced or saved search page, in the **Field** column, select the required Formula type.
    
    The following options are available (they are listed in alphabetical order, intermingled with field names in the **Field** column dropdown list):
    
    | Formula Type | Example |
    | --- | --- |
    | Formula(Currency) | `TO_NUMBER({amount})` |
    | Formula(Date) | `TO_DATE('11/16/2020','MM/DD/YYYY')` |
    | Formula(Date/Time) | `{now}` |
    | Formula(Numeric) | `{field_id}` |
    | Formula(Percent) | `% of total 30/100` |
    | Formula(Text) | 
    -   `{quantity} || 'x ' || {item}`
    -   `CASE WHEN {duedate} < CURRENT_DATE THEN 'Overdue' ELSE 'On Time' END`
    
     |
    | Formula(HTML) | 
    
    -   `'<a href="https://docs.oracle.com/app/common/entity/entity.nl?id=%27%20||%20{entity.id}%20||%20%27" target="_blank">' || {entity} || '</a>'`
    -   `NVL2({approvalstatus}, '<span> Approved</span>', '<span> Not Approved</span>')`
    
     |
    
    As when you define formulas for search criteria, the type of formula you choose should correspond to the type of calculation and validation required.
    
    Important:
    
    To improve the security of saved searches, results for Formula(Text) fields are displayed as plain text only. To prevent issues with your searches, you should replace your Formula(Text) fields with the Formula (HTML) field. For more information about displaying HTML code in your search results, see [Evaluating Code in Saved Searches Using Formula(HTML) Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403035152.html).
    
2.  In the **Formula** field, define your formula and click **Done**, or click the **Set Formula** button to open a popup window that can help you correctly enter the formula expression.
    
    Note:
    
    For details about supported SQL functions, refer to [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html). For tables of NetSuite field IDs, you can also refer to [SuiteScript Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3170023.html).
    
    -   Select from the Function dropdown list to include a SQL function in the formula expression.
        
    -   Select a field name from the Field dropdown list to include its ID in the formula expression.
        
    -   There is a 1000 character limit per formula expression. You may be able to preview a search with a formula containing more characters, but when you run the search invalid expression errors occur.
        
3.  Click **Submit** to view your search results.
    

For example, to add a search results column that displays the total number of days a case has been open, enter the formula {today}-{startdate}.

### Related Topics

-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
