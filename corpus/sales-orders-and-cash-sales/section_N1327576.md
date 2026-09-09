---
id: "section_N1327576"
type: "section"
title: "Example - Renewal Impact of Upsell and Returns"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Managing Contracts > Contracts and Returns > Example - Renewal Impact of Upsell and Returns"
parent: "section_N1326489"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1327576.html"
anchors: []
sha256: "61d84ea26752f7720eaad4dbb5d2654265d7d9af7670133bd0a76529514992d8"
---

Contract renewal automatically reflects upsell and returns that occur during the original term of the contract. Upsell items that extend to the end of the contract term are renewed, and items that are returned aren't renewed.

For example, a software company creates an order for a new contract that includes these items:

-   A twelve-month term product license
    
-   Three-months of on-site professional services training
    
-   100 seats
    
-   A support entitlement
    

All of these items are renewable except for the training, which ends after three months. The training isn't generated as a contract item.

When the order is approved and fulfilled, a contract is generated that includes all of the order line items (except for the training) as contract items.

Six months into the contract, the company purchases an add-on module. A new order is created and tied to the existing contract. When the existing contract is selected in the Contract field, the term, start and end dates are automatically updated on the transaction.

The new order includes the module as well as a support entitlement for the module.

![Items subtab showing details of new contract sales order (tied to the existing contract).](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/SalesOrdersCashSales/ContractBilling_ComplexExample_UpsellOrder.png)

After the order is approved and billed, the contract is updated with the new contract items.

Nine months into the contract, there is an economic downturn, and the company decides to reduce the number of seats from 100 to 75. A return authorization is entered.

![Items subtab on the return authorization showing 1 line item with the Qty highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/SalesOrdersCashSales/ContractBilling_ComplexExample_ReturnItemst.png)

The return shows as a negative line on the contract.

When the contract renews, only the renewable items from the original contract and the add-on module that was added mid-term are renewed. The 25 seats that were removed through the RMA aren't renewed. Also, the support entitlement from the upsell order is combined with the support item that was included in the original contract.

### Related Topics

-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html)
-   [Contract Upsell](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326206.html)
-   [Contracts and Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326489.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
