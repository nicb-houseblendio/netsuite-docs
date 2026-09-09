---
id: "section_N3197042"
type: "section"
title: "Revenue Commitment Reversal"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Revenue Commitment Reversal"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3197042.html"
anchors: ["bridgehead_1493048533", "bridgehead_1493048554", "bridgehead_N3197074"]
sha256: "4e113089f9d84868d5eb8609d72e1e8c97dcad31550775ec0354376fee6af7ac"
---

If a revenue commitment cannot be invoiced, or the revenue and unbilled receivable must be reversed for some reason, a user with sufficient permission must reverse the revenue commitment.

For help working with this record in the UI, see [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html).

The internal ID for this record is `revenuecommitmentreversal`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/revenuecommitmentreversal.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493048533}

The revenue commitment reversal record is scriptable in client and server SuiteScript.

## Supported Functions {#bridgehead_1493048554}

The revenue commitment reversal record is partially scriptable. It can be updated, copied, deleted, and searched using SuiteScript. It cannot be created.

## Usage Notes {#bridgehead_N3197074}

You cannot create this record using the standard [record.create(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258059.html) function. To create a Revenue Commitment Reversal record, you must execute a Return Authorization to Revenue Commitment Reversal transformation. Note that the Return Authorization must be approved and received for the transform to work.

In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

### Related Topics

-   [Creating Revenue Commitment Reversals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1709562.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
