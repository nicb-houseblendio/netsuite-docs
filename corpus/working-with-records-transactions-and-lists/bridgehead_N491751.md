---
id: "bridgehead_N491751"
type: "bridgehead"
title: "Status and Timing of Merge Operations"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection > Merging or Deleting Duplicate Records > Status and Timing of Merge Operations"
parent: "section_N491111"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491751.html"
anchors: []
sha256: "c7ab2549bdcfd318da01d1dfb30b898cbc97c5874dc641d5e945568b57771b80"
---

When you submit a duplicate merge operation, it's placed in a queue and is executed when operations ahead of it in the queue are completed. Go to _Lists > Mass Update > Duplicate Resolution Status_ to view the Duplicate Resolution Status page. Here you can view the status of duplicate merge operations, the number of records merged, and the number of records that could not be merged. You can view possible errors that occur during the operation by clicking the Details link in the Errors column.

After you submit a duplicate merge operation, you can keep working in NetSuite without waiting for the merge operation to finish. You can't edit records you've marked as duplicates during the time that the duplicate operation is queued or running. The primary record is locked only for a brief time when the merge starts.

Note:

System notes aren't transferred from duplicate entity records to the primary entity record during a merge. Merging entities updates the system notes and last modified date for all transactions associated with the duplicate entity or entities. The system notes for these transactions will indicate that they were updated by the Duplicate Resolution process.

Warning:

Merging entities is a data-intensive operation, and complex merges of many records such as transactions, custom fields, or workflows may time out when processing. You should test the merge process in a sandbox account first to ensure that it can be completed.

You should designate the entity with the most transactions as the primary record and entities with fewer transactions as duplicates to reduce the time it takes to complete the merge. You should also avoid merging entities with large numbers of transactions whenever possible.

Historical log records for duplicate merge tasks are saved in NetSuite for only seven days before the information is permanently erased.

### Related Topics

-   [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html)
-   [Manage Record Duplicates Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4160068263.html)
-   [Submitting Merge Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491162.html)
-   [Merging Records with Active Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3843896859.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
