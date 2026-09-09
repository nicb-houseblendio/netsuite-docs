---
id: "section_N391803"
type: "section"
title: "Importing Entities and Contacts Together"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Relationships Import Type > Importing Entities and Contacts Together"
parent: "section_N383063"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N391803.html"
anchors: ["bridgehead_N391973", "bridgehead_N392068", "bridgehead_N392099", "bridgehead_N392162", "bridgehead_N392274", "bridgehead_N392310", "bridgehead_N392616"]
sha256: "db57b52b084bf2aa4096f67b8ea04531a3cc3f0afe30a3a9e5456bd3a2f77950"
---

It is now possible to import data for Contacts and some entities together, meaning you can import the following types of records with a single Import Assistant job:

-   Customers and Contacts
    
-   Leads and Contacts
    
-   Prospects and Contacts
    

Review the following guidelines for importing entities and contacts together:

-   [Requirements for Importing Entities and Contacts in a Single Job](#bridgehead_N391973)
    
-   [Benefits of Importing Related Records Together](#bridgehead_N392068)
    
-   [Importing Address Sublist Data for Contacts](#bridgehead_N392099)
    
-   [Setting the Global Subscription Status Field for Entities and Contacts](#bridgehead_N392162)
    
-   [Subsidiary Field Not Required for Entities and Contacts in OneWorld](#bridgehead_N392274)
    
-   [Steps for Importing Entities and Contacts Together](#bridgehead_N392310)
    
-   [Import Job Processing for Entities and Contacts Imports](#bridgehead_N392616)
    

## Requirements for Importing Entities and Contacts in a Single Job {#bridgehead_N391973}

-   You can use one CSV file that contains both entity and contact data, or you can use two separate files, one containing entity data and one containing contact data.
    
    -   If you use one file, contact field values are stored by column, and you're limited to importing five contacts per entity in each import.
        
    -   If you use two files, contact field values are stored by row, and this limitation on imported contacts per entity doesn't apply.
        
-   If you use two files, you need to complete the File Mapping page of the Import Assistant to define a column in the contact data file that maps to the primary key column in the entity data file, such as Customer ID. (So if the Contacts CSV file doesn't include this column, you should add it before the import.)
    
-   You must ensure that the [Ignore Read Only Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046796.html) advanced option is enabled.
    
-   Whether you use one or two files, you can map required fields for both entities and Contacts in one step on the Import Assistant's Field Mapping page.
    
    You have the option of mapping the Attached Role field for Contacts. This field describes how the Contact is attached to the entity. Standard role values include Alternate Contact, Primary Contact, Consultant, and Decision Maker.
    

Important:

The Customers and Contacts single job import doesn't support the import of contact access data, such as password, login, and role. You can import this data in a separate Customers Only import after your Customers and Contacts import has completed successfully. See [Importing NetSuite Access Details for Customer Contacts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html#bridgehead_N385500).

When you import entities and contacts together with the **Update** or the **Add or Update** options, all fields in the contact records that have a default value in the UI will take the default value. This happens even if you have given a different value to these fields in your CSV file. If you want to update the value of such fields for contacts, you must use the **Contacts Only** import.

## Benefits of Importing Related Records Together {#bridgehead_N392068}

Combining related records has the following advantages:

-   The process is quicker and easier, as you can import both record types during the same import, rather than requiring two distinct imports.
    
-   You're no longer forced to rely on name matching to link contacts and entities together, which can be prone to inaccuracy.
    

## Importing Address Sublist Data for Contacts {#bridgehead_N392099}

When you import entities and contacts together, the Address sublist for contacts isn't available for mapping. However, the address sublist values imported for each entity (customer, lead, or prospect) record are copied to all of the entity's contacts. If a contact already has one or more addresses, the newly imported address data is added; it doesn't overwrite existing address data.

When you map the fields in the entity's Address sublist, their values are imported to the Address subrecords on entity records and copied to the Address subrecords on all related contact records.

By default, the entity Address field is read-only, and data from other address sublist fields is copied into it. If you map the Override field and set it to Yes (meaning true), you can import data for the Address field.

## Setting the Global Subscription Status Field for Entities and Contacts {#bridgehead_N392162}

The Global Subscription Status field on lead, prospect, customer, and contact records determines whether these entities can receive email sent through campaigns and email merge operations.

-   Four values are possible: Confirmed Opt-In, Soft Opt-In, Soft Opt-Out, and Confirmed Opt-Out, but only the soft values are available to be set by import.
    
-   If you want to send campaign email, set this field's value to Soft Opt-In, because you can't send a campaign email to users with Soft Opt-Out status; you can only send an opt-in email.
    
    Note:
    
    Certain jurisdictions, such as the European Union (EU), have regulations regarding whether you can contact entities if you don't have their explicit permission to do so. You should check that your global subscription status adheres to the regulations in the recipient's jurisdiction.
    
-   If you don't include this field in an import, its value is defaulted, based on the Unsubscribed to Marketing By Default option at _Setup > Marketing > Marketing Preferences_. By default, this option is disabled, and the Global Subscription Status field defaults to Soft Opt-In. When this option is enabled, the field defaults to Soft Opt-Out.
    
-   After an import, you can change the value of the Global Subscription Status between Soft Opt-In and Soft Opt-Out manually in the user interface and through mass updates. Only recipients themselves can change the value to Confirmed Opt-In or Confirmed Opt-Out.
    

For more information about global subscription statuses, see [Subscription Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N994827.html).

## Subsidiary Field Not Required for Entities and Contacts in OneWorld {#bridgehead_N392274}

If your account is using NetSuite OneWorld, the Subsidiary field is a required field for importing entities and contacts together.

The Subsidiary field is not required for importing entities and contacts together only in an account that is not a OneWorld account.

#### Steps for Importing Entities and Contacts Together {#bridgehead_N392310}

1.  Before you start the Import Assistant, review one of the following topics to get some background information about entity imports: [Customers Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383794.html), [Leads Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N386282.html), or [Prospects Only Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N389753.html).
    
2.  Ensure that each CSV file includes required columns.
    
    If you're using two files for the import, the file containing Contacts data should include a column with values that map to the entities' primary key field values. You will need to map the two files' key columns on the Import Assistant's File Mapping page.
    
3.  Start the Import Assistant by going to _Setup > Import/Export > Import CSV Records_.
    
4.  On the Scan & Upload CSV File page:
    
    1.  Choose the import's record type:
        
        -   Customers and Contacts Together
            
        -   Leads and Contacts Together
            
        -   Prospects and Contacts Together
            
    2.  If needed, change the default character encoding. For information, see [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).
        
    3.  Choose the number of files to upload:
        
        -   One file to upload
            
        -   Multiple files to upload
            
    4.  Click the Select buttons and browse to the CSV files for entities and contacts data.
        
        If you also are importing sublist data, you can select files for sublist data as well. For information, see [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html).
        
    5.  After you have selected one or more files to upload, click Next.
        
5.  On the Import Options page:
    
    1.  Select a Data Handling option.
        
    2.  If needed, expand the Advanced Options and make changes. For information, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html). Note that the Ignore Read-Only Fields advanced option must be enabled.
        
    3.  Click Next.
        
6.  (If you're uploading multiple files only) On the File Mapping page:
    
    1.  Select a key column for the CSV file containing entity data. (The Import Assistant refers to this file as the Primary File.)
        
    2.  Select the Contacts column containing values to be mapped to entity key values.
        
    3.  Click Next.
        
7.  On the Field Mapping page, review the Import Assistant's auto mappings shown in the center pane.
    
    1.  Note that Contact fields may be mapped multiple times so that multiple linked contacts can be imported for each entity.
        
    2.  Make sure that required fields (fields marked Req. in the center pane) are mapped. You can set default values by clicking the edit icon.
        
    3.  Click Next.
        
    4.  If necessary, correct any mapping errors.
        
8.  On the Save Mapping and Start Import page, provide a mapping name and, optionally, a description, then click Save and Run.
    

## Import Job Processing for Entities and Contacts Imports {#bridgehead_N392616}

The following table illustrates the actions taken during job processing for imports of Customers, Leads, or Prospects together with Contacts. This processing varies based on the following:

-   Data handling option (Add, Update, Add or Update)
    
-   Reference type (Name, Internal ID, External ID)
    
-   Whether auto-generated numbering is enabled
    

| Matching Conditions | Add | Update | Add or Update |
| --- | --- | --- | --- |
|  |  |  |  |
| **Name Matching** | \- | \- | \- |
| No Matching Entity, No Matching Contact | Add Both | Fail Both | Add Both |
| No Matching Entity, 1 Matching Contact | Fail Both | Fail Both | Add Entity, Update Contact |
| No Matching Entity, 2 Matching Contacts | Fail Both | Fail Both | Fail Both |
|  |  |  |  |
| 1 Matching Entity, No Matching Contact | 
Add Both if Auto-GeneratedNumbering

Else Fail Both



 | Fail Both | Update Entity, Add Contact |
| 1 Matching Entity, 1 Matching Contact | Fail Both | Update Both | Update Both |
| 1 Matching Entity, 2 Matching Contacts | Fail Both | Fail Both | Fail Both |
|  |  |  |  |
| 2 Matching Entities, No Matching Contact | 

Add Both if Auto-GeneratedNumbering

Else Fail Both



 | Fail Both | Fail Both |
| 2 Matching Entities, 1 Matching Contact | Fail Both | Fail Both | Fail Both |
| 2 Matching Entities, 2 Matching Contacts | Fail Both | Fail Both | Fail Both |
|  |  |  |  |
| **Internal ID or External ID Matching** | \- | \- | \- |
| No Matching Entity, No Matching Contact | Add Both | Fail Both | Add Both |
| No Matching Entity, 1 Matching Contact | Fail Both | Fail Both | Add Entity, Update Contact |
|  |  |  |  |
| 1 Matching Entity, No Matching Contact | 

Add Both if Auto-GeneratedNumbering

Else Fail Both



 | Fail Both | Update Entity, Add Contact |
| 1 Matching Entity, 1 Matching Contact | Fail Both | Update Both | Update Both |

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Lead Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1086131.html)

### Related Topics

-   [Relationships Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N383063.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
