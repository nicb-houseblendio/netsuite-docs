---
id: "bridgehead_N663826"
type: "bridgehead"
title: "Calculating Time Taken to Approve Orders"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Calculating Time Taken to Approve Orders"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N663826.html"
anchors: []
sha256: "4401e1599fc67996510b0b470e382bbb7a10c2cf053ab2a3dab626f10a4cded9"
---

You can use formulas in searches to calculate the time taken to approve orders.

#### To use a formula for calculating the time taken to approve orders:

1.  Create a Transaction search, with filters of Type is Sales Order, Main Line is true, System Notes : Field is Document Status, and System Notes : New Value is Pending Fulfillment.
    
2.  Add a **Formula(Numeric)** results column with the formula {systemnotes.date}-{datecreated}. You can add a Custom Label that indicates this calculation is the time taken to approve each order.
    

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
