---
id: "section_N1325604"
type: "section"
title: "Contract Creation Process"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Contract Creation Process"
parent: "chapter_N1319596"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html"
anchors: []
sha256: "819420236be2f64145ff1588a2cd4437d7e9b393ee671ac11bf29df69d6dd217"
---

With the Software Vertical Contract Renewals SuiteApp, contracts are generated from sales orders. When you enter a sales order using the Sales Order - Contract Renewal form, you define the term of the contract by setting the contract term and start date. For information about contract term, see [Contract Term Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4582083020.html).

![Example Sales Order record, with Contract Term and Start Date fields highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/SalesOrdersCashSales/ContractBilling_SO_ContractTermFields.png)

By default, line items added to the order are given the same start and end dates as the body of the transaction. You can modify the term length and the dates for individual line items.

The value that you selected in the **Sales Order Status to Create Contract** preference determines when a new contract is generated for a sales order. If you selected **Sales Order: Pending Approval**, a contract is generated and associated with the order after the sales order is saved (even if the sales order isn't yet approved). If you selected **Sales Order: Pending Fulfillment**, a contract is generated when the sales order is approved. For information about this preference, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

You can also create a contract for a specific sales order by clicking the **Create Contract** button on the transaction record. This button is available on sales orders with an empty **Contract** field (that is, a contract isn't yet created for the order).

When a contract is generated for the order, a link to the contract record is shown in the **Contract** field on the **Items** subtab of the sales order.

![Example Items subtab with Contract field highlighted.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/SalesOrdersCashSales/ContractBilling_SO_ContractShown.png)

When the order is fully billed (which is the default preference setup), contract items are added to the contract based on the line items on the sales order. By default, these contract items are set to be generated on an hourly basis, but you can change the frequency of this process by setting the schedule on the deployment record. For information about setting the timing of the contract item script (R03), see [Setting Up Schedules for Contract Item Creation and Contract Renewal](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4569844795.html). For information about billing sales orders, see [Invoicing Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1219162.html).

On the contract record, the value of the contract is shown in these fields:

-   **Contract Value (Base Curr)** - For NetSuite OneWorld accounts, this field displays the value of the contract in the base currency of the customer's subsidiary. Otherwise, this field displays the value of the contract in the currency of your company.
    
-   **Contract Value (Customer Primary Curr)** - This field displays the value of the contract in the primary currency of the customer.
    

For information about contract values, see [Contract Value Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4473187166.html).

By default, 90 days prior to the end date of the contract, a renewal transaction is automatically generated for the contract. You can change when contract renewals are processed by setting the **Days Before Renewal** preference on the Contract Renewals Preferences page. For more information, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

You can also override the **Days Before Renewal** global preference for specific contracts by specifying a value in the Contract Days Before Renewal field on the contract record. For more information, see [Editing a Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448152522.html).

Any items that are set up as renewable are automatically included on the renewal contract. For more information, see [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html).

### Related Topics

-   [Software Vertical Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1319596.html)
-   [Contract Renewals Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4442063121.html)
-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html)
-   [Setting Up Items for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325048.html)
-   [Creating a New Contract](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325805.html)
-   [Importing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1328129.html)
-   [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)
-   [Scripting Contract and Contract Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1329149.html)
-   [Adding Transaction Fields to a Web Service Request for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4539453728.html)
-   [Software Vertical Contract Renewals References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4581932984.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
