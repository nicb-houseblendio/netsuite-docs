---
id: "section_N439392"
type: "section"
title: "Sublist Data Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Sublist Data Import"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439392.html"
anchors: []
sha256: "966733767c8b67dd6046348cf79397e1161294544cdf987ec59d46ae29df6328"
---

Some types of NetSuite records may include sets of related data called sublists. For example, each sales order record includes a set of items. The items data is considered a sublist of sales order. You can use the Import Assistant to import sublist data for some record types. Sublist data can be included in the same file as other record type data, or you can upload a separate file for each sublist's data.

Note:

Some related data may be structured as a subrecord rather than a sublist of a record type. See [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html).

Supported sublist imports vary according to the features that are enabled in your account. For a list of sublists supported for import, see [Supported Sublist Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html).

Note:

Custom sublists aren't available in CSV import.

Some sublists include one or more key fields that can uniquely identify each sublist record. For keyed sublists, imported CSV file sublist data can selectively update or completely overwrite existing sublist data, depending on the [Overwrite Sublists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751046270.html) option. For non-keyed sublists, CSV file sublist data can either be appended to or completely overwrite existing sublist data. Complete deletion of sublist data currently isn't supported.

Be aware that if you don't map any fields for a sublist, no sublist data is imported, even if you set a default value for one or more sublist fields on the Field Mapping page. For information about mapping sublist fields, see [Required Fields for Sublist Import Mapping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html).

Be aware that the CSV Import Assistant allows the import of records without a sublist, even if the sublist contains required fields. The Never Empty option, that makes a sublist required and is available in the UI, isn't supported in CSV import.

For some transaction types, you can update items data during the CSV import. For more information, see [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html).

### Related Topics

-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)
-   [Importing Subrecord Data](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314672015.html)
-   [Supported Subrecord Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4314686228.html)
-   [Effects of Auto-Generated Numbers during Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N452342.html)
-   [General CSV File Conventions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453326.html)
-   [Tips for Using Numbers in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453795.html)
-   [Values in CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453857.html)
-   [Avoiding Errors for Commas and Other Delimiter Symbols within CSV File Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N453950.html)
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [State and Province Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
