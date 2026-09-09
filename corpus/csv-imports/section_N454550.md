---
id: "section_N454550"
type: "section"
title: "State and Province Names for CSV Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Tips for Successful CSV Imports > State and Province Names for CSV Import"
parent: "section_N439220"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454550.html"
anchors: []
sha256: "0ebda5496057ef2b30b151d9cf25f6b4b1c6c185f88a2f9de73cdd5f234e91f2"
---

State and province names in CSV files need to match **Short Name** values listed at _Setup > Company > States/Provinces/Counties_.

![Country list on the States/Provinces/Counties page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/StatesProvincesCountries.png)

NetSuite provides initial system lists of names for several countries. You can add custom states and provinces at _Setup > Company > States/Provinces/Counties_ > New.

If an imported CSV file includes state or province names that don't match current system or custom names, the import job returns an error like 'Invalid state `state_name` for country `country_name` '. If you receive this error, review state and province names in your file, and either make corrections to the file or make additions to system States/Provinces/Counties.

Important:

If a CSV file includes the full names for states or provinces rather than short names, the import job may complete, but state or province values may not be saved correctly. To avoid errors, use short names. For example, importing full names for the Shipping Address Country field in transactions can prevent later calculation of shipping costs.

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
-   [Delimiters for Hierarchical and Multi-Select Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454061.html)
-   [Name References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454355.html)
-   [Country Names for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N454670.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
