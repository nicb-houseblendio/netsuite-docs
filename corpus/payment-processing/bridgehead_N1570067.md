---
id: "bridgehead_N1570067"
type: "bridgehead"
title: "Voiding Credit Card Transactions"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Accepting Credit Card Payments > Voiding Credit Card Transactions"
parent: "section_N1569326"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1570067.html"
anchors: ["bridgehead_4700636251"]
sha256: "34e4d9042c894418d5c430bb27a02790457f961143935569e71f88e0e170dbcf"
---

NetSuite lets you void (reverse) authorizations by canceling the sales order. When you cancel or close a sales order, NetSuite sends a void request to the payment gateway to void the authorization and release shopper's funds. For details on closing a sales order, see [Closing a Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4698204292.html).

Important:

Voiding authorizations from within NetSuite is supported only for CyberSource and MerchantE gateway integrations.

If the gateway integration doesn't support voiding, you must manually void the transaction through your merchant account at the payment gateway.

Authorizations are automatically voided when your customers cancel their orders in the customer center.

**To void a payment authorization**, on a sales order with Pending Approval status, click **Cancel Order**. If the sales order is pending fulfillment, click **Close Order**.

For the authorization to be voided, the sales order must meet the following conditions:

-   The selected payment processing profile must support the void request.
    
-   The authorization must not be expired or captured.
    

## Status of the Voiding Operation {#bridgehead_4700636251}

Depending on the gateway's response, the void operation can have one of the following results:

-   **Accept** - The sales order is canceled, and funds are released.
    
-   **Hold** - The sales order is canceled, but funds are not yet released. The payment gateway sends subsequent request to NetSuite to update the voiding result.
    
-   **Reject** - The sales order is canceled in NetSuite, but the hold isn't removed. When this happens, contact the payment gateway and void the authorization manually.
    

To check the voiding status on a sales order, click Billing, and then view the payment events under the Payment subtab.

### Related Topics

-   [Credit Card Authorization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1567295.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
