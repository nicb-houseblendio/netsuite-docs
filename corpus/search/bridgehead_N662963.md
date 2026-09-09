---
id: "bridgehead_N662963"
type: "bridgehead"
title: "Including Line Numbers in Transaction Searches"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Including Line Numbers in Transaction Searches"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N662963.html"
anchors: []
sha256: "5a5657bed72c0f8394384ff93a4afed8ad38294b3c47c6ce8fe359becc3c4145"
---

To make transaction line items easier to read, you can add line numbers to your transaction search results. On the **Results** subtab of the search definition page, add the **Line Sequence Number** field. This field shows the internal sequence number for each transaction line.

Line numbers may not always appear in order, even if your results include every line of a transaction. To show line numbers as a continuous sequence in your results, add a **Formula(Numeric)** field to your search results and use the following formula:

          `RANK() OVER (PARTITION by {internalid} ORDER BY {linesequencenumber})` 
        

You can create a custom formula field for line numbers and apply it to transaction forms to show line numbers on viewed and printed transactions. For instructions, see [Creating a Formula Field to Display Transaction Line Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2832808.html).

You can also include the line number in your search results to keep search results consistent with viewed and printed transaction items.

#### To include the line number in your search results:

1.  Set a criteria of Main Line = No (false).
    
2.  Filter out transaction line items related to taxes.
    
3.  Add the **Item** field as a results field.
    
4.  Add the **Amount (Gross)** field as a results field. Don't use the **Amount** field.
    
5.  Add a **Formula(Numeric)** field as a results field with the following formula expression:
    
                    `RANK() OVER (PARTITION by {internalid} ORDER BY {linesequencenumber})` 
                  
    

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
