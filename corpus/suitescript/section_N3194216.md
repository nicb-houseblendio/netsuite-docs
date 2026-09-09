---
id: "section_N3194216"
type: "section"
title: "Deposit Application"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Deposit Application"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3194216.html"
anchors: ["bridgehead_1492718896", "bridgehead_1492719531", "bridgehead_1492719396"]
sha256: "3552044ed1013c38633aecae137e2b9062271bdd9fc2e875cdcbe07017e8e982"
---

A deposit application transaction applies a customer deposit against an invoice after the order is complete.

For help working with this record in the UI, see [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html).

The internal ID for this record is `depositapplication`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/depositapplication.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492718896}

The deposit application record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492719531}

The deposit application record cannot be created, but otherwise it is fully scriptable. It can be copied, updated, deleted, and searched in SuiteScript.

## Usage Notes {#bridgehead_1492719396}

You do not use [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html) to create a deposit application record. Deposit applications are always created when a customer deposit is applied to an invoice. The application can only be created by applying an open customer Deposit from the deposit sublist of the customer payment. On submit, the backend creates a deposit application in the amount applied.

You can use the **doc** field on the apply sublist of the customer payment to get the internal ID of the deposit or invoice.

### Related Topics

-   [Applying a Customer Deposit](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1299826.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
