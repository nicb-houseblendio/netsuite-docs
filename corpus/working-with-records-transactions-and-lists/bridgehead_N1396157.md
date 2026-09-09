---
id: "bridgehead_N1396157"
type: "bridgehead"
title: "Currency Field Limitations"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Working with Records > Currency Field Limitations"
parent: "section_N488213"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1396157.html"
anchors: []
sha256: "53966efbaaf331976f830542eb7f510d725d9dc35c8c38fd184e255afab2d184"
---

When you work with currency fields in NetSuite, the fields might not calculate the correct value for large decimal numbers correctly. This is related to the limitations of floating-point numbers in computer science.

The maximum whole number that can be represented accurately is 9,007,199,254,740,991. However, for decimal numbers, when a number has 15 or more digits before the decimal point, rounding errors can occur. For example, 142,325,911,132,191.64 might be incorrectly rounded to 142,325,911,132,191.62.

With more digits before the decimal, the system may truncate the decimal part entirely, for example 14,232,591,113,219,174.64 might be rounded to 14,232,591,113,219,174.

### Related Topics

-   [Working with Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N488213.html)
-   [NetSuite Record Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N488305.html)
-   [NetSuite Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N488657.html)
-   [Searching for Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4335483183.html)
-   [Viewing and Editing Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N489685.html)
-   [Creating a Transaction from a Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N561399.html)
-   [Attaching Files to Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490137.html)
-   [Inactivating Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490731.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
