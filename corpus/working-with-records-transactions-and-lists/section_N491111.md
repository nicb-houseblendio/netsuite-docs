---
id: "section_N491111"
type: "section"
title: "Merging or Deleting Duplicate Records"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection > Merging or Deleting Duplicate Records"
parent: "section_N490932"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html"
anchors: []
sha256: "000b63d1dad4bcc83f1646b86593ba3f6d58276b1d3c71cef429d47b90f0ef69"
---

When you find duplicate records in your NetSuite account, you can merge them, resulting in one complete record for each person or company you do business with.

Four types of records support duplicate matching:

-   Customer
    
-   Vendor
    
-   Partner
    
-   Contact
    

The Administrator role is required to set up which types of records you detect duplicates for and how you determine that two records are duplicates. An administrator selects fields on records to check for matching information. When matches are found, the system identifies the records as possible duplicates. For example, the administrator may choose to identify duplicates based on matching email addresses. If the selected fields are blank, they don't match.

You must have full permissions for the entity types you're merging. For example:

-   You must have full permissions for Vendors to merge two vendors.
    
-   You must have full permissions for both Contacts and Customers to merge Individual Customers, which are composed of both.
    
-   You must have full permissions for both Customers and Vendors to merge into a Customer/Vendor entity.
    

When you merge records, the records' transaction histories are also merged. The original data, such as entity name, is retained to preserve a transaction's history. Your administrator may have restricted the ability to perform merges to specific roles.

Note:

System notes aren't transferred from duplicate entity records to the primary entity record during a merge. Merging entities updates the system notes and last modified date for all transactions associated with the duplicate entity or entities. The system notes for these transactions will indicate that they were updated by the Duplicate Resolution process.

Warning:

Merging entities is a data-intensive operation, and complex merges of many records such as transactions, custom fields, or workflows may time out when processing. You should test the merge process in a sandbox account first to ensure that it can be completed.

You should designate the entity with the most transactions as the primary entity and entities with fewer transactions as duplicates to reduce the time it takes to complete the merge. You should also avoid merging entities with large numbers of transactions whenever possible.

You can merge duplicate entity records that have login access but have different email addresses only if an administrator has set the **Resolve Duplicates with Conflicting Login Access** preference to **By deleting the duplicates' access**. This setting deletes the login access of records you define as duplicates. When this preference is set to the default value of **Manually**, you must first manually remove the login access of one record before you merge. The person whose access is removed must use the login access defined on the primary record. Be sure to notify this person of the change because the deleted login will no longer work.

To prevent you from merging records that aren't duplicates, you can only merge records if they have the same tax registration numbers or if both records don't have tax registration numbers.

This section is divided into the following subsections:

-   [Manage Record Duplicates Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4160068263.html)
    
-   [Submitting Merge Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491162.html)
    
-   [Merging Records with Active Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3843896859.html)
    
-   [Status and Timing of Merge Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491751.html)
    

Note:

For NetSuite OneWorld accounts: you can only merge entities from different subsidiaries if they're the same type.

For more information administrators should see [Setting Up Duplicate Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html).

### Related Topics

-   [Duplicate Record Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490932.html)
-   [Merging Large Numbers of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3744355188.html)
-   [Merging Different Types of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491887.html)
-   [Words Excluded from Duplicate Detection Matching](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492354.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
