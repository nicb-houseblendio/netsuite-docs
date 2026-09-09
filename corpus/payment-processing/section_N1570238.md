---
id: "section_N1570238"
type: "section"
title: "Managing Payment Holds"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Managing Payment Holds"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html"
anchors: ["section_N1568265", "bridgehead_N1570279", "bridgehead_N1570299", "bridgehead_N1570389"]
sha256: "0725ffd39d4632b9de46f7f0a65fd23880402f58666ea1c8d0566b725bba30bb"
---

When a payment hold is placed on an order, your next step is to review the order and determine what action to take.

You can review orders placed on payment hold from:

-   Payment subtab of a sales order - review and take action on a single order
    
-   Manage Payment Holds page - review and take action on multiple orders
    
-   CyberSource Decision Manager- available if you subscribe to their fraud management service
    

## Reviewing Payment Status and Sales Orders {#section_N1568265}

Sales orders flagged with a payment hold are saved and available for review and further action. Evaluate the reason and details returned for the payment request and determine how to proceed. You can resubmit the sales order for credit card authorization with corrected credit card information or with a lower order amount, for example. You can also resubmit the order because the verification service is now available, or because you make some other change in the order.

To resubmit an order, enter changes, if any, on the sales order, check the Get Authorization box on the Payment subtab, and save the order.

Use the Manage Payment Holds page to process changes for multiple orders. Go to _Customers > Sales > Manage Payment Holds_. This page displays all orders with a payment status of Hold, filtered by Hold Reason.

![Manage Payment Holds page with the Hold Reason list expanded.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/managepayholds.png)

For the orders you select, you can:

-   Clear the payment hold
    
-   Resubmit for payment authorization
    
-   Cancel the order
    

Use the page filters to limit the list of orders by customer or hold reason. The Manage Payment Holds page displays orders only for one type of hold reason. You can't view a list of all payment holds. To open a specific sales order, click the link in the date column.

## Override Payment Holds Permission {#bridgehead_N1570279}

Only users with a role that includes the Override Payment Holds permission can access the Manage Payment Holds page and the Override Payment Hold button on a sales order. Standard roles with this permission include A/R Clerk, Accountant (Reviewer), CFO, Sales Manager, Sales Vice President, Store Manager, and System Administrator. You can also add the Override Payment Holds permission to a custom roles. See [Changing Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N289485.html).

## Manage Payment Holds {#bridgehead_N1570299}

Use the Manage Payment Holds page to review and take action on multiple orders. For example, you can check all orders for one customer and resubmit them for authorization at the same time.

1.  Go to _Customers > Sales > Manage Payment Holds_.
    
2.  Filter the list of orders displayed to find specific orders or limit the orders displayed. You can filter by customer or hold reason.
    
3.  Select the order or orders you want to process.
    
4.  You can select:
    
    -   **Cancel Order** - cancels the sales order
        
    -   **Override Payment Hold** - removes payment hold from sales order, checks the Credit Card Approved box and saves the order. The order can now be fulfilled.
        
    -   **Get Authorization** - removes the payment hold and resubmits the order for payment authorization. This button isn't enabled when the hold reason is Verification Required.
        

## Working with CyberSource Decision Manager in NetSuite {#bridgehead_N1570389}

To use Decision Manager you must subscribe to the service in your CyberSource account and identify the type of orders it applies to when setting up the credit card processing profile in NetSuite. You can also map NetSuite sales order fields to data fields defined in Decision Manager for advanced fraud rules, reporting, and reconciliation. Decision Manager and Merchant Defined Data Mapping are only available for CyberSource gateways.

CyberSource provides the information about how to configure and use Decision Manager to manage credit card processing decisions.

Important:

CyberSource doesn't push any order changes you make in Decision Manager back to NetSuite. You must manually update transactions in NetSuite to record actions taken in Decision Manager.

Note:

If you override a payment hold in NetSuite, you must also update that information in Decision Manager.

### Related Topics

-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Transitioning to a New Gateway and Disabling the Old Gateway](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1566955.html#section_N1577424)
-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)
-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   _Credit Card Processing Gateway FAQ_
    
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)
-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Order Verification Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567770.html)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Setting Up Customer Credit Card Soft Descriptors](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1568841.html)
-   [Using CyberSource Decision Manager for Fraud Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1492534842.html)
-   [Viewing Customer Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1571967.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
