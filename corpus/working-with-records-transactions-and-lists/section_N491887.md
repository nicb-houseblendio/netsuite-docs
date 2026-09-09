---
id: "section_N491887"
type: "section"
title: "Merging Different Types of Records"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection > Merging Different Types of Records"
parent: "section_N490932"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491887.html"
anchors: ["subsect_156268126238", "procedure_N491941"]
sha256: "77ac59beadae61acf84e6121a46090f86ce0746347a40554c9578dbd44ff5e5d"
---

Sometimes duplicate records exist between record types, such as a vendor record and a partner record for the same person or company. The Duplicate Detection feature only searches for possible matches within the same record type, but if you know of duplicated between two record types, you can merge them manually.

Note:

System notes aren't transferred from duplicate entity records to the primary entity record during a merge. Merging entities updates the system notes and last modified date for all transactions associated with the duplicate entity or entities. The system notes for these transactions will indicate that they were updated by the Duplicate Resolution process.

Warning:

Merging entities is a data-intensive operation, and complex merges of many records such as transactions, custom fields, or workflows may time out when processing. You should test the merge process in a sandbox account first to ensure that it can be completed.

You should designate the entity with the most transactions as the primary record and entities with fewer transactions as duplicates to reduce the time it takes to complete the merge. You should also avoid merging entities with large numbers of transactions whenever possible.

You can merge records between the following record types:

-   Partners
    
-   Vendors
    
-   Customers
    

You must have full permissions for the entity types you're merging. For example:

-   You must have full permissions for Vendors to merge two vendors.
    
-   You must have full permissions for both Contacts and Customers to merge Individual Customers, which are composed of both.
    
-   You must have full permissions for both Customers and Vendors to merge into a Customer/Vendor entity.
    

## Merging Customer/Vendor Entities in Different Subsidiaries {#subsect_156268126238}

You can merge Customer/Vendor entities across subsidiaries, creating a single multi-subsidiary Customer/Vendor entity. Merging two entities from different subsidiaries results in the following:

-   The primary subsidiary becomes the Primary Entity subsidiary.
    
-   The Duplicate Entity subsidiary becomes a secondary subsidiary for each entity.
    
-   The Contact from the primary subsidiary is linked and synchronized with the primary entity.
    

#### To merge records of different types: {#procedure_N491941}

1.  Open the duplicate record you want to merge into a primary record in edit mode. Don't make any changes to the record.
    
2.  Click **Merge**. This opens a new page.
    
3.  In the **Primary** field, select the name of the customer, partner, or vendor record into which the record should be merged.
    
    The record selected in the Primary field becomes the primary record.
    
4.  A summary of the files to be merged will appear in the **Duplicate/Master Summary**.
    
5.  Click **Save**.
    

The merged record opens. All activities, transactions, messages, files, cases, contacts, and other subtab lists are combined on the merged record. Any fields that were blank on the primary record get filled in from the duplicate, but existing data isn't replaced.

Note:

Administrators can restrict the ability of users to merge records. For more information about how to limit the merge function by role, see [Duplicate Entity Management Permission](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491767.html).

### Related Topics

-   [Duplicate Record Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490932.html)
-   [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html)
-   [Merging Large Numbers of Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3744355188.html)
-   [Words Excluded from Duplicate Detection Matching](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492354.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
