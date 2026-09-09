---
id: "section_N345294"
type: "section"
title: "Choose Data Handling for Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Step Two Import Options > Choose Data Handling for Import"
parent: "section_N344550"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345294.html"
anchors: []
sha256: "f7510a84d55e76e30960229312358eb6259a0863fdd0a75b8294ba0d14aa5dff"
---

On the Import Options page, select a Data Handling option to show how your import will affect NetSuite data:

-   **Add** - Select this if all records in your file are new to NetSuite.
    
-   **Update** - Select this if all records in your file already exist in NetSuite, and you want to update them.
    
-   **Add or Update** - Select this if your import has a mix of new and existing records.
    

Note:

See [Required Permissions for CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345544.html) to get an understanding of the permission level a user must have for a record type to add or update records of that type through CSV import.

Keep these things in mind when updating NetSuite data with CSV imports:

-   The reference type you pick in the Field Mapping step decides how your CSV records are mapped to existing NetSuite records. You can use external ID, internal ID, or name. Using names can cause errors more frequently, because of matching failures. For more info, see [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html).
    
-   By default, NetSuite won't clear out fields if your CSV leaves them blank. You can change this by enabling the Overwrite Missing Fields advanced option. For more info, see [Overwrite Missing Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751050565.html).
    
-   Imports always populate dependent field values automatically when related field values are set, in the same manner that dependent field values are populated in the user interface. For updates, make sure your CSV includes all the necessary values so you don't accidentally change something to a default.
    
-   How sublist data gets updated depends on the Overwrite Sublists option and whether the sublists are keyed. You can set Overwrite Sublists as an advanced option for a job or as a general preference at _Setup > Import/Export > CSV Import Preferences_.
    
    If Overwrite Sublists is enabled, CSV file sublist rows completely replace existing sublist data. If the Overwrite Sublists option is disabled, for keyed sublists, CSV file sublist rows selectively update existing sublist data, and for other sublists, CSV file rows are added to the existing sublist.
    
    For more information about the option, see [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html). To review which sublists are keyed, see [Supported Sublist Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html).
    
-   You can't currently fully delete sublist data. You can only overwrite it with new CSV data, not remove it by leaving blank rows.
    

### Related Topics

-   [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html)
-   [Required Permissions for CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345544.html)
-   [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html)
-   [Use Multiple Threads and Multiple Queues to Run CSV Import Jobs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347015.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
