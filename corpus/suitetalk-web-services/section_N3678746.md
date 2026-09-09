---
id: "section_N3678746"
type: "section"
title: "Invoice"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Invoice"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3678746.html"
anchors: ["bridgehead_N3678784", "bridgehead_N3679054", "bridgehead_N3679091", "bridgehead_N3679100", "bridgehead_N3679160", "bridgehead_N3679253", "bridgehead_N3679270", "bridgehead_N3679283", "bridgehead_N3679296", "procedure_N3679310", "bridgehead_N3679322", "bridgehead_N3679343"]
sha256: "bddcc9a3b9045596ecf6044f3497e1e2fb3cb3a532cde06bd01e777488deb061"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Invoice](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161488248489.html).

An invoice transaction creates a bill for goods, services (or both) sold to a customer for which payment is not received at the time of delivery. The invoice indicates terms of payment that specify payment is to be received. Invoice aging tracks how long the amount has been due as payable. Each invoice consists of multiple line items whose sales amounts add up to the total of the invoice. Companies that bill costs back to customers can identify billable costs, mark them up and add them to invoices.

For more details about this type of transaction, see [Custom Workflow Based Invoice Approval](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1235332.html).

The invoice record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3678784}

The following operations can be used with the invoice record:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3679054}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [invoice](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/invoice.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3679091}

## Initializing Invoices {#bridgehead_N3679100}

You can initialize an invoice from a [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html), an [Estimate/Quote](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3673214.html), an [Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684743.html), or a [Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3690924.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For information about creating a single invoice from multiple sales orders, see [Creating Invoices or Cash Sales from Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1221414.html). For more information about the initialize operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

## Working with Invoice Sublists {#bridgehead_N3679160}

The SOAP Schema Browser includes all sublists associated with the Invoice record. See the following information for usage notes regarding specific Invoice sublists. Usage notes are not provided for every sublist type.

-   [InvoiceSalesTeamList](#bridgehead_N3679253)
    
-   [InvoiceItemCostList](#bridgehead_N3679270)
    
-   [InvoiceExpCostList](#bridgehead_N3679283)
    
-   [InvoiceTimeList](#bridgehead_N3679296)
    
-   [GiftCertRedemptionList](#procedure_N3679310)
    

## InvoiceSalesTeamList {#bridgehead_N3679253}

The InvoiceSalesTeam list defines the sales team for a specific invoice. This list is only available when the Team Selling feature is enabled in the account.

On add, a single line item is entered by default when a sales rep is currently associated with the entity set in the entity field. When a sales group is currently associated with the entity, the list is populated by the group.

## InvoiceItemCostList {#bridgehead_N3679270}

These fields map to the Billable Items subtab on the Item list of an invoice record. This is where you define how and when to bill item costs back to a customer. Billing items back to customers enables you to purchase items and supplies for an order or job, and then bill the cost to the customer. The Bill Costs To Customers feature must be enabled to use this list.

## InvoiceExpCostList {#bridgehead_N3679283}

These fields map to the Billable Expenses subtab on the Item list of an invoice record. This is where you define how and when to bill expenses back to a customer. The Bill Costs To Customers feature must be enabled to use this list.

## InvoiceTimeList {#bridgehead_N3679296}

These fields map to the Billable Time subtab on the Item list of an invoice record. This is where you define how and when to bill time back to a customer. The Bill Costs To Customers feature must be enabled to use this list.

## GiftCertRedemptionList {#procedure_N3679310}

This sublist is available on the invoice, sales order, and cash sale records.

## Associating Invoices with Opportunities {#bridgehead_N3679322}

You can associate estimates, cash sales, sales orders, and invoices with opportunities. After a transaction other than an estimate is associated with an opportunity, the opportunity's status is automatically set to **Closed Won**. After an opportunity's status is set to **Closed Won**, it is no longer available to be selected on other cash sale, sales order, or invoice records.

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3679343}

As of the 2011.2 endpoint, code to access serial number, lot number, and bin number data varies according to whether the Advanced Bin Management / Numbered Inventory Management feature is enabled.

-   If this feature is enabled, you must use the 2011.2 endpoint or later to access the [Inventory Detail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3744760.html) subrecord and the most up-to-date bin and numbered inventory fields. You need to update any SOAP web services code from a previous endpoint that accesses these fields, to avoid errors or unexpected results.
    
-   If this feature is not enabled, you do not need to use the inventory detail record to access bin and numbered inventory fields and you do not need to update any related SOAP web services code from prior to 2011.2.
    

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
