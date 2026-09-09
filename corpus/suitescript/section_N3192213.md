---
id: "section_N3192213"
type: "section"
title: "Cash Refund"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Cash Refund"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3192213.html"
anchors: ["bridgehead_1492705773", "bridgehead_1492705807", "bridgehead_N3192255", "bridgehead_1495581215", "bridgehead_1495581258"]
sha256: "9794607cc409aca90d1cb056b4b5c4139f706fd7dc0a01d2646e67a8e7fd5da9"
---

A cash refund transaction records the return of money to a customer who immediately paid for goods or services using cash, a check or a credit card.

For help working with this record in the UI, see [Refunding a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1247359.html).

The internal ID for this record is `cashrefund`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/cashrefund.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492705773}

The cash refund record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492705807}

The cash refund record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3192255}

See the following sections for more details on working with this record:

-   [Fields](#bridgehead_1495581215)
    
-   [Email Operations](#bridgehead_1495581258)
    

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

## Fields {#bridgehead_1495581215}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| ccnumber | Credit Card # | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

## Email Operations {#bridgehead_1495581258}

NetSuite enables a user to email a copy of a transaction to a customer or another recipient.

If you deploy a beforeLoad user event script on a transaction, in general the script executes when the transaction is emailed. In these cases, the sending of the email is considered an operation of type email on the transaction. However, if the companywide preference **Use Popup for Main Transaction Email Button** is enabled, a beforeLoad script will not execute in certain cases, depending on how the email is sent. That is, the script will not execute if the user views the transaction and selects Actions > Email, or edits the transaction and sends the email by using the Communications subtab. In these cases, the system displays a popup window that the user can work with to manually edit and send the email. Actions taken with this window are not considered operations on the transaction. If you have your system configured this way, and you want to deploy a beforeLoad script on emails sent using the popup, deploy the script on the [Message](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3191112.html) record type.

An additional way of emailing a transaction is by editing the transaction and using the Save & Email button. Note that, even if the Use Popup for Main Transaction Email Button preference is enabled, the popup window is not available for emails sent this way. For that reason, a beforeLoad user event script deployed on the transaction will always be triggered by use of the Save & Email button.

For more information about the Use Popup for Main Transaction Email Button preference, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html). For details about emailing transactions, see [Emailing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N513303.html).

### Related Topics

-   [Refunding a Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1247359.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
