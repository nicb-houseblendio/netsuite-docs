---
id: "bridgehead_N1569986"
type: "bridgehead"
title: "Copying a Sales Order with a Credit Card Payment"
branch: "payment-processing"
category: "order-management"
breadcrumb: "Order Management > Payment Processing > Payment Processing Options > Customer Credit Card Processing > Copying a Sales Order with a Credit Card Payment"
parent: "section_N1566458"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1569986.html"
anchors: []
sha256: "98f11da5e955b9a36b62e4568652bc0f3ba8e720fc24399563c90dd77a0caad2"
---

You can copy a sales order with a credit card payment. This is an efficient way to create an additional order for a customer without having to re-enter all their information.

Important:

Don't copy an order and resubmit to correct authorization errors. In this case, change the billing information as needed, check **Get Authorization**, and save the order.

You must be in View mode to copy an order. The following payment information about the Billing subtab copies to the new order:

-   Credit Card # (masked)
    
-   Expires on (MM/YYYY)
    
-   Name on Card
    
-   Card address information
    

The copied order won't show:

-   CSC
    
-   credit card gateway response information including P/N Ref, Auth. Code, AVS Street Match, AVS Zip Match, and CSC Match
    
-   payment events from original transaction
    

On the new order:

1.  Enter the three-digit security code (CSC).
    
2.  Make any other changes that are required.
    
3.  Verify that the **Get Authorization** box is checked.
    
4.  Save the order.
    

### Related Topics

-   [Maintaining Recurring Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3887850446.html)
-   [Accepting Credit Card Payments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1569326.html)
-   _Credit Card Processing Gateway FAQ_
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
