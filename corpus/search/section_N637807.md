---
id: "section_N637807"
type: "section"
title: "Global Search by Email Address"
branch: "search"
category: "suiteanalytics"
breadcrumb: "SuiteAnalytics > Search > Global Search > Tips for Effective Global Searches > Global Search by Email Address"
parent: "section_N637092"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637807.html"
anchors: []
sha256: "43af81387ab504f66fd30cd86f2353176f7753bb79ac5ed8663c3729541f0bdb"
---

To search for an email address, enter the full address in the format **<user name>@<domain>**.

When you use this format, global search treats it as a single keyword and returns only an exact match.

This special handling of email address overrides the usual rule where the **.** and **@** characters are treated as spaces.

For example:

-   If you enter a full email address, such as **john.brown@abc.com**, you get that exact match only.
    
-   If you enter only **brown@abc.com**, global search still treats it as a full email address and returns that exact match only.
    
-   If you enter only **john.brown**, global search looks for "john" and "brown" as separate keywords, and returns any records containing these two keywords.
    

The starts-with matching doesn't work for email addresses, you need the full email address for global search to recognize it as an email address.

### Related Topics

-   [Tips for Effective Global Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N637092.html)
-   [Global Search by IP Address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N639465.html)
-   [Global Search by Document Number](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554367380.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
