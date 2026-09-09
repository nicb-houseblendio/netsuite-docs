---
id: "bridgehead_N663659"
type: "bridgehead"
title: "Finding the Most Recent Record Updater"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Formulas in Searches > Search Formula Examples and Tips > Finding the Most Recent Record Updater"
parent: "section_N662868"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N663659.html"
anchors: []
sha256: "edeba91c6c23b1fab762a5d85d4d08f76e0d82fc6c3d5a8e97d05dc18f4e94fb"
---

Use the `dense_rank` function in a formula to order records by values in a field and assign each record a consecutive numeric ranking from 1 to _n_, where _n_ is the number of records returned.

Use the keep (`dense_rank`) function to return only the first or last ranking record as ordered by values in a specified field.

For example, to return the name of the user who most recently updated a document, do a document search and create a **Formula(Text)** field with a Summary Type of **Minimum** and a formula like the following:

min({systemnotes.name}) keep (dense\_rank last order by {systemnotes.date})

### Related Topics

-   [Search Formula Examples and Tips](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N662868.html)
-   [Formulas in Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_5143710889.html)
-   [Using a Custom Formula Field in a Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N660895.html)
-   [Using a Formula in Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661053.html)
-   [Using a Formula in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N661334.html)
-   [Using Formula Tags in Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054298146.html)
-   [SQL Expressions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2833020.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
