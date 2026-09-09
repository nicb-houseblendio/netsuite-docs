---
id: "section_N430392"
type: "section"
title: "Importing Transaction Item Options"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Transactions Import Type > Importing Transaction Item Options"
parent: "section_N405613"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N430392.html"
anchors: []
sha256: "9d1f20bbe3870e95a713e0477275f1e32033f335b3a049b4fae2f3f613edf964"
---

When the Item Options feature is enabled, transaction item options can be created and imported in your account. Transaction item options are custom fields that may be included in transaction line items to represent item-specific choices. When you import transaction records, you can import transaction item options along with Items sublist data.

To be available for import, transaction item options must first be set up at _Customization > Lists, Records, & Fields > Transaction Item Options > New_. The setup of a transaction item option includes selecting the types of transactions to which the item option can be applied. See [Creating Custom Transaction Item Options](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2828730.html).

![Item Option page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TransItemOption_2014_2.png)

The Import Assistant Field Mapping page includes item options as a flat list under the Items sublist folder. Only the item options that have been set up to apply to the type of transaction being imported are included. Each item option is prefixed with the word 'Options' and is marked as a custom field.

![Item Options in the Items sublist folder.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TransItemOptionMap.png)

To import values for a transaction item option, you must map it to a column in the CSV file.

![Edit icon on the Field Mapping page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TransItemOptionMapPencil.png)

You can click the edit icon to select a default or null value for an item option.

![Default Value window with the Provide Default Value field options.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/TransItemOptionDefValue.png)

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)

### Related Topics

-   [Transactions Import Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N405613.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
