---
id: "section_N575781"
type: "section"
title: "Limitations on Exports to PDF"
branch: "exporting-reports-searches-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Exporting Reports, Searches, and Lists > Limitations on Exports to PDF"
parent: "chapter_N575321"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N575781.html"
anchors: []
sha256: "eb7c54eac11ae3ad070f9c64d2d14ff38c6ee062653efbc7dac39a59bc7859b1"
---

Exported PDFs have some limitations. If your export has more than 10,000 rows, exporting to PDF could cause an error. Also, if your export has a lot of columns or long field values, you may see formatting issues.

To avoid performance problems, don't export more than 30 columns. If you export more than 10 columns, the number of rows is limited, as shown in the table below:

| Number of Columns in PDF Export | PDF Export Row Limit |
| --- | --- |
| 1-9 columns | 3000 rows |
| 10-20 columns | 2000 rows |
| 21-30 columns | 1000 rows |
| more than 30 columns | not supported |

All PDFs you export are checked against the BFO document type definition (DTD). BFO is a a set of third-party libraries for generating PDF documents. The BFO documentation is available at [http://bfo.com/products/report/docs/userguide.pdf](http://bfo.com/products/report/docs/userguide.pdf).

### Additional Information

-   [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html)

### Related Topics

-   [Exporting Reports, Searches, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html)
-   [Limitations on CSV Exports of Data with Special Characters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N576068.html)
-   [Comparing Export Formats](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N575321.html#bridgehead_N575409)
-   [Exporting Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N495079.html)
-   [Exporting a Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N736119.html)
-   [Exporting Search Results](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N663983.html)
-   [Exporting Account Registers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1511672.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
