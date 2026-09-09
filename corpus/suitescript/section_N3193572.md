---
id: "section_N3193572"
type: "section"
title: "Customer Deposit"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions > Customer Deposit"
parent: "chapter_N3191224"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3193572.html"
anchors: ["bridgehead_1492708642", "bridgehead_1492708685", "bridgehead_N3193613"]
sha256: "34e950c30e0a260015305d07a686df9a1348d5f351ab8266040982ac3d37bc4d"
---

A customer deposit transaction records the funds received when a customer makes an advance payment for an order. This payment is recorded in the general ledger as a liability until the goods or services are delivered, and does not affect the customer's accounts receivable balance. After the order is filled, the deposit is applied against the invoice.

For help working with this record in the UI, see [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html).

The internal ID for this record is `customerdeposit`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customerdeposit.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492708642}

The customer deposit record is scriptable in both client and server SuiteScript.

## Supported Functions {#bridgehead_1492708685}

The customer deposit record is fully scriptable. It can be created, updated, copied, deleted, and searched using SuiteScript.

## Usage Notes {#bridgehead_N3193613}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| ccnumber | Credit Card # | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| isrecurringpayment | Recurring Payment | A value for this field is stored only if the value for paymentmethod is a credit card. |

### Related Topics

-   [Customer Deposits](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1296349.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
