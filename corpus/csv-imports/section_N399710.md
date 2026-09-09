---
id: "section_N399710"
type: "section"
title: "Common Errors When Importing Cost Templates"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Supply Chain Import Type > Manufacturing Cost Template Import > Common Errors When Importing Cost Templates"
parent: "section_N395199"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N399710.html"
anchors: ["bridgehead_N399722", "bridgehead_N399738"]
sha256: "29bcd3e180e896879e1f899aa363b4031c68deda710bb2f3629e0dade9595b53"
---

The 'Results' file for a failed cost template import might include any of the following messages.

## You must enter at least one line {#bridgehead_N399722}

This error indicates that you failed to include sublist data for every cost template record. Each cost template record must have at least one sublist record.

If you're doing a multiple-file import, this error might point to a problem with the key column you're using to link the files. For example, one of the files might include a typo in this column, preventing proper linking of the cost template's body data to its sublist data.

## Invalid item reference key {#bridgehead_N399738}

Indicates that the item name in one of your sublist records is incorrect. You may have typed it incorrectly, or you may have paired it with a cost category that it doesn't belong to. Check the item record to see what the correct category is. The category is shown on the Purchasing subtab of the item record.

### Related Topics

-   [Manufacturing Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395199.html)
-   [Prerequisite Records for Cost Template Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N395402.html)
-   [Cost Template Body and Sublist Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N396186.html)
-   [Cost Template CSV File Examples](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N398462.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
