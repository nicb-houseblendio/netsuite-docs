---
id: "section_N3197428"
type: "section"
title: "Transaction Search"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Transaction Search"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3197428.html"
anchors: ["bridgehead_1493050069", "bridgehead_1493050093", "bridgehead_N3199185"]
sha256: "a3d9965c25a9f995d1892c90c2bf8b31ef5c8f2d690deb56ed2d75db3dfecb71"
---

Nearly all transaction record types use the TransactionSearch record for search.

For help working with this record in the UI, see [Defining an Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646177.html). For help working with this record by using SuiteScript API, see [N/search Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345764122.html).

The internal ID for this record is `transaction`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/transaction.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/search Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4345764122.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493050069}

The transaction search is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1493050093}

Only search is supported for the transaction search record.

## Usage Notes {#bridgehead_N3199185}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Search Filters and Search Columns** |
| ccnumber | Credit Card # | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| entity | Name | The search filter entity is synonymous for the search filter name. Either filter can be used when searching the value of the Name / ID field in the UI. |

### Related Topics

-   [Main Line in Transaction Search Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4459563851.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
