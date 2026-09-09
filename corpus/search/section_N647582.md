---
id: "section_N647582"
type: "section"
title: "Using Expressions in Search Criteria"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Simple and Advanced Searches > Defining an Advanced Search > Advanced Search Criteria Filters > Using Expressions in Search Criteria"
parent: "section_N646477"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647582.html"
anchors: ["procedure_N647602"]
sha256: "79d193db80d051ce57b288c6848be092cbd39602aea5b32ee3132bb3ed925f65"
---

You can use parentheses in search criteria for advanced and saved searches. When you create expressions, you can set up criteria connected by AND or OR.

For example, you can search for customers who live near your store location in CA by entering **(city is San Francisco AND phone starts with 415) OR (city is Los Angeles AND phone starts with 310) OR (city is San Diego AND phone starts with 619)**.

NetSuite addresses parentheses from inside to outside. For example, in the following expression **(clause1 AND ((clause2 OR clause4) AND (clause5 OR clause6))) OR clause7**, clauses are processed in this order:

1.  '(clause2 OR clause4)' and '(clause5 OR clause6)'
    
2.  '((clause2 OR clause4) AND (clause5 OR clause6))'
    
3.  '(clause1 AND ((clause2 OR clause4) AND (clause5 OR clause6)))'
    
4.  '(clause1 AND ((clause2 OR clause4) AND (clause5 OR clause6))) OR clause7'
    

We can show it on a transaction saved search with these criteria:

          `(Type is 'Journal' AND (Account is 'Sales Orders' OR Account is 'Purchase Orders' )) OR Account is 'Estimates'` 
        

This search shows all transactions with the **Estimates** account (regardless of transaction Type) and all journal transactions with the **Sales Orders** or **Purchase Orders** accounts.

![And/Or expressions example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/ExpressionsAndOr.png)

#### To define search criteria using expressions: {#procedure_N647602}

1.  On the **Criteria** subtab of an advanced or saved search, check the **Use Expressions** box.
    
2.  To indicate criteria for records or transactions you don't want in your results, check the box in the **Not** column.
    
3.  In the **Parens** column, select an opening parenthesis to begin an expression.
    
4.  In the **Filter** column, select a field from the record or transaction you want to use.
    
    For more information about defining filters, see [Defining Standard Search Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646693.html).
    
5.  In the popup window, set your filter criteria and click **Set**.
    
6.  In the **Parens** column you can close the parentheses or leave it blank to add to your expression.
    
7.  In the **And/Or** column:
    
    -   Select **And** to add criteria that records or transactions must also meet to be in your results list. Records or transactions must match all criteria connected by **And**.
        
    -   Select **Or** to add criteria that return records or transactions that match either the first line of criteria or the next one you add. They can match any criteria connected by **Or**.
        
8.  In the **Parens** column, close your parentheses to end an expression.
    
9.  Click **Add** when you've finished a line of criteria.
    
10.  After setting your criteria:
     
     -   If you're doing an advanced search, choose how you want your results to look, then click **Submit**.
         
     -   If you're saving or customizing a search, set up your results and filters, then click **Save**.
         

Important:

If the **Use Expressions** option is enabled for a search, inline editing is disabled in list, dashboard, and sublist views based on that search. If you want inline editing to be available, ensure that the **Use Expressions** box isn't checked for the search that filters view results.

### Related Topics

-   [Advanced Search Criteria Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646477.html)
-   [Defining Standard Search Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646693.html)
-   [Main Line in Transaction Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4459563851.html)
-   [Summary Search Filters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N647835.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
