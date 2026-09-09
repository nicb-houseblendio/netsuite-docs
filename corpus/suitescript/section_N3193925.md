---
id: "section_N3193925"
type: "section"
title: "Customer Refund"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Customer Refund"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3193925.html"
anchors: ["bridgehead_1492717774", "bridgehead_1492717850", "bridgehead_N3193965", "bridgehead_156335319751"]
sha256: "5c9e6a00a0c5b49742982570494a6b3ac75bb4950f4ce89c90fc4e3d4ee6dabf"
---

The internal ID for this record is `customerrefund`.

For help working with this record in the UI, see [Customer Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4417991286.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customerrefund.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492717774}

The customer refund record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492717850}

The customer deposit record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3193965}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| ccnumber | Credit Card # | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

The Deposits sublist is a **list** sublist.

## Using the Payee Address Sublist {#bridgehead_156335319751}

Payee address data is stored in a subrecord instead of a text field. On the Customer Refund form in the UI, address information is now displayed in a sublist instead of a single field. SuiteScript includes specialized APIs that you must use to script with subrecord data. You should use these subrecord APIs to script with payee address data.

For details about scripting subrecords with SuiteScript 2.x, see:

-   [SuiteScript 2.x Scripting Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4675623115.html)
    
-   [Record Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html#bridgehead_4273190849)
    
-   [CurrentRecord Object Members](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4625600928.html#bridgehead_4642652726)
    
-   [About the Address Subrecord](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4706872407.html)
    

Warning:

This change may impact existing scripts that reference customer refund payee address data. You should review these scripts to determine whether updates are needed.

### Related Topics

-   [Customer Refunds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4417991286.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
