---
id: "section_N1566458"
type: "section"
title: "Customer Credit Card Processing"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing"
parent: "preface_4289351924"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html"
anchors: ["bridgehead_N1566815", "bridgehead_N1566894"]
sha256: "337b4faf6cb4f7df3f92097a6f44ecd0e1a0be68d0e7f6b56558f1d3539e2dab"
---

Use integrated credit card processing in NetSuite to efficiently handle credit card payments for sales orders and website orders.

This all-in-one solution automates decision making to speed up your order-to-cash process and cuts down on manual order screening.

The NetSuite integrated credit card processing provides these benefits:

-   encrypted card numbers for full PCI compliance and secure data storage
    
-   seamless integration for card approval and funds capture for mail orders and telephone orders (MOTO), and Web store orders
    
-   payer authentication and level II and level III purchase card processing for processing cost optimization
    
-   payment holds to review orders for validity
    
-   fraud management using CyberSource's Decision Manager
    
-   enhanced reporting by mapping sales order data to CyberSource reporting fields
    
-   soft descriptors to simplify card statement identification
    

Plus, with CyberSource or MerchantE, you can set up rules to make sure only valid, credit-worthy orders get approved for fulfillment, and flag any that don't meet your payment criteria for review.

You can review these orders one at a time or all at one time.

Use CyberSource Decision Manager for extra verification and fraud management services.

## Credit Card Processing Flow {#bridgehead_N1566815}

The following diagram illustrates the credit card authorization process and the communication between NetSuite and the payment gateway.

![Flowchart with icons that show the steps in the credit card authorization process and arrows to show communication between NetSuite and the payment gateway.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/CCAuthFlowChart.png)

1.  Customer places an order through different channels.
    
2.  NetSuite securely sends an authorization request together with the order information to a payment gateway. The payment gateway receives order information and performs the requested operation. The operation in this example is Authorization.
    
3.  The payment gateway formats the transaction and securely routes the authorization request to the payment processor or clearing house.
    
4.  The transaction is routed to the issuing bank (shopper's bank) to request placing a hold on the shopper's funds.
    
5.  The transaction is authorized or declined by the issuing bank.
    
6.  The payment gateway forwards the processing result to NetSuite.
    
    If the issuing bank authorizes the transaction, an order is submitted in NetSuite with a Pending Fulfillment or Pending Approval status.
    

## Transferring Credit Card Funds {#bridgehead_N1566894}

The following diagram illustrates the funds settlement (capture) process.

![Flowchart with icons that show the steps in the fund settlement (capture) process and arrows to show communication between NetSuite and the payment gateway.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/OrderManagement/PaymentProcessing/CCCaptureFlowChart.png)

1.  When you bill the sales order, NetSuite sends a capture request to the payment gateway.
    
2.  The payment gateway checks with the issuing bank if funds are already authorized. If not, some gateways automatically reauthorize funds.
    
3.  If funds are authorized, the gateway adds the capture request to a batch of requests. This batch is sent to the issuing bank for processing at the end of every day.
    
4.  The issuing bank is asked to verify the fund transfer to the merchant's account.
    
5.  The issuing bank approves the transfer of money to the acquiring bank (merchant's bank).
    
6.  The acquiring bank credits the merchant's account.
    

### Related Topics

-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   [Auto-charge Credit Card](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1500449969.html)
-   [Setting Up Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572221.html)
-   [Setting Up Payment Processing Profiles in NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1572588.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
