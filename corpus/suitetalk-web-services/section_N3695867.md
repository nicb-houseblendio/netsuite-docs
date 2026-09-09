---
id: "section_N3695867"
type: "section"
title: "Vendor Payment"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Vendor Payment"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3695867.html"
anchors: ["bridgehead_N3695904", "bridgehead_N3696157", "bridgehead_N3696194", "bridgehead_N3696203", "bridgehead_N3696252"]
sha256: "353c92c02368d4153f760a5871bfa2e639b8aedc4b4d45e4a2fac3ebb4265880"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Vendor Payment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_7095737506.html).

A vendor payment transaction posts to the general ledger as an expense and the amount of the payment is deducted from your accounts payable total. A vendor payment can be applied to one or more vendor bills. Vendor payments can help to track expenditures and total payables due.

For details about this type of transaction, see [Vendor Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2381615.html).

The vendor payment record is defined in the [tranPurch (purchases)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/purchases.xsd) XSD.

## Supported Operations {#bridgehead_N3695904}

The following operations can be used with vendor payment records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3696157}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [vendor payment](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/vendorpayment.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3696194}

## Initializing Vendor Payments {#bridgehead_N3696203}

You can initialize a vendor payment from an [Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3643925.html), a [Vendor](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3646902.html), or a [Vendor Bill](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3694535.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Applying Vendor Payments to Bills {#bridgehead_N3696252}

As of the 2011.1 endpoint and later, you can use {doc, line} on the VendorPaymentApply sublist to identify the vendor bill line to which a payment should be applied. You can use the line element to uniquely identify a sublist entry when the **doc** element is not sufficient. The line element prevents problems with record creation due to duplicate keys.

Use the initialize operation to obtain the doc and line values from the vendor bill.

Warning:

As of the 2011.1 endpoint and later, if you do not provide a value for the line element for an entry to VendorPaymentApply, you may receive the error: 'Ambiguous sublist reference; multiple matches exist for key value <doc>'. Earlier endpoints do not return this error.

### Related Topics

-   [Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3657735.html)
-   [Usage Notes for Transaction Record Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3658677.html)
-   [Transaction Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3659492.html)
-   [Multiple Shipping Routes in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3702654.html)
-   [How to Use the SOAP Web Services Records Help](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635039.html)
-   [SOAP Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3635369.html)
-   [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html)
-   [SuiteTalk SOAP Web Services Platform Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3412777.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
