---
id: "section_N3196490"
type: "section"
title: "Opportunity"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Opportunity"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3196490.html"
anchors: ["bridgehead_1492795839", "bridgehead_1492795855", "bridgehead_N3196532"]
sha256: "6ffb4651dd4900f8fb8152c9e2ca8022eab7cd72e3047f541ab2470b4008e4a7"
---

Opportunities represent negotiations with prospects. You must first enable opportunities in your NetSuite account before you can access this record type. To enable opportunities, go to _Setup > Company > Enable Features_. On the CRM subtab, under Sales, select the Opportunities box.

For help working with this record in the UI, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).

The internal ID for this record is `opportunity`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/opportunity.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492795839}

The opportunity record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492795855}

The manufacturing operation task record is fully scriptable. It can be created, copied, updated, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3196532}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

Also note that this record has available transforms. See the SuiteScript Records Browser for available transforms. In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

### Related Topics

-   [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
