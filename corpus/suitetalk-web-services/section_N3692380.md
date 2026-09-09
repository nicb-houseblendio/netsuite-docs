---
id: "section_N3692380"
type: "section"
title: "Transfer Order"
branch: "suitetalk-web-services"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteTalk Web Services > SuiteTalk SOAP Web Services Records Guide > Transactions > Transfer Order"
parent: "chapter_N3657735"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3692380.html"
anchors: ["bridgehead_N3692433", "bridgehead_N3692702", "bridgehead_N3692739", "bridgehead_N3692747", "bridgehead_N3692831", "bridgehead_N3692968", "bridgehead_N3694316"]
sha256: "67eec941fa6161a88ab139b562c543e4279d7f58c047f05c90da7690c17f5dfc"
---

Important:

Most types of records are also supported in REST web services. For a list of all records supported in REST, see [REST Web Services Supported Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1558962745.html).

Important:

For information about working with this record type in REST web services, see [Transfer Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_0817021034.html).

The Transfer Order transaction is used to move inventory between locations when the Multi-Location Inventory (MLI) feature is enabled. Existing integrations with external warehouse management systems can leverage this transaction to manage data about inventory movement between locations.

Transfer orders can initialize item fulfillment and item receipt transactions. See [Item Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3680777.html) and [Item Receipt](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3681685.html) for details about these transactions.

The transfer order record is defined in the [tranInvt (inventory)](https://webservices.netsuite.com/xsd/transactions/v2025_2_0/inventory.xsd) XSD.

## Supported Operations {#bridgehead_N3692433}

The following operations can be used to modify transfer order records:

[add](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480855.html) | [addList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481360.html) | [attach / detach](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3481947.html) | [delete](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486046.html) | [deleteList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3486552.html) | [get](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3488543.html) | [getDeleted](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3497592.html) | [getList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3499748.html) | [getSavedSearch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3503649.html) | [getSelectValue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3504236.html) | [initialize / initializeList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3508536.html) | [search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3514306.html) | [update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527090.html) | [updateList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3527652.html) | [upsert](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3532463.html) | [upsertList](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3533243.html)

Note:

You can also use the asynchronous equivalents of SOAP web services list operations. For information about asynchronous operations, see [SOAP Web Services Asynchronous Operations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3480635.html). For more information about request processing, see [Synchronous Versus Asynchronous Request Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3444207.html).

## Field Definitions {#bridgehead_N3692702}

The SOAP Schema Browser includes definitions for all body fields, sublist fields, search filters, and search joins available to this record. For details, see the SOAP Schema Browser's [transfer order](https://system.netsuite.com/help/helpcenter/en_US/srbrowser/Browser2026_1/schema/record/transferorder.html) reference page.

Note:

For information about using the SOAP Schema Browser, see [SOAP Schema Browser](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3639052.html).

## Usage Notes {#bridgehead_N3692739}

## Transfer Order Features and Preferences {#bridgehead_N3692747}

The Transfer Order transaction is available when the Multi-Location Inventory feature is enabled. Note that the Pick, Pack and Ship feature can affect transfer order workflow.

The following accounting preferences, available at _Setup > Accounting >Accounting Preferences_, on the Order Management subtab, apply to transfer orders:

-   Default Transfer Order Status indicates whether transfer orders require approval by default.
    
    -   Pending Approval means that by default the status of someone with permission must approve the order before it is processed.
        
    -   Pending Fulfillment means that by default transfer orders are sent directly to the fulfillment queue without requiring further approval.
        
-   Use Item Cost as Transfer Cost affects how the Transfer Price from each transfer order is used on the related item receipt transaction.
    
    -   When this option is enabled, the transfer price is used as a declared shipping value for reference only, such as for insurance or international shipping, and the item cost from the item record is used on the item receipt. Also, when this option is enabled and different items are fulfilled in different item fulfillments, you must receive the items separately. In this case, a separate item receipt is created for each item fulfillment.
        
    -   When this option is disabled, the transfer price on the transfer order is used as the item cost on the item receipt. In this case, both the item fulfillment and the item receipt resulting from the transfer order have G/L impact. Also, when this option is disabled and different items are fulfilled in different item fulfillments, you can receive all items in the same item receipt.
        

## Transfer Order Workflow {#bridgehead_N3692831}

The following is a rough outline of transfer order workflow. For more details, see [Inventory Transfer Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2308766.html).

1.  A transfer order is entered to schedule the movement of items and its status is set to either Pending Approval or Pending Fulfillment.
    
    A transfer order can be approved by setting the status to Pending Fulfillment.
    
    Note:
    
    A transfer order initially can be saved without a source location value, for example, in a case where an item is needed at the destination location but the source location has not yet been identified. However, the source location value is required for an approved transfer order.
    
2.  After its status is set to Pending fulfillment, the transfer order can be fulfilled from the source location.
    
    -   An item fulfillment transaction is created.
        
    -   Items are committed out of the source location's inventory.
        
    -   The On Order quantity of items increases at the destination location.
        
    -   Fulfilled items are removed from the On Hand count at the source location.
        
    -   The value of items in transit are removed from the Inventory Asset account and added to the Inventory in Transit account for the source location.
        
    -   The status of the transfer order is set to Pending Receipt, or if the Pick, Pack and Ship feature is enabled, to Shipped.
        
3.  After the transfer order status has been set to Pending Receipt (or to Shipped),Transfer order items can be received at the destination location.
    
    -   An item receipt transaction is created.
        
    -   The items are added to the destination location's inventory and increase the On Hand count.
        
    -   The items' value is added to the Inventory Asset account for the destination location.
        
    -   The On Order quantity of the item in the destination location decreases.
        

## Serialized and Lot Inventory Transfer Orders {#bridgehead_N3692968}

Serial or lot numbered items can be included as transfer order line items. Note the following requirements:

-   Serial or lot numbers are limited to 3800 characters.
    
-   Supported separators for serial numbers are: space, comma, or line break.
    
-   A serial number is required for every serialized line item.
    
    For example, if the quantity of a line item is 2, two serial numbers are required.
    
-   Lot numbers must use the following format: <Lot #>(<Quantity>)
    
    For example, to indicate a quantity of 100 for an item with lot number AAA-3400, format would be: AAA-3400(100)
    

## Accessing Serial/Lot or Bin Data for Line Items {#bridgehead_N3694316}

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
