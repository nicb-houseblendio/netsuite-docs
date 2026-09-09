---
id: "section_N3203206"
type: "section"
title: "Subsidiary"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Lists > Subsidiary"
parent: "chapter_N3200673"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3203206.html"
anchors: ["bridgehead_1492455335", "bridgehead_1492455346", "bridgehead_4744107425"]
sha256: "39b349d5f097d5b39642fec7b9fda66e9a1d4962090c148ae70aa4f7db4e5e24"
---

A NetSuite OneWorld account enables you to manage data for a hierarchical structure of separate legal entities, or subsidiaries. This structure is organized as a tree that rolls up to a root, or top-level parent subsidiary. The root subsidiary is the highest-level subsidiary in your account, and all other subsidiaries are below it in the hierarchy. If an account that is upgraded to OneWorld has preexisting data, this data is used for the root subsidiary.

Each subsidiary represents a separate company within your global organization. Subsidiaries can be international or domestic. When you create a subsidiary record in NetSuite, the country you define for its address determines the NetSuite edition and tax nexus associated with that subsidiary.

For help working with this record in the UI, see [Subsidiaries in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N268563.html) and [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html).

The internal ID for this record is `subsidiary`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/subsidiary.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492455335}

The subsidiary record is supported in client and server SuiteScript.

## Supported Functions {#bridgehead_1492455346}

The subsidiary record is fully scriptable, which means that it can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_4744107425}

The Company Information page and the root Subsidiary record share information. In OneWorld accounts, if you update shared fields on the Company Information page, the corresponding fields on the root Subsidiary record are also updated. An update to the Company Information page also triggers all user event scripts deployed on the Subsidiary record. If your script updates a shared field on the Subsidiary record, the corresponding field on the Company Information page is also updated.

The Subsidiary record is hidden in accounts that are not OneWorld, but the record still exists. You cannot deploy a stand-alone user event script on the Subsidiary record in accounts that are not OneWorld. You can, however, bundle your script and distribute it to these accounts. In this scenario, updates to the Company Information page trigger the of the bundled script.

You can create up to 249 subsidiary records in addition to the root subsidiary, for a total of 250.

On some records, the Subsidiary field is a multi-select field type. When executing a search containing multi-select fields, SuiteScript treats commas as a delimiter of values. Therefore, you should avoid using commas in subsidiary record names. If you do not, subsidiary record names containing a comma can skew your search results.

### Related Topics

-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3200673.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
