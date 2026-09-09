---
id: "section_N1325805"
type: "section"
title: "Creating a New Contract"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Contract Creation Process > Creating a New Contract"
parent: "section_N1325604"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325805.html"
anchors: ["procedure_N1325836"]
sha256: "a2969b2383e8aeeab898e5b410d6b7584962113845b13d5b93a3310293f44f5e"
---

With Software Vertical Contract Renewals SuiteApp, contracts and their contract items are generated from sales transactions: opportunities, estimates, and sales orders. Opportunities and estimates must be converted to a sales order before a contract record can be generated. Contracts are created from sales orders using the Sales Order - Contract Renewals form or any customized version of this form.

You can choose when a contract record will be generated from a sales order in the **Sales Order Status to Create Contract** field on the Contract Renewals Preferences page. For more information, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

Note:

Contracts and contract items can't be created manually, but you can import contracts using CSV import. For more information, see [Importing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1328129.html).

#### To create new contract from a sales order: {#procedure_N1325836}

1.  Go to Transactions > Sales > Enter Sales Order.
    
2.  In the **Custom Form** field, select **Sales Order - Contract Renewals**.
    
3.  In the **End User** field, select a customer. If necessary, on the **Channel** subtab, define who this end user is relative to the customer in the **Bill To Customer** field.
    
4.  In the **Contract Term** field, enter the number of months this contract runs. You can enter decimal numbers if you need to represent a term in days.
    
5.  In the **Start Date** field, enter the start date for this contract. The end date is calculated automatically based on the contract term and start date values. For information about contract term, see [Contract Term Calculation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4582083020.html).
    
    Note:
    
    By default, transactions created from an opportunity don't have a start date. You must manually enter the start date for these transaction records.
    
6.  Enter values in the other fields on the transaction header as you would in a standard sales order. For more information, see [Creating Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1216500.html).
    
7.  On the **Items** subtab:
    
    1.  If this is an order for a new contract, leave the **Contract** field blank.
        
        If this is an upsell order for an existing contract, select a contract in the **Contract** field. For more information, see [Contract Upsell](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326206.html).
        
    2.  In the **Item** column, select items that you want to include in the contract. If you're creating a sales order from an estimate or opportunity, the items are populated from that transaction.
        
        If you want to apply a percentage uplift for a renewable item, enter the value in the Contract Item Uplift column. For more information, see [Contract Item Uplift](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4852275502.html).
        
        Note:
        
        You may need to edit these items to ensure that the dates are set properly. The start and end dates for each item are populated from the transaction body. You can change these dates for items that don't apply to the full contract term.
        
        Note:
        
        If the sales order status is Pending Fulfillment, you won't be able to edit the line item dates after adding the item. Also, after adding the first line item, the start date column will be grayed out for succeeding line items. If you want to be able to modify the dates for each line item, change the status of the sales order to Pending Approval.
        
        Important:
        
        Items that don't co-terminate with the end of the contract aren't renewed even if they are set up to be renewable.
        
8.  If you want to set a custom price for any of the item, click the **Options & Log** subtab and set these fields:
    
    -   **Block Custom Price Level** - Default value is **Yes**. Set this field to **No** if you want to enable setting a custom price level for items in this transaction. This setting overrides the settings you made in the **Item Category = For Custom Price Block** preference on the Contract Renewals Preferences page, which blocks custom pricing for specific item categories. This setting applies only to non-maintenance/support items.
        
    -   **Allow Custom Price Level for M/S Items** - Default value is **No**. Set this field to **Yes** if you want to enable setting a custom price level for maintenance and support items in this transaction. This setting overrides the settings you made in the **Item Category = For Custom Price Block** preference on the Contract Renewals Preferences page, which blocks custom pricing for specific item categories.
        
    -   **Custom Price Entered is Annual Rate** - Check this box if you want to enter custom price level list rates as annual rates. This setting enables you to enter annual rates in the List Rate column for items with custom price level, to ensure proper calculation of the amount. In the end, the list rate will be divided by 12 months and stored as a monthly rate.
        
9.  Click **Save**.
    

The value in the **Sales Order Status to Create Contract** preference determines when a new contract is generated for a sales order based on its status.

-   If you selected **Sales Order: Pending Approval**, a contract is generated upon saving of the sales order (even if the order isn't yet approved).
    
-   If you selected **Sales Order: Pending Fulfillment**, a contract is generated upon approval of the sales order. In this case, a contract won't be automatically generated for sales orders with a status of Pending Approval. However, you've the option to create contracts on demand for sales orders with no contract yet by clicking the **Create Contract** button on the transaction record.
    

When a contract is saved or approved (depending on the preference set), a user event script saves the transaction record and creates a contract in the background. After the contract is created, the user event script triggers a workflow action that attaches the contract record to the sales order.

To improve performance, the contract creation user event script doesn't wait for the workflow action to finish attaching the contract to the sales order. For this reason, there may be instances when the **Contract** field on the **Items** subtab displays an incomplete contract ID and the **Check Log Status** field on the **Options & Log** subtab is empty after a sales order is saved.

To check if the workflow action has successfully attached the contract to the sales order, refresh the Sales Order page and check if the **Contract** field is displaying the complete contract ID and the value in the **Check Log Status** field on the **Options & Log** subtab is **Pending**.

Contracts are given an ID in the following format: **ID\_<Start Date>\_<End Date>**. Click the link in the **Contract** field on the sales order to go to the contract record.

You can also create Contract Items on demand, refer to [Creating Contract Items On Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1490160021.html).

### Related Topics

-   [Software Vertical Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1319596.html)
-   [Contract Renewals Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4442063121.html)
-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html)
-   [Setting Up Items for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325048.html)
-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Importing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1328129.html)
-   [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)
-   [Scripting Contract and Contract Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1329149.html)
-   [Adding Transaction Fields to a Web Service Request for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4539453728.html)
-   [Software Vertical Contract Renewals References](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4581932984.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
