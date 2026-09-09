---
id: "section_N660895"
type: "section"
title: "Using a Custom Formula Field in a Search"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Using a Custom Formula Field in a Search"
parent: "article_5143710889"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html"
anchors: ["procedure_N660903"]
sha256: "fcf868ca579dbd4d8153ccaf6b37ff35dac54fd1fab6faeda5a12d2748ef73c6"
---

#### To use a previously defined custom formula field in a search: {#procedure_N660903}

1.  On an advanced or saved search page, on the **Criteria** or **Results** subtab, select the previously defined custom field and set criteria as for any other custom field. Click **OK**.
    
    To learn how to define a custom formula field, see [Creating Formula Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2832369.html).
    
    ![Available Non-Committed Quantity (Custom) field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteAnalyticsDashboardsSearchesReports/Search/customformula1.png)
2.  Click **Submit** to view your search results.
    
    Note:
    
    If your searches are returning static values for a custom formula field instead of recalculating when new data is entered into the system, the field may have been defined to store the value for the calculation at the time of record creation. This is controlled by the **Store Value** box on the custom field definition. Check with your system administrator if the value should be dynamically calculated at the time of every search.
    
    Note:
    
    If the formula field does not have the **Store Value** box checked, the field is not available in search results, including lists based on saved searches.
    
    If you have a use case for running a saved search on a formula field where the value is not stored, an alternative solution is available. For more information, see Running a Saved Search on a Formula Field Where the Value is Not Stored (SuiteAnswers ID: 1017388).
    

Important:

To improve the security of saved searches, results for Formula (Text) fields are displayed as plain text only. To prevent issues with your searches, you should replace your Formula (Text) fields with the Formula (HTML) field. For more information about the Formula (HTML) field, see [Evaluating Code in Saved Searches Using Formula(HTML) Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0403035152.html).

### Related Topics

-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
