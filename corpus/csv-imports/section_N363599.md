---
id: "section_N363599"
type: "section"
title: "Custom Records Import"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Guidelines for CSV Import Files > Custom Records Import"
parent: "chapter_N356211"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N363599.html"
anchors: []
sha256: "2559fecf4c4d0cff4eccc6cb73f25713456d87414f2dcd98f99bcf7923c9e0b1"
---

A custom record type is an entry form you can create to collect information specific to the needs of your business, when the Custom Records feature is enabled. To enable the Custom Record feature, go to _Setup > Company > Enable Features_, on the SuiteCloud subtab.

For more details, see: [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)

For already existing custom record types, you can use the CSV Import Assistant to:

-   Add new custom record instances
    
-   Update the data in existing custom record instances and sublists
    
-   Delete data from existing custom record instances and sublists
    

When adding a new custom record instance, the Name field is a required field. The Name field can also be used as a reference type when updating or deleting data in existing custom record instances, but it is not a Unique Key. Therefore it is more susceptible to errors because of matching failures. Unique Keys are the External ID (if enabled) and the Internal ID.

For more information about Reference Types, see: [Select Reference Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N349594.html)

For more details about fields that can be mapped in custom records, see the SOAP Schema Browser's [custom record](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/customrecord.html) reference page. For information about working with the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

When you create new custom record instance through CSV Import, it is possible to import values for the Translations sublist, if the Enable Name Translation field is enabled for the corresponding custom record type. For more details on configuring a custom record type to allow for translations, see [Translating Custom Record Instance Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_3746164319.html).

The Import Assistant is available at _Setup > Import/Export > Import Tasks > Import CSV Records_. For more information about the Import Assistant, see: [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)

### Additional Information

-   [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html)
-   [CSV Import Error Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4568635774.html)
-   [Custom Records Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2875173.html)
-   [Custom Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2826978.html)

### Related Topics

-   [Guidelines for CSV Import Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N356211.html)
-   [Supported Record Types for CSV Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N356360.html)
-   [Tips for Successful CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N439220.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
