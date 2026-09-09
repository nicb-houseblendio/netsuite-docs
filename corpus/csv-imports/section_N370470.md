---
id: "section_N370470"
type: "section"
title: "Items Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Items Import"
parent: "chapter_N356211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370470.html"
anchors: []
sha256: "ec9a37f923594c0cf6e0028de144f8873144e26ecd0aafc4843eb6ea4833468f"
---

Item records allow you to track and manage the goods and services your company buys and sells in the course of doing business.

For a list of the types of items that you can add or update with the Import Assistant, see [Item Record Types that Can Be Imported](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N370727.html).

For a table of item sublist data that can be imported, see [Item Sublists Available for Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N371212.html).

To review issues you may encounter when you import Items data, see [Notes about Items Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N372644.html) and [Selecting General Ledger Accounts for Item Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373097.html).

If the Demand Planning feature is enabled in your account, review [Importing Demand Planning Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N373888.html) for information about importing related data.

If the Web Site feature is enabled in your account, review [Importing Related Items Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375476.html).

If the Warehouse Management feature is enabled, you can import data for the following fields: Rotation Type, Item Process Group, and Item Process Family. For more information about working with these fields, see [Creating Items for NetSuite WMS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541433512.html).

For information about using the Import Assistant to set up matrix options for items, see [Importing Matrix Options for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N375701.html).

For tips about importing price levels for items, see [Importing Pricing Data for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N377331.html).

For an example of replacing the contents of a sublist with the content from the CSV import, see [Replacing the Bill of Materials Sublist with the CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4583275282.html).

Important:

Because the Quantity on Hand field isn't available for entry on NetSuite user interface Item forms, CSV imports can add Quantity on Hand values for new item records being imported, but can't update Quantity on Hand values for existing NetSuite item records. The Quantity on Hand field should only be available on the Field Mapping page for Adds, but currently may appear for Updates as well. If you map this field for an update, currently no error occurs, but Quantity on Hand field values are not updated.

For details about fields that can be mapped in Item records, refer to the [SOAP Schema Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/index.html), which has a reference page for each supported item type. You can use the field definitions here as a basis for creating your own CSV import template file. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Using Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2164525.html)

### Related Topics

-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
