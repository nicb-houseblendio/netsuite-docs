---
id: "section_N1282009"
type: "section"
title: "Voiding a UPS Order"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > Voiding a UPS Order"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282009.html"
anchors: ["procedure_N1282029"]
sha256: "f42487b9904735e357cd6ab1666be4a23e87f4d853e2dc20a7a97f8d537ac8b0"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

You can void a UPS shipment after you fulfill a sales order in your NetSuite account and UPS has not received the package. This cancels the UPS order and your account is not charged. You cannot void an order after it has been scanned by a UPS driver or drop-off location.

#### To void a UPS shipment: {#procedure_N1282029}

1.  Go to _Transactions > Sales > Fulfill Orders > List_.
    
2.  Beside the fulfillment you want to void, click **Edit**.
    
3.  In the **Actions** list, click **Delete**.
    
4.  In the delete box, select a **Deletion Reason**.
    
5.  Enter the reason for deleting this fulfillment in the **Memo** field.
    
6.  Click **Delete**.
    
    If this order has a UPS integrated shipping item, you receive a message confirming whether the UPS order was voided.
    
    -   If the void is successful, the fulfillment is deleted and UPS will not pickup the order or charge your account. You cannot print a barcode label.
        
    -   If the void is unsuccessful, the fulfillment is still deleted, but a system alert is set up to remind you to contact UPS to manually void the order.
        

The most common reasons for an unsuccessful void are:

-   The package has already been scanned by a UPS driver or drop-off location.
    
-   More than 24 hours has elapsed since the tracking number / label was issued.
    

### Related Topics

-   [Fulfilling Orders with UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1279306.html)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
