---
id: "section_N454061"
type: "section"
title: "Delimiters for Hierarchical and Multi-Select Fields"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Delimiters for Hierarchical and Multi-Select Fields"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html"
anchors: ["bridgehead_N454126"]
sha256: "8c1ea475dbf386fb5ee4e500692989781f17a8121b0abf817a0e4e95a15408fb"
---

When importing records that contain hierarchical relationships, use a colon ':' as the field delimiter. If relationships are multi-tiered, place a colon between each record and subrecord. Place a space between each value and each delimiter.

If there is a hierarchy in a user interface dropdown list, then the CSV file requires the colon delimiter, even if a colon doesn't display in the UI dropdown list.

-   For multi-select field values, the default delimiter is a pipe '|' . You can specify a different single character to be used instead of the pipe, for an import job. Set this value on the Import Assistant's Import Options page, in the Advanced Options section. For information, see [Set Advanced CSV Import Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N345887.html).
    
-   If you're an administrator, you can specify a different character be used for all import jobs in the account, on the CSV Import Preferences page. For information, see [Setting CSV Import Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355760.html).
    
-   The user-level character set as an advanced option for an import job overrides the account-level character, for that import job.
    
-   In your CSV files' multi-select fields, leave a space between each value and each delimiter.
    

## Example Hierarchical Delimiters {#bridgehead_N454126}

In this example, Solution 1 is associated with Topic B, which is a Subtopic of A. Solution 2 is associated with Topic Z, a Subtopic of Y, which is a Subtopic of X. The colon ':' is the field delimiter. You signify the hierarchy between items using the colon in the topic column.

| Solution | . . . | Topic | Is Inactive |
| --- | --- | --- | --- |
| 1 | . . . | A : B | FALSE |
| 2 | . . . | X : Y : Z | FALSE |

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Sublist Data Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
