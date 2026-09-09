---
id: "bridgehead_N663440"
type: "bridgehead"
title: "Comparing Summed Amounts Across Two Fiscal Years for Transactions"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Comparing Summed Amounts Across Two Fiscal Years for Transactions"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N663440.html"
anchors: []
sha256: "b3a71c0c202b0af14172e996c7aae9255dddc65f622170328ca9b30e6657e64e"
---

In transactions, you can compare summed amounts across two fiscal years.

#### To compare the summed amounts:

1.  On the **Criteria** subtab, check the **Use Expressions** box and enter the following on two separate lines:
    
    Date is within this fiscal year to date OR Date is within last fiscal year to date.
    
2.  On the **Results** subtab, enter the following formulas:
    
    -   If the fiscal year starts in July:
        
        -   For current year to date, Formula (Numeric), SUMMARY TYPE = Sum:
            
                                    `DECODE(TO_CHAR(ADD_MONTHS({trandate},6),'YYYY'), TO_CHAR(ADD_MONTHS({today},6),'YYYY'),{amount},0)` 
                                  
            
        -   For previous year to date, Formula (Numeric), SUMMARY TYPE = Sum:
            
                                    `DECODE(TO_CHAR(ADD_MONTHS({trandate},6),'YYYY'), TO_CHAR(ADD_MONTHS({today},-6),'YYYY'),{amount},0)` 
                                  
            
    -   If the fiscal year is the calendar year:
        
        -   For current year to date, Formula (Numeric), SUMMARY TYPE = Sum:
            
                                    `DECODE(TO_CHAR({trandate},'YYYY'),TO_CHAR({today},'YYYY'),{amount},0)` 
                                  
            
        -   For previous year to date, Formula (Numeric), SUMMARY TYPE = Sum:
            
                                    `DECODE(TO_CHAR({trandate},'YYYY'),  TO_CHAR(ADD_MONTHS({today} ,-12),'YYYY'),{amount},0)` 
                                  
            

Note:

Consider the following:

-   `ADD_MONTHS` compensates calendar year for current fiscal year (6) and previous fiscal year (- 6) if fiscal year begins in July, and compensates for previous year (-12) if fiscal year is the same as calendar year.
    
-   `TO_CHAR` extracts the (fiscal) years.
    
-   `DECODE(value1, value2, {amount}, 0)` compares the transaction date's fiscal year value (`value1`) to the current or previous fiscal year (`value2`). If equal, use amount; otherwise zero it out.
    

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
