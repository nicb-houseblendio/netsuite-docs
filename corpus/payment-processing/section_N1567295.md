---
id: "section_N1567295"
type: "section"
title: "Credit Card Authorization"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Accepting Credit Card Payments > Credit Card Authorization"
parent: "section_N1569326"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html"
anchors: ["bridgehead_N1570082"]
sha256: "23d3ad016d1b565a091634fedb6327352ab592e18816be58535ef383e23acf2d"
---

NetSuite sends a request to your credit card processing gateway to authorize the card for payment and verify the billing address and the security code of the card, if available. An authorization request is sent when:

-   a shopper submits an order in your Web store
    
-   you save an internal sales order with the Get Authorization box checked
    

If the authorization is successful, the gateway returns a response to NetSuite and includes an authorization code.

Orders with authorized credit card payments are saved and advance in your order management workflow. Generally, authorization is held for 3-7 days and can be captured against for up to 30 days.

Orders that are not approved for payment are either saved for review or canceled based on the type of order, your processing gateway, order verification rules, and if you use CyberSource, Decision Manager settings.

If an internal order (MOTO) gets an authorization decline or processing error, NetSuite flags it with a payment hold and saves it for review.

Web store orders with processing errors are placed on hold and saved for review. Web store orders with an authorization decline aren't saved, except in one case. If you use CyberSource Decision Manager with a third-party web store and connect to NetSuite using SOAP web services, web store orders with an authorization decline are saved in NetSuite.

For all other web store orders with an authorization decline, the shopper needs to fix their credit card info before they can submit the order.

Note:

For gateways other than CyberSource and MerchantE, system errors and gateway errors are reported as authorization declines.

| Hold Reason | Order Type | CyberSource | MerchantE | Others |
| --- | --- | --- | --- | --- |
| System Error | All | Yes | Yes | Yes |
| Gateway Error | All | Yes | Yes |
| Authorization Decline | Internal orders | Yes | Yes |
| Verification Required | All | Yes | Yes | \- |
| External Fraud Review | All | Yes | \- | \- |
| External Fraud Reject | All | Yes | \- | PayPal PayFlow Pro - Yes All others - Not Applicable |

If you use CyberSource or MerchantE, you can set up order verification rules for payment authorizations. For more information, see [Order Verification Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567770.html).

## Searching and Reporting on Credit Card Authorization Status {#bridgehead_N1570082}

You can customize a search or report for sales orders to include credit card authorization information. The following fields are available for searches and reports:

-   AVS Street Match
    
-   AVS Street Zip
    
-   CSC Match
    

### Related Topics

-   [Payment Card Number Security and Compliance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567137.html)
-   [Customer Credit Card Processing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1566458.html)
-   [Reviewing Payment Status and Sales Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1570238.html#section_N1568265)
-   [Voiding Credit Card Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1570067.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
