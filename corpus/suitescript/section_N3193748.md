---
id: "section_N3193748"
type: "section"
title: "Customer Payment"
branch: "suitescript"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteScript > SuiteScript Records Guide > SuiteScript Supported Records > Transactions-related Records > Customer Payment"
parent: "article_160518507969"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3193748.html"
anchors: ["bridgehead_1492708796", "bridgehead_1492708830", "bridgehead_N3193789"]
sha256: "7d686e838519c021b8cc27f500da5cedc731228109904c7fb062fc1b0841accd"
---

When a customer makes a payment, record the payment and apply it to the appropriate invoice or cash sale. Applying a payment decreases the amount due and tracks income.

For help working with this record in the UI, see [Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html).

The internal ID for this record is `customerpayment`.

See the [SuiteScript Records Browser](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/script/record/customerpayment.html) for all internal IDs associated with this record.

Note:

For information about using the SuiteScript Records Browser, see [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html) in the NetSuite Help Center.

Important:

When the apply sublist appears on the customer payment record, the Apply subtab is visible, however, all apply sublist data appears on a subtab called Invoice. Also, note that the UI label for the **Amt. Due** (due) field can also appear as **Amount Remaining**.

For information about scripting with this record in SuiteScript, see the following help topics:

-   [SuiteScript 2.x Scripting Records and Subrecords](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4675582755.html)
    
-   [SuiteScript 2.1 Custom Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1518455588.html)
    
-   [N/record Module](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4267255811.html)
    

## Supported Script Types {#bridgehead_1492708796}

The customer payment record is scriptable in server SuiteScript only.

## Supported Functions {#bridgehead_1492708830}

The customer payment record is partially scriptable - it can be updated, deleted, and searched using SuiteScript. It cannot be created or copied.

## Usage Notes {#bridgehead_N3193789}

The following table provides usage notes for specific fields on this record.

| Field Internal ID | Field UI Label | Note |
| --- | --- | --- |
| **Body Fields** |
| ccnumber | Credit Card # | To prevent users from accessing sensitive information such as password and credit card data, this field cannot be read in beforeSubmit user event scripts for external role users (for example, shoppers, online form users (anonymous users), customer center). |
| isrecurringpayment | Recurring Payment | A value for this field is stored only if the value for paymentmethod is a credit card. |

The Deposits sublist is a **list** sublist.

### Related Topics

-   [Customer Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285644.html)
-   [Working with the SuiteScript Records Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3169369.html)
-   [SuiteCloud Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_3710625923.html)
-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3191224.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
