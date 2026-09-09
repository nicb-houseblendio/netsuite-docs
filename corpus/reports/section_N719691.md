---
id: "section_N719691"
type: "section"
title: "Row Limitations for Report Results"
branch: "reports"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Reports > Working with Report Results > Navigating a Report > Row Limitations for Report Results"
parent: "section_N718860"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719691.html"
anchors: []
sha256: "dabfb3744778169c9b266d185a1c58ddc5dcde5c73efb0febd61a8bd09d2d2a9"
---

Report size is measured by the number of database rows retrieved for it. The number of rows retrieved for a report might be higher than the number displayed, for example when results are split across multiple classifications.

Report results get cut off if they exceed the following row limits. These limits help performance. Row limits are the same for all NetSuite reports, but reports run in the background, like scheduled, emailed, or exported reports, have higher limits.

The limits for retrieved rows per report are:

-   100,000 rows - for a report executed on demand (synchronously)
    
-   1,000,000 rows - for a report executed in the background (asynchronously)
    

If a report is being truncated, you can try the following:

-   Set additional filters to limit report results. See [Filtering Data on Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N742381.html).
    
-   Create a saved search to return the desired data. Saved searches don't have row limitations like reports, although you may be unable to export search results with extremely large data sets. See [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html). To learn how to persist saved search results for searches that contain a high volume of data, see [Persisting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_1029112142.html).
    
-   Obtain access to NetSuite SuiteAnalytics Connect service. See [SuiteAnalytics Connect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3963845427.html).
    

### Related Topics

-   [Navigating a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N718860.html)
-   [Drilling Down to Records or Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719130.html)
-   [Using the Report Navigation Pane](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N719475.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
