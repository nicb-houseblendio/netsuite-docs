---
id: "section_N3664209"
type: "section"
title: "Check"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Check"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3664209.html"
anchors: ["bridgehead_N3666021", "bridgehead_N3666273", "bridgehead_N3666310", "bridgehead_N3666318"]
sha256: "0a1d000497fc21d72545359fea16535445c5755d483ad3678e91291ff6e3726d"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Check](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_081706221410.html).

A check transaction creates and records a check used to pay an expense, records an expense paid in cash and not entered as a bill, or records a non-check debit transaction, such as a debit card transaction, ATM (automated teller machine) transaction, or EFT (electronic funds transfer) payment. A check transaction records an expense directly to your books by debiting the expense account specified in the transaction detail and crediting the bank account the check selected for the check.

For more details about this type of transaction, see [Checking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1543613.html).

The check record is defined in the [tranBank (bank)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/bank.xsd) XSD.

## Supported Operations {#bridgehead_N3666021}

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3666273}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's the [check](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/check.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3666310}

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3666318}

As of the 2011.2 endpoint, code to access serial number, lot number, and bin number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the Inventory Detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

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
