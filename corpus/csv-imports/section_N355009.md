---
id: "section_N355009"
type: "section"
title: "Including Import Maps and CSV Files in SuiteBundler"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Working with Saved CSV Imports > Including Import Maps and CSV Files in SuiteBundler"
parent: "section_N353796"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html"
anchors: []
sha256: "221549b6607539dcfefb59320009955c97864a6ee48cb20bf27aa831fc60ccc6"
---

Saved import mappings are available on the Saved CSV Imports page, according to the access and audience defined for them, as described in [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html). All of the mappings listed on your Saved CSV Imports page also are available to you in SuiteBundler, a NetSuite tool for packaging customization and configuration objects for sharing among accounts, if you have access to SuiteBundler.

You can add saved import mappings to a customization bundle by selecting the Saved CSV Imports object type in the Bundle Builder.

You also can include CSV files in SuiteBundles. These CSV files may be used as import template files or to store data to be imported. If you want to include a CSV file in a SuiteBundle, upload the file to the File Cabinet, and after it has been uploaded, edit the file record to check the Available for SuiteBundles box, as shown in the following screenshot. The file is then listed under the Files object type in the Bundle Builder, as shown in the above screenshot.

Note:

When including CSV files in a bundle, do not specify default field values, because the target account field values use internal IDs that are different between accounts. SuiteBunder does not remap those values to ones on the target account. After the bundle has been installed in the target account, the default values can be manually mapped using the Import Assistant.

![Available for SuiteBundles box checked on the File upload page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/CSVFileBundle.png)

For more information about using the File Cabinet, see [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html). For information about building SuiteBundles, see [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html).

### Related Topics

-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)
-   [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html)
-   [Sharing Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html)
-   [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
