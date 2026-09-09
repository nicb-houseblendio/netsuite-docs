---
id: "section_N3199397"
type: "section"
title: "Vendor Bill"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Vendor Bill"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3199397.html"
anchors: ["bridgehead_1493051520", "bridgehead_1493051555", "bridgehead_N3199439", "bridgehead_N3199551", "bridgehead_4471669833"]
sha256: "ac011a1e614e55c3e1ed67fd419aac199ea5bd0ff65ee16f0f7ec611ec661733"
---

The vendor bill transaction records payables as they arrive from vendors, allowing you to pay bills from the payables list as they are due, and providing an accurate picture of payables at all points of the billing cycle.

For help working with this record in the UI, see [Vendor Bills](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2370131.html).

The internal ID for this record is `vendorbill`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/vendorbill.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1493051520}

The vendor bill record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1493051555}

The vendor bill record is fully scriptable, which means that the record can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3199439}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |
| usertotal | Amount | This field is not available using search or lookup for any transactions. |

## Using Landed Cost Fields {#bridgehead_N3199551}

When you create a landed cost category, the associated field IDs for the first category are landedcostamount1 and landedcostsource1. If you create a second category, the IDs will be landedcostamount2 and landedcostsource2.

This pattern increments by one with each additional category. For example, the IDs for the next landed cost category will be landedcostamount3 and landedcostsource3, and so on.

## Using the Payee Address Sublist {#bridgehead_4471669833}

Payee address data is stored in a subrecord instead of a text field. On the Bill Payment form in the UI, address information is now displayed in a sublist instead of a single field. SuiteScript includes specialized APIs that you must use to script with subrecord data. You should use these subrecord APIs to script with payee address data.

For details about scripting subrecords with SuiteScript 2.x, see:

-   [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html)
    
-   [Record Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html#bridgehead_4273190849)
    
-   [CurrentRecord Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html#bridgehead_4642652726)
    
-   [About the Address Subrecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4706872407.html)
    

Warning:

This change may impact existing scripts that reference bill payee address data. You should review these scripts to determine whether updates are needed.

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
