---
id: "section_N3675550"
type: "section"
title: "Intercompany Transfer Order"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions-related Records > Intercompany Transfer Order"
parent: "article_160526452785"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3675550.html"
anchors: ["bridgehead_N3675586", "bridgehead_N3675855", "bridgehead_N3675892", "bridgehead_N3675913", "bridgehead_N3675961"]
sha256: "87e94606a146149358d541d611882f8fe8f7d04b29b5ccb7b07a0da84b23a9eb"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Intercompany Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0822103427.html).

In accounts using NetSuite OneWorld, the Intercompany Transfer Order transaction is used to move inventory from a location for one subsidiary to a location for another subsidiary. The intercompany transfer order record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

For information about how intercompany transfer orders are used, see [Intercompany Inventory Transfers - Non-Arm's Length](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2313577.html).

## Supported Operations {#bridgehead_N3675586}

The following operations can be used to modify intercompany transfer order records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3675855}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [intercompany transfer order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/intercompanytransferorder.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3675892}

You should read the usage notes for [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html), because these notes also apply to the Intercompany Transfer Order. The following additional notes apply.

## Source Subsidiary and Destination Subsidiary {#bridgehead_N3675913}

An intercompany transfer order must have a Subsidiary (meaning the source subsidiary) and a Destination Subsidiary value.

All transfer order line items must be available to both the source and destination subsidiaries.

The Source Location for a transfer order must be from the (source) Subsidiary and the Destination Location must be from the Destination Subsidiary.

The Department and Class values for a transfer order must be from the (source) Subsidiary. These values are used for shipment transactions.

You must have permissions for both the source (Subsidiary) and Destination Subsidiary to create or edit an intercompany transfer order. Permissions for both the Source Location and Destination location also are required, whether the transfer order status is set to Pending Approval or Pending Fulfillment.

## Transfer Pricing Notes and the Use Item Cost as Transfer Cost Preference {#bridgehead_N3675961}

Intercompany transfer orders can be entered when the Use Item Cost as Transfer Cost preference is enabled on the Order Management subtab at _Setup > Accounting > Accounting Preferences_.

The transfer order Transfer Price value defaults to the Transfer Price listed on the item record, but can be changed when the transfer order is created or edited.

-   The item record Transfer Price is in the currency of the root parent subsidiary. On the transfer order, the Transfer Price should be converted to the correct value in the currency of the source subsidiary.
    
-   If the item record Transfer Price is not set, the Transfer Price on the transfer order is 0. In this case, be sure to edit the transfer order Transfer Price as necessary.
    

The difference between the item cost and the transfer order Transfer Price is recorded in a Gain/Loss account, and G/L impact occurs after item receipt, as shown in the following table:

| Account | Debit | Credit | Subsidiary |
| --- | --- | --- | --- |
| Inventory Asset | X | \- | Destination Subsidiary |
| Inventory in Transit | \- | X | Source Subsidiary |
| Intercompany Payable/Receivable Intercompany Clearing | \- | X | Destination Subsidiary (Payable) |
| Intercompany Payable/Receivable Intercompany Clearing | X | \- | Source Subsidiary (Receivable) |

Important:

When NetSuite released the Intercompany Time and Expenses feature, the first set of accounts created were named Intercompany Payable/Receivable XXX, where XXX denoted the currency ISO code. In 2013.1 NetSuite OneWorld introduced the Intercompany Clearing XXX account. This new account replaced the Intercompany Payable/Receivable Account for new accounts because the existing accounts were being used by the Intercompany Elimination feature. The change applied to only new accounts. Existing accounts were not renamed. In 2014.1, NetSuite OneWorld introduced new intercompany clearing accounts for payable and receivable that are not currency locked. These new clearing accounts are used for intercompany transactions. All existing currency-locked intercompany clearing accounts (the Intercompany Payable/Receivable accounts) are now child accounts of the new clearing account. For more information, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html) and [Intercompany Elimination Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1498385.html).

Be aware that the exchange rate between subsidiaries' currencies can affect the G/L impact to each subsidiary.

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
