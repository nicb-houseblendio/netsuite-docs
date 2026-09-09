---
id: "section_N451547"
type: "section"
title: "Required Fields for Sublist Import Mapping"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > Sublist Data Import > Required Fields for Sublist Import Mapping"
parent: "section_N439392"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451547.html"
anchors: ["bridgehead_N451690"]
sha256: "f7ef8c45229a81523c6106ae9463caea2aa69d671cd36a88737efbd260089c9f"
---

Generally, fields marked (Req) on the Import Assistant Field Mapping page must be mapped for an import to proceed. These fields automatically display in the center pane of the Field Mapping page to make it clear that they must be mapped.

However, you don't always need to map sublist fields that are marked (Req), as these fields are only required if you're importing sublist records. For example, the Vendor field in the Item Vendors sublist is only required if you map one or more fields from this sublist.

![Field Mapping example.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/SublistReqField.png)

The Import Assistant determines whether you're importing sublist records, and whether to treat mapping of the sublist's required fields as required for import, based on your selection of **One File to Upload** or **Multiple Files to Upload** on the Scan & Upload CSV File page:

-   If you choose a single file upload, the Import Assistant doesn't assume that you're importing any sublist data, so sublist required fields don't display in the center pane of the Field Mapping page and aren't required for import.
    
-   If you choose a multiple file upload, meaning one primary file for the record type and one or more linked files for sublists, the Import Assistant assumes you're importing data for each sublist that has a linked file, and sublist required fields display in the center pane of the Field Mapping page.
    

Processing for Import Assistant updates handles the addition and removal of fields, in the same manner as the user interface. If an import adds a field that depends on other required fields, these other required fields are added. If an import removes a required field, all of its fields are removed as well.

If a sublist field has the same name as a required body field, the required sublist field is automatically mapped. For an import where you're adding records, you can remove the required sublist field from the mapping if needed.

Note:

The Import Assistant handles Items sublist required fields for some transactions imports differently, because items are required to add new records of these types, but not for updates to existing records. See [Required Items Sublist Fields for Transactions Imports](#bridgehead_N451690).

For a single file upload, if you attempt to map a sublist field on the Field Mapping page, the system displays a pop-up dialog. This dialog states that if you map the field, you must map all required fields for the sublist. After you click OK, the sublist's required fields display in the center pane so you can map them.

## Required Items Sublist Fields for Transactions Imports {#bridgehead_N451690}

The Import Assistant provides special handling of Items sublist required fields for the following transactions imports: Cash Sale, Estimate, Invoice, Purchase Order, Sales Order, Vendor Bill, Vendor Credit, and Vendor Return Authorization imports. This handling is necessary because new records for these transactions can't be saved without any items. The import of Items sublist data is always required when new records are imported for these transaction types, but is not required when updated records are imported for these transaction types. (For Opportunity imports, Items sublist data is never required.)

The Import Assistant determines whether you're importing Items sublist records for transactions, and whether to treat mapping of the Items sublist's required fields as required for import, based on your selection of **Add, Update**, or **Add or Update** data handling on the Import Options page

-   If you select **Add**, Items required fields display in the center pane of the Field Mapping page and you're required to map these fields.
    
-   If you select **Update**, or **Add or Update**, Items required fields don't display in the center pane of the Field Mapping page and you're not required to map these fields.
    
    If you then attempt to map an Items sublist field on the Field Mapping page, you receive a warning that you must map Items required fields. When you click OK, the Items sublist's required fields display in the center pane so you can map them.
    

You can create a saved CSV import without the items sublist to add transactions without items. However, each time you run the import, the sublist Item field appears in the mapping. If you're not importing items, remove the sublist Item field from the mapping.

### Related Topics

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Supported Sublist Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439528.html)
-   [Importing Sublist Data in a Single File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493384282.html)
-   [Multiline Sublists for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1493796058.html)
-   [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html)
-   [Line Item Updates on Transactions Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N451889.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
