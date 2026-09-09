---
id: "bridgehead_N663290"
type: "bridgehead"
title: "Displaying the Percentage Variance between Custom Record Values"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Displaying the Percentage Variance between Custom Record Values"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N663290.html"
anchors: []
sha256: "a3b4422b41740e5e01490ef20a1e8337206b6e739ff00c9440dcf301894a174b"
---

On the **Results** subtab, select **Formula (Percent)**, a summary type of **Group**, and a Function of **Round to Hundredths**. You can also add a custom label, such as **Average**. Enter the following formula:

          `ROUND ( ({custrecord_value1} / {custrecord_value2} - 1.00 ) * 100, 2)` 
        

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
