---
id: "bridgehead_N663716"
type: "bridgehead"
title: "Calculating Days a Sale Is In Effect"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Calculating Days a Sale Is In Effect"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N663716.html"
anchors: []
sha256: "44b4a8770a1e8eba742075d39f57f888fb7a2be1dfe681d15b87b44519210f6a"
---

You can use a formula to calculate the days a sale is in effect up to the date it is canceled, like a contract age. If there is no cancellation date, substitute today's date. Select **Formula(Numeric)** and enter the following formula:

          `ABS({custom_field_startdate}-nvl({custom_field_cxldate},{today}))` 
        

You can use a similar formula to calculate the days remaining on a contract based on the end date field.

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
