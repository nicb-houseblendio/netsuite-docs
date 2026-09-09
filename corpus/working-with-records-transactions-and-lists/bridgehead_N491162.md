---
id: "bridgehead_N491162"
type: "bridgehead"
title: "Submitting Merge Operations"
branch: "working-with-records-transactions-and-lists"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > Working with Records, Transactions, and Lists > Duplicate Record Detection > Merging or Deleting Duplicate Records > Submitting Merge Operations"
parent: "section_N491111"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491162.html"
anchors: ["procedure_N491219"]
sha256: "617325c04aba019ec19f06545b04e399bc9f100f29a65181b620a24338c484c8"
---

Note:

You must have the full level of the Duplicate Entity Management permission to merge duplicates. By default, the Sales Person role has only view level. The Sales Manager and Administrator roles have full level.

Note:

System notes aren't transferred from duplicate entity records to the primary entity record during a merge. Merging entities updates the system notes and last modified date for all transactions associated with the duplicate entity or entities. The system notes for these transactions will indicate that they were updated by the Duplicate Resolution process.

Warning:

Merging entities is a data-intensive operation, and complex merges of many records such as transactions, custom fields, or workflows may time out when processing. You should test the merge process in a sandbox account first to ensure that it can be completed.

You should designate the entity with the most transactions as the primary entity and entities with fewer transactions as duplicates to reduce the time it takes to complete the merge. You should also avoid merging entities with large numbers of transactions whenever possible.

You must have full permissions for the entity types you're merging. For example:

-   You must have full permissions for Vendors to merge two vendors.
    
-   You must have full permissions for both Contacts and Customers to merge Individual Customers, which are composed of both.
    
-   You must have full permissions for both Customers and Vendors to merge into a Customer/Vendor entity.
    

#### To search for possible duplicates: {#procedure_N491219}

1.  Click the notice in the duplicate record.
    
    ![Warning notice with a link to the list of duplicates.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/NetSuiteBasics/WorkingWithRecords_DuplicateDetection.png)
2.  Expand the **Filters** area at the top of the list to display the filters.
    
3.  In the **Entities** filter, select a type of record to view possible duplicates for that type.
    
    Four types of records support duplicate matching:
    
    -   Customer
        
    -   Vendor
        
    -   Partner
        
    -   Contact
        
    
    For example, select **Contacts** to view all contacts you've access to that have some of the same information as other contact records.
    
    Important:
    
    You can merge two records that both have login access only if those records have different login email addresses and passwords.
    
4.  In the **Merge Type** field, select how you want to merge the selected records:
    
    | Option | Description |
    | --- | --- |
    | **Mark all selected as not duplicates** | This keeps all records without any changes. |
    | **Make duplicates subcustomers of primary** | This option is available only for customer records. It makes the duplicate record a subcustomer of the primary customer record. For more information, see [Creating a Subcustomer Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1085616.html). |
    | **Merge duplicates into primary record** | This merges all information from the duplicate records into empty fields in the primary record. If information is entered in the field on both the primary and the duplicate, the information about the primary record remains the same. |
    | **Merge duplicates into record created the earliest** | This saves the record with the earliest date in the Created column and places information from selected duplicated records into any empty fields on the saved record. |
    | **Merge duplicates into record with most populated fields** | This saves the record with the highest number in the Fields column and places information from selected duplicate records into any empty fields on the saved record. |
    | **Merge duplicates into record with most recent activity** | This saves the record with the most recent date in the Last Activity column and places information from selected duplicate records into empty fields on the saved record. |
    | **Delete duplicates, keep primary record** | This saves only the record you selected as the primary and deletes all records you selected as duplicates. |
    | **Delete duplicates, keep record created the earliest** | This saves the record with the earliest date in the Created column and deletes all other selected records in this group. |
    | **Delete duplicates, keep record with most populated fields** | This saves the records with the highest number in the Fields column and deletes all other selected records in that group. |
    | **Delete duplicates, keep record with most recent activity** | This saves the record with the most recent date in the Last Activity column and deletes all other selected records in the group. |
    | **Make duplicates subrecords of primary** | This saves the record you designate as the original, primary record and converts those you mark as duplicates into its subrecords. |
    
5.  For each group of records, check the box in the **Primary** column next to the record you want to designate as the main record. Information from duplicate records is merged into empty fields on the primary record.
    
6.  Check the box in the **Duplicate** column next to any record that is for the same person as the primary record. Information from these records is merged into the primary record.
    
    You can also click **Mark All As Dup.** to check all boxes in the Duplicate column.
    
7.  Check the box in the **Not A Duplicate** column next to any record that isn't for the same person as the primary record. These records remain unchanged.
    
    You can also click **Mark All as Not Dup.** to check all boxes in the **Not a Dup** column.
    
8.  Click **Submit Selected** to complete the action you selected in the **Merge Type** field.
    

### Related Topics

-   [Merging or Deleting Duplicate Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N491111.html)
-   [Manage Record Duplicates Page](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4160068263.html)
-   [Merging Records with Active Workflow Instances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3843896859.html)
-   [Status and Timing of Merge Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N491751.html)
-   [Near Match Detection](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_2103425532.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
