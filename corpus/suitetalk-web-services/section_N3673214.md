---
id: "section_N3673214"
type: "section"
title: "Estimate/Quote"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Estimate/Quote"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3673214.html"
anchors: ["bridgehead_N3673258", "bridgehead_N3673528", "bridgehead_N3673565", "bridgehead_N3673574", "bridgehead_N3673606", "bridgehead_N3673659", "bridgehead_N3673671", "bridgehead_N3674370"]
sha256: "b469c35bff9635ab6ef90009c36f5f3d4ef1e25b6363d565c81f149154dd7455"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Estimate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0719105836.html).

An estimate transaction, sometimes referred to as a quote, is a non-posted record of estimated charges to a customer. An estimate can be printed, emailed, or faxed to the customer. After the customer accepts the estimate, it can be converted into a sales order, invoice, or cash sale. This transaction is available when the Estimates feature is enabled at _Setup > Company > Enable Features_, on the Transactions subtab.

Note:

Estimates have no accounting impact until they are converted into invoices or cash sales.

For more details about this type of transaction, see [Estimates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1069662.html).

The estimate/quote record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3673258}

The following operations can be used with estimate records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3673528}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [estimate](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/estimate.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

Note:

The balance field is only returned when using advanced search. It is not returned when using the <Record>SearchBasic search object. In advanced search, you must set the bodyFieldsOnly preference to false. The balance field is not returned if the bodyFieldsOnly preference is set to true. For more information, see [bodyFieldsOnly](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4170181850.html#bridgehead_N3423730).

## Usage Notes {#bridgehead_N3673565}

## Initializing Estimates {#bridgehead_N3673574}

You can initialize an estimate from an [Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684743.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Accessing Serial/Lot Number Data for Line Items {#bridgehead_N3673606}

As of the 2011.2 endpoint, code to access serial number or lot number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the Inventory Detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

For more details, see [Updating SOAP Web Services Code When Advanced Bin / Numbered Inventory Management is Enabled](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3745415.html).

## Setting Handling Cost {#bridgehead_N3673659}

If you want to set a value for handlingCost, be aware of the following guidelines.

## Only Certain Shipping Methods Allow Handling Cost To Be Set {#bridgehead_N3673671}

In both the UI and in SOAP web services, the default behavior of the system is that you cannot specify a handling cost on a new estimate. To be able to enter a value for handling cost, you must choose a shipping method that enables the handling cost field.

You can identify an appropriate shipping method by reviewing the details for the corresponding shipping item. Choose _Lists > Accounting > Shipping Items_, then select the shipping item you want to review (each shipping item corresponds with a shipping method). In the item record, review the details on the Handling Rate subtab. If the Handling - No Handling Charge is **not** selected, then choosing this shipping item lets you set a handlingCost value.

During an add operation, you must set the shipMethod value in the same SOAP request where you set the handlingCost value. If you fail to set any value for shipMethod, or if you choose a value that does not enable the handling cost field, the system generates an error reading in part 'You do not have permissions to set a value for element handlingcost.'

## You Must Specify a Shipping Cost {#bridgehead_N3674370}

If you are doing an add operation, be aware that in some cases the system may overwrite the handlingCost value specified in your SOAP request. To avoid this, make sure that your SOAP request include a shippingCost value. If you fail to include a shippingCost, the system overwrites your handlingCost value with an automatically generated value.

This behavior is specific to the add operation. During an update, it is possible to set a value for handlingCost without specifying the shippingCost.

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
