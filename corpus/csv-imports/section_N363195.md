---
id: "section_N363195"
type: "section"
title: "Messages Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Communications Import Type > Messages Import"
parent: "section_N363101"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363195.html"
anchors: []
sha256: "cd0b7f70dc6ebe792fb5e1e141720ef42e590e8507c74ff694a58ab8dac6baae"
---

The Messages import adds message records to NetSuite. Messages are used to attach email messages to NetSuite entities and transactions.

The fields available for messages imports correspond to those on the Recipients and Messages subtabs of the Attach Message dialog. This dialog appears when a user clicks Attach on the Messages subtab of one an entity or transaction record.

For details about fields that can be mapped in the Message record, see the SOAP Schema Browser's [message](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/message.html) reference page. You can use the field definitions as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note the following:

-   Because messages are not editable in the UI, they're not editable through CSV import. You can use CSV import to add new message records only, not to edit existing message records. For messages imports, the **Update** and **Add or Update** data handling options are unavailable on the Step 2 Import Options page of the Import Assistant.
    
-   Required messages fields for import are: From (the sender of the message), Attach to (the recipient of the message and the record to which the message is attached in NetSuite), and Subject (which also serves as a title). Entities provided as From and Attach to field values must already exist in NetSuite. If the From and Attach to entity records don't have email addresses, then the From Email Address and To (Email) fields are required.
    
-   Unlike in the user interface, the Attach to field doesn't default to be the logged in user. You need to include values for this field in your CSV file or set up a default on the Import Assistant Field Mapping page. See [Assign Default Values during Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349918.html).
    
-   To attach messages to transactions, map the Transaction field, and either set a default value or include transaction values in the CSV file.
    
-   The Emailed field is a that indicates whether an email message was sent. Messages imports don't send any email messages.
    
-   Import of file attachments isn't supported, although files can be attached to messages in the NetSuite user interface.
    

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. After you select the record type for import, choose the import character encoding. For more information, see [Select a Record Type for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344030.html) and [Choose Import Character Encoding](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344158.html).

### Related Topics

-   [Communications Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363101.html)
-   [Notes Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363414.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
