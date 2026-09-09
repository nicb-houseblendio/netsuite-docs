---
id: "section_N3663345"
type: "section"
title: "Cash Sale"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Cash Sale"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3663345.html"
anchors: ["bridgehead_N3663390", "bridgehead_N3663660", "bridgehead_N3663697", "bridgehead_3946331793", "bridgehead_N3663705", "bridgehead_N3663765", "bridgehead_N3663874", "bridgehead_N3663891", "bridgehead_N3663904", "bridgehead_N3663918", "bridgehead_N3663931", "procedure_N3663944", "bridgehead_N3663956", "bridgehead_N3663968", "bridgehead_N3663990"]
sha256: "219b2c38a692e351d434c147ddfa762efb448413f73c8f1368ca3e07fdb69a1e"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Cash Sale](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161487969808.html).

A cash sale transaction records the sale of goods or services for which immediate payment is received at the time of delivery. Cash sale line items specify the goods and services sold and their sales amounts. The sum of all sales amounts plus any applicable tax equals the total amount paid for the transaction.

For more details about this transaction, see [Cash Sales](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1244343.html).

The cash sale record is defined in the [tranSales (sales)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/sales.xsd) XSD.

## Supported Operations {#bridgehead_N3663390}

The following operations can be used with cash sale records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3663660}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [cash sale](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/cashsale.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3663697}

## Working with Credit Card Data {#bridgehead_3946331793}

When working with credit card data, be aware of the following security features:

-   When adding a transaction that uses a credit card number, you cannot identify the credit card number using a masked value such as \*\*\*\*\*\*\*\*\*\*\*\*5151. You must enter the full 16-digit number, or you can identify an existing credit card record through a RecordRef. (You can identify the full number using the **ccNumber** field. You can reference an existing record using the **creditCard** field.)
    
-   Searches do not work if they include the operator **is** or **isNot** in conjunction with the ccNumber field. The only search operators that can apply to this field are **empty** and **notEmpty**.
    

## Initializing Cash Sales {#bridgehead_N3663705}

You can initialize a cash sale from a [Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639940.html), [Estimate/Quote](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3673214.html), [Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3684743.html), or [Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3690924.html).

The SOAP web services initialize operation emulates the UI workflow by prepopulating fields on transaction line items with values from a related record. For more information about this operation, see [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html).

Note:

To initialize a cash sale from a sales order that is in the Pending fulfillment status, you must enable the Invoice in Advance of Fulfillment preference. You can enable this preference at _Setup > Accounting > Preferences > Accounting Preferences (Administrator)_, on the Order Management subtab. For more information, see [Caching Behavior in SOAP Web Services](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1512050046.html).

## Working with Cash Sale Sublists {#bridgehead_N3663765}

The SOAP Schema Browser includes all sublists associated with the cash sale record. See the following information for usage notes regarding specific cash sale sublists. Usage notes are not provided for every sublist type.

-   [CashSaleSalesTeamList](#bridgehead_N3663874)
    
-   [CashSaleItemList](#bridgehead_N3663891)
    
-   [Cash SaleItemCostList](#bridgehead_N3663904)
    
-   [CashSaleExpCostList](#bridgehead_N3663918)
    
-   [CashSaleTimeList](#bridgehead_N3663931)
    
-   [GiftCertRedemptionList](#procedure_N3663944)
    

## CashSaleSalesTeamList {#bridgehead_N3663874}

The CashSaleSalesTeam list defines the sales team for a specific cash sale. This list is only available when the Team Selling feature is enabled in the account.

On add, a single line item is entered by default when a sales rep is currently associated with the entity set in the entity field. When a sales group is currently associated with the entity, the list is populated by the group.

## CashSaleItemList {#bridgehead_N3663891}

The orderLine field in this sublist establishes the relationship with an existing sales order, if any. You must set a value for orderLine to populate the createdFromfield.

## Cash SaleItemCostList {#bridgehead_N3663904}

These fields map to the Billable Items subtab on the Item list of a cash sale record. This is where you define how and when to bill item costs back to a customer. Billing items back to customers enables you to purchase items and supplies for an order or job, and then bill the cost to the customer. The Bill Costs To Customers feature must be enabled to use this list.

## CashSaleExpCostList {#bridgehead_N3663918}

These fields map to the Billable Expenses subtab on the Item list of a cash sale record. This is where you define how and when to bill expenses back to a customer. The Bill Costs To Customers feature must be enabled to use this list.

## CashSaleTimeList {#bridgehead_N3663931}

These fields map to the Billable Time subtab on the Item list of a cash sale record. This is where you define how and when to bill time back to a customer. The Bill Costs To Customers feature must be enabled to use this list.

## GiftCertRedemptionList {#procedure_N3663944}

This sublist is available on the invoice, sales order, and cash sale records.

## Promotion Code Validation {#bridgehead_N3663956}

Note that validation of promotion code date range for a cash sale transaction generated from a sales order is different in SOAP web services than in the user interface. In the user interface, if the sales order date was within the promotion code date range, cash sale can be generated without error, even if cash sale date is outside of promotion code date range. In SOAP web services, cash sale date must be within promotion code date range.

## Associating Cash Sales with Opportunities {#bridgehead_N3663968}

You can associate estimates, cash sales, sales orders, and invoices with opportunities. After a transaction other than an estimate is associated with an opportunity, the opportunity's status is automatically set to **Closed Won**. After an opportunity's status is set to **Closed Won**, it is no longer available to be selected on other cash sale, sales order, or invoice records.

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3663990}

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
