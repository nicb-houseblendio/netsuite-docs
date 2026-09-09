---
id: "section_N1567770"
type: "section"
title: "Order Verification Rules"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Order Verification Rules"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567770.html"
anchors: ["bridgehead_N1567973", "procedure_N1567997"]
sha256: "c6e42d9da1408877f4fab955a232bff19c39875b9e97ce4bf9676981e0993d14"
---

With CyberSource and MerchantE gateways, you can set up rules to determine how to handle the different types of authorization responses returned by your credit card gateway for Address Verification System (AVS) and Credit Card Verification (CSC) authorization requests.

![The Order Verification Settings subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/avsrules.png) ![The Credit Card Verification (CSC) Rules subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/cscrules.png)

Based on the rule criteria, orders can be placed in a queue to be reviewed and either approved for fulfillment or canceled.

The gateway returns one AVS response and one CSC response for an authorization request. The response with the most restrictive action determines the payment status for the order.

-   **Accept** - payment authorization is valid and order status is set to Pending Fulfillment or Pending Approval.
    
-   **Cancel Order** - payment authorization is rejected, order is canceled and not fulfilled.
    
-   **Verification Review** - payment status for order is set to On Hold and order must be reviewed to determine if it should be resubmitted for authorization, canceled, or saved for fulfillment. For information about payment holds, see [Managing Payment Holds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html).
    

For example, you set up the following AVS and CSC order verification rules:

| Condition | Action |
| --- | --- |
| Partial AVS Match | Verification Review |
| No CSC Match | Cancel Order |

Then you save a sales order, which submits a request for payment authorization for a sales order. The gateway returns response codes indicating that the address isn't a complete match the cardholder address information and the CSC information isn't a match. According to the rules in the gateway profile, the payment status for the order is set to Cancel Order and the sales order is canceled.

## Setting Up Order Verification Rules {#bridgehead_N1567973}

You can set up order verification rules when you set up a credit card processing profile for CyberSource or MerchantE. These settings determine how orders are handled based on the address verification (AVS) and credit card verification (CSC) responses returned by the gateway.

#### To set up order verification rules: {#procedure_N1567997}

1.  Go to Setup > Accounting > Payment Processing Profiles, and edit the gateway profile for which you want to set up order verification.
    
2.  On the payment processing profile page, go to Order Verification Settings.
    
3.  Under Address Verification (AVS) Rules, select the action to take for the sales order for each of the AVS responses:
    
    -   **Accept** - payment is approved and order status is set to Pending Approval or Pending Fulfillment.
        
    -   **Cancel Order** - order is canceled.
        
    -   **Verification Review** - a payment hold is placed on the order and must be reviewed for further action.
        
4.  On the **Credit Card Verification (CSC) Rules** subtab, select the action to take for the following gateway CSC responses:
    
    -   **Accept** - payment is approved and order status is set to Pending Approval or Pending Fulfillment.
        
    -   **Cancel Order** - order is canceled.
        
    -   **Verification Review** - a payment hold is placed on the order and must be reviewed for further action.
        
5.  Click **Save**.
    

### Related Topics

-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)
-   [Reviewing Payment Status and Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html#section_N1568265)
-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
