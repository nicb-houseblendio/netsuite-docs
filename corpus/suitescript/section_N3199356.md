---
id: "section_N3199356"
type: "section"
title: "Transfer Order"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Transfer Order"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199356.html"
anchors: ["bridgehead_1502143965", "bridgehead_1502143979"]
sha256: "248f97bcf5efe3ecddc8120e0226d6bee79957a2b36262e18aa176c6c134d20f"
---

The Transfer Order transaction is used to move inventory between locations when the Multi-Location Inventory (MLI) feature is enabled. Existing integrations with external warehouse management systems can leverage this transaction to manage data about inventory movement between locations.

Transfer orders can initialize item fulfillment and item receipt transactions. See [Item Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3680777.html) and [Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3681685.html) for details about these transactions.

For help working with this record in the UI, see [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html) and [Customer Return Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302852.html).

The internal ID for this record is `transferorder`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/transferorder.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Usage Notes {#bridgehead_1502143965}

## Fields {#bridgehead_1502143979}

| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| --- | --- | --- |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

### Related Topics

-   [Order Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1222915.html)
-   [Customer Return Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1302852.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
