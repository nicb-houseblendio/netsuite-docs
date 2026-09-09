---
id: "section_N3193361"
type: "section"
title: "Check"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Check"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3193361.html"
anchors: ["bridgehead_1492707626", "bridgehead_1492707675", "bridgehead_N3193403", "bridgehead_N3193514", "bridgehead_156019998577", "bridgehead_156106253149"]
sha256: "3524efd1bcff49b2662e5ba6ac440488680b95de5930b9ce7e7cde6d211cf951"
---

A check transaction creates and records a check used to pay an expense, records an expense paid in cash and not entered as a bill, or records a non-check debit transaction, such as a debit card transaction, ATM (automated teller machine) transaction, or EFT (electronic funds transfer) payment. A check transaction records an expense directly to your books by debiting the expense account specified in the transaction detail and crediting the bank account the check selected for the check.

For help working with this record in the UI, see [Checking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1543613.html).

The internal ID for this record is `check`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/check.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492707626}

The check record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492707675}

The check record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3193403}

The following sections provide usage notes for specific fields and sublists.

## Using Landed Cost Fields {#bridgehead_N3193514}

When you create a landed cost category, the associated field IDs for the first category are landedcostamount1 and landedcostsource1. If you create a second category, the IDs will be landedcostamount2 and landedcostsource2.

This pattern increments by one with each additional category. For example, the IDs for the next landed cost category will be landedcostamount3 and landedcostsource3, and so on.

## Using the Payee Address Sublist {#bridgehead_156019998577}

Payee address data is stored in a subrecord instead of a text field. On the Check form in the UI, the address information is now displayed in a sublist instead of a single field. SuiteScript includes specialized APIs that you must use to script with subrecord data. You should use these subrecord APIs to script with payee address data.

For details about scripting subrecords with SuiteScript 2.x, see:

-   [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html)
    
-   [Record Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html#bridgehead_4273190849)
    
-   [CurrentRecord Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html#bridgehead_4642652726)
    
-   [About the Address Subrecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4706872407.html)
    

Warning:

This change may impact existing scripts that reference check payee address data. You should review these scripts to determine whether updates are needed.

## Using Profit, Cost, and Amount Fields {#bridgehead_156106253149}

The following table provides usage notes for fields on this record related to estimated gross profit and profit percent, estimated extended cost, and amount.

| Field UI Label | Note |
| --- | --- |
| Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |
| Amount | This field is not available using search or lookup for any transactions. |

### Related Topics

-   [Checking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1543613.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
