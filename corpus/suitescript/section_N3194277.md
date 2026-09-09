---
id: "section_N3194277"
type: "section"
title: "Estimate"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Estimate"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3194277.html"
anchors: ["bridgehead_1492719919", "bridgehead_1492719963", "bridgehead_N3194318", "bridgehead_1495575725", "bridgehead_1495575714"]
sha256: "edbdb53a44ea856c99effcd194813fa4482c6c36ca73c8a0bf3f0872e861bb98"
---

The internal ID for this record is `estimate`.

For help working with this record in the UI, see [Estimates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069662.html) and [Quotes for Commerce Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4464799196.html).

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/estimate.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492719919}

The estimate / quote record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492719963}

The estimate / quote record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript. It can also be transformed.

## Usage Notes {#bridgehead_N3194318}

See the following sections for more details on working with this record:

-   [Fields](#bridgehead_1495575725)
    
-   [Email Operations](#bridgehead_1495575714)
    

## Fields {#bridgehead_1495575725}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

Also note that this record has available transforms. See the SuiteScript Records Browser for available transforms. In the NetSuite Help Center, see [record.transform(options)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267258715.html) for examples on how to transform records.

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

The Shipping sublist's Shipping Tax Code field, internal ID shippingtaxcode, appears only if per-line taxes have been set on the Item sublist.

## Email Operations {#bridgehead_1495575714}

NetSuite enables a user to email a copy of a transaction to a customer or another recipient.

If you deploy a beforeLoad user event script on a transaction, in general the script executes when the transaction is emailed. In these cases, the sending of the email is considered an operation of type email on the transaction. However, if the companywide preference **Use Popup for Main Transaction Email Button** is enabled, a beforeLoad script will not execute in certain cases, depending on how the email is sent. That is, the script will not execute if the user views the transaction and selects Actions > Email, or edits the transaction and sends the email by using the Communications subtab. In these cases, the system displays a popup window that the user can work with to manually edit and send the email. Actions taken with this window are not considered operations on the transaction. If you have your system configured this way, and you want to deploy a beforeLoad script on emails sent using the popup, deploy the script on the [Message](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3191112.html) record type.

An additional way of emailing a transaction is by editing the transaction and using the Save & Email button. Note that, even if the Use Popup for Main Transaction Email Button preference is enabled, the popup window is not available for emails sent this way. For that reason, a beforeLoad user event script deployed on the transaction will always be triggered by use of the Save & Email button.

For more information about the Use Popup for Main Transaction Email Button preference, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html). For details about emailing transactions, see [Emailing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N513303.html).

### Related Topics

-   [Estimates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069662.html)
-   [Quotes for Commerce Websites](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4464799196.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
