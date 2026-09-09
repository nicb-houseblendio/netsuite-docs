---
id: "section_N490932"
type: "section"
title: "Duplicate Record Detection"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection"
parent: "chapter_N488023"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490932.html"
anchors: []
sha256: "793db4e421ac738c34c128130596d0084d13b27d040eb25032b40b818765e760"
---

The Duplicate Detection & Merge feature helps you find duplicate records in your NetSuite account and use the information in them to create a single record.

An administrator can turn on the Duplicate Detection & Merge feature at _Setup > Company > Enable Features (Administrator)_ on the Company subtab in the Data Management section. The administrator configures the types of records you detect duplicates of and also chooses which fields to consider when finding duplicates. For more information about the setup of this feature, see [Setting Up Duplicate Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N258211.html).

Four types of records support duplicate matching:

-   Customer
    
-   Vendor
    
-   Partner
    
-   Contact
    
    Note:
    
    Private contacts are excluded from the Duplicate Detection process.
    

You must have full permissions to the entity types you're merging. For example:

-   You must have full permissions for Vendors to merge two vendors.
    
-   You must have full permissions for both Contacts and Customers to merge Individual Customers, which are composed of both.
    
-   You must have full permissions for both Customers and Vendors to merge into a Customer/Vendor entity.
    

Duplicate Customers and Vendors can be detected across subsidiaries. The subsidiary a potential duplicate customer or vendor belongs to is shown in the Primary Subsidiary column. You must first enable the Detect Duplicates Across Subsidiaries feature at _Setup > Company > Company Management > Duplicate Detection_.

Note:

System notes aren't transferred from duplicate entity records to the primary entity record during a merge. Merging entities updates the system notes and last modified date for all transactions associated with the duplicate entity or entities. The system notes for these transactions will indicate that they were updated by the Duplicate Resolution process.

Warning:

Merging entities is a data-intensive operation, and complex merges of many records such as transactions, custom fields, or workflows may time out when processing. You should test the merge process in a sandbox account first to ensure that it can be completed.

You should designate the entity with the most transactions as the primary entity and entities with fewer transactions as duplicates to reduce the time it takes to complete the merge. You should also avoid merging entities with large numbers of transactions whenever possible.

With this feature enabled, you get a notification before saving a record that might be a duplicate. Notification occurs in two ways:

-   When you create a new record and enter matching data in fields the administrator set up as duplicate criteria, a warning appears at the top of the record with a link to the potential duplicates. If you've permission to view those records, you can click the link to resolve these matching records.
    
-   When you add a record from a list by using Quick Add or use the Edit button to make changes to a record that would make it a duplicate, you receive a popup warning.
    

You can also go to _Lists > Mass Update > Entity Duplicate Resolution_ to search for all possible duplicate records based on your criteria. With the duplicate resolution mass update, you can find and resolve large numbers of duplicate records in your NetSuite account in a single operation.

For more information about how to manage duplicate records, see [Manage Record Duplicates Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4160068263.html).

For more information, see the following:

-   [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html)
    
-   [Merging Large Numbers of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3744355188.html)
    
-   [Merging Different Types of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491887.html)
    
-   [Words Excluded from Duplicate Detection Matching](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492354.html)
    

### Related Topics

-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)
-   [Working with Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N488213.html)
-   [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html)
-   [Working with Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N545359.html)
-   [Working with Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N494311.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
