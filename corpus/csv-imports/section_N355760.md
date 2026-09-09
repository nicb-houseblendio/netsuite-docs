---
id: "section_N355760"
type: "section"
title: "Setting CSV Import Preferences"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Setting CSV Import Preferences"
parent: "chapter_N343158"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html"
anchors: ["procedure_N355784", "bridgehead_N355884", "bridgehead_N355900", "bridgehead_N356029", "bridgehead_4341167101", "bridgehead_4341168670"]
sha256: "a68267db17acfb1bbf6e465ad746bcc453459a728cd4ddcb00a9623df997db5b"
---

Note:

These preferences don't apply to simple imports.

If you are an account administrator, or you have the Set Up CSV Preferences permission, you can set the following CSV preferences. They appear on the Import Options page and become the default for everyone.

Any changes that users make in the Import Assistant override the default preferences from the CSV Import Preferences page.

#### To set CSV import preferences: {#procedure_N355784}

1.  Go to _Setup > Import/Export > CSV Import Preferences_.
    
2.  On the CSV Import Preferences page, enable or disable options, and click **Save**.
    
    See the sections below for information about available preferences:
    
    -   [Custom Multi-Select Value Delimiter](#bridgehead_N355884)
        
    -   [Log System Notes For Custom Fields](#bridgehead_N355900)
        
    -   [Run Server SuiteScript and Trigger Workflows](#bridgehead_N356029)
        
    -   [CSV Column Delimiter](#bridgehead_4341167101)
        
    -   [CSV Decimal Delimiter](#bridgehead_4341168670)
        

## Custom Multi-Select Value Delimiter {#bridgehead_N355884}

By default, the Import Assistant expects the pipe '|' to be the delimiter for multi-select field values. The Assistant also supports the use of any single character as a custom multi-select delimiter.

To specify that a custom character be used as a delimiter, instead of the pipe, for all import jobs in your account, enter the character in this field. The Import Assistant then interprets the custom character, and not the pipe, to indicate a multi-select relationship. Users can enter an alternate character in the Advanced Options area of the Import Options page, that overrides the account-level character for a specific import job.

## Log System Notes For Custom Fields {#bridgehead_N355900}

Enable this option to create system notes during the import of data from custom fields. This option is disabled by default. Disabling system notes for custom fields improves performance and is preferred for imports that add data.

Important:

System-generated notes are used in NetSuite to track changes to a record, including what action was taken, when the record was modified, and the user that was responsible for the change. These notes are important for maintaining a complete audit trail. If you turn off system-generated notes for custom fields, specific changes related to custom fields within the imported record are **not** recorded in NetSuite, although all changes for standard fields are logged as usual. If a custom field contains sensitive information that is critical for audit purposes, you should **not** disable system-generated notes. For more information about system notes, see [System Notes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158644279544.html).

## Run Server SuiteScript and Trigger Workflows {#bridgehead_N356029}

Enable this option to run any server-side SuiteScript during the CSV imports, but note that it will slow the save process.

You must enable this option if you want a CSV import to trigger workflows based on record creation or updates. If disabled, workflows won't run when records are imported or updated.

You typically should enable this option when you are synching 'live' data or running a partner application (for example, Outlook synchronization).

You should disable this option when you are doing a historical import.

Note:

To enable or disable this option, you must be logged in to NetSuite with a Role that has full permission to:

-   Import CSV File.
    
-   Control SuiteScript and Workflow Trigger per CSV Import.
    

For more information about how to set up permissions for a role, see [Setting Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288727.html) under the [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html) topic.

## CSV Column Delimiter {#bridgehead_4341167101}

By default, the Import Assistant expects comma-separated values. However, you can also import CSV data that uses a different type of separator. Other valid options are the colon (:), semicolon (;), pipe (|), space ( ), and tab.

## CSV Decimal Delimiter {#bridgehead_4341168670}

By default, the Import Assistant expects the period to be used as the decimal mark in numbers. If you use the comma as the decimal mark in the CSV files you import, you can set it to be the default decimal delimiter for CSV data.

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Step One Scan & Upload File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N343532.html)
-   [Step Two Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N344550.html)
-   [Step Three File Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347303.html)
-   [Step Four Field Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N347418.html)
-   [Step Five Save Mapping & Start Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N350233.html)
-   [Setting Integration Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356104.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
