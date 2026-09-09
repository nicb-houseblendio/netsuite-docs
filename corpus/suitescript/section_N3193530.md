---
id: "section_N3193530"
type: "section"
title: "Credit Memo"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Credit Memo"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3193530.html"
anchors: ["bridgehead_1492708525", "bridgehead_1492708555", "bridgehead_1495573690", "bridgehead_1502143670"]
sha256: "a33d41bee99436469fbda5723671e29746226d1d1582ec1d2207e0155bc77fc5"
---

A credit memo transaction decreases the amount a customer owes you. This type of transaction can be used to reverse a charge billed to a customer. If a customer receives a credit memo after they have paid an invoice, this memo can be applied to any of the customer's open or future invoices.

For help working with this record in the UI, see [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html).

The internal ID for this record is `creditmemo`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/creditmemo.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492708525}

The credit memo record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492708555}

The credit card refund record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_1495573690}

NetSuite enables a user to email a copy of a transaction to a customer or another recipient. There are several ways to email a transaction. One way is to open the transaction for viewing and select Actions > Email. Additional approaches for emailing transactions are described in [Emailing Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N513303.html).

If you deploy a beforeLoad user event script on a transaction, in general the script executes when the transaction is emailed. In these cases, the sending of the email is considered an operation of type email on the transaction record. However, if the companywide preference Use Popup for Main Transaction Email Button is selected, a beforeLoad script will not execute when a user selects Activity > Email. In this case, the system displays a popup window that the user can work with to manually edit and send the email. Actions taken with this form are not considered operations on the transaction. If you have your system configured this way, and you want to deploy a beforeLoad script on emails sent using the popup, deploy the script on the [Message](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3191112.html) record type.

Note that the Use Popup for Main Transaction Email Button preference does not affect other methods of emailing a transaction. For example, a user may email a transaction by using its Communications subtab or by using the Save and Email button. In these cases, a beforeLoad user event script deployed on the transaction still executes, regardless of how the preference is configured. For more information about the Use Popup for Main Transaction Email Button preference, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html).

The Multi-Partner Management feature must be enabled in your account for the Partners sublist to appear.

## Fields {#bridgehead_1502143670}

| estgrossprofit | Est. Gross Profit | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| --- | --- | --- |
| estgrossprofitpercent | Est. Gross Profit Percent | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. When this field appears on the sublist line level, this field is not scriptable. |
| totalcostestimate | Est. Extended Cost | When this field is on the body of the form in edit mode, this field is scriptable and can be returned in a transaction search. |

### Related Topics

-   [Customer Credit Memos](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1311306.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
