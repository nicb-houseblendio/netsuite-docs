---
id: "section_N673560"
type: "section"
title: "Searching System Notes"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Auditing Data Changes using Searches > Searching System Notes"
parent: "chapter_4774167775"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N673560.html"
anchors: ["subsect_159171041562", "bridgehead_4448302226", "bridgehead_4508845103", "procedure_N674874"]
sha256: "e5ee8ca82457a950a00a28b4351f8d22f5c187b5a726c6f4bb339c8169d19700"
---

Note:

Unless identified as System Notes v2, this topic applies to System Notes only. For information about searching System Notes v2, see [Searching and Filtering System Notes v2](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159499608205.html).

System note records show changes made to NetSuite records. NetSuite offers a system note search that you can use to retrieve system notes data.

To use this search, go to _Reports > New Search_ and click **System Note.**

-   Use a simple search to retrieve system notes data filtered by: the user(s) who entered the changes, role of the user who entered the changes, the date and time of the changes, the type of change, the field(s) changed, the value before the changes, the context for the change, and the value after the changes. For information, see [Defining a Simple Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N645582.html).
    
-   Use an advanced search for more filtering and display options. For information about the capabilities available, see [Defining an Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646177.html).
    
-   Use a saved search to take advantage of additional functionality such as emailing search results and the ability to quickly rerun the search. For information, see [Defining a Saved Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N676039.html).
    

System notes fields also are available to be used as filters and displayed as results for other record types' advanced and saved searches, including the following: contact, customer, employee, issue, item, project, opportunity, partner, transaction, and vendor.

## Searching System Notes v2 {#subsect_159171041562}

For information about searching in System Notes v2, see [Viewing System Notes v2](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_158108595525.html) and [Searching and Filtering System Notes v2](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159499608205.html).

## System Notes and Deleted Records {#bridgehead_4448302226}

-   System Notes for existing records are never automatically deleted. System Notes are only deleted when the record they belong to is deleted.
    
-   System Notes v2 are never deleted, even in cases where a record is deleted.
    
-   In some cases, NetSuite creates a log of the deleted record. The log provides some basic information about the deleted record. For more information, see [Searching for Deleted Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4031815869.html).
    

## System Notes for Changes to Configuration and Setup Pages {#bridgehead_4508845103}

System notes log changes made to enabled features, company information, and account-level preferences, such as:

-   Company Information (_Setup > Company > Company Information_)
    
-   Enable Features (_Setup > Company > General Preferences_)
    
-   General Preferences (_Setup > Company > Enable Features_)
    
-   Expense Categories (_Setup > Accounting > Expense Categories_)
    
-   Accounting Lists: Payment Method (_Setup > Accounting > Accounting Lists_)
    
-   Accounting Lists: Term (_Setup > Accounting > Accounting Lists_)
    
-   Accounting Lists: Cost Category (_Setup > Accounting > Accounting Lists_)
    
-   Accounting Lists: Budget Category (_Setup > Accounting > Accounting Lists_)
    
-   Accounting Lists: Subscription Term (_Setup > Accounting > Accounting Lists_)
    
-   Accounting Preferences (_Setup > Accounting > Accounting Preferences_)
    
-   Location Costing Groups (_Setup > Accounting > Setup Tasks > Location Costing Groups_)
    
-   Nexuses (_Setup > Accounting > Nexuses_)
    
-   Tax Types (_Setup > Accounting > Tax Types_)
    
-   Tax Codes (_Setup > Accounting > Tax Codes_)
    
-   Tax Groups (_Setup > Accounting > Tax Groups_)
    

You can create a saved search that shows system notes on features that were enabled by selecting Enable Features in the Record Type dropdown when you define your search.

## Other Methods for Viewing System Notes {#procedure_N674874}

NetSuite offers different methods that you can use to view system notes for particular record types.

-   The audit trail function enables you to retrieve filtered sets of system notes for a selected record type. For information about using the audit trail, see [Viewing an Audit Trail for a Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N675070.html) and [Using the Transaction Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556825.html).
    
-   Each transaction record includes a System Notes subtab on the History subtab where you can view system notes for that transaction. See [Viewing Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555355.html). History for individual line items also may be available from transaction records. See [Line-Level Audit Trail for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557476.html).
    
-   Each record of a type other than transaction, such as Employee or Customer, includes a System Notes subtab on the General subtab. You can view system notes for the record on the System Notes subtab.
    

### Related Topics

-   [Auditing Data Changes using Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4774167775.html)
-   [Viewing an Audit Trail for a Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N675070.html)
-   [Searching for Deleted Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4031815869.html)
-   [Understanding the Context for Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4032860783.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
