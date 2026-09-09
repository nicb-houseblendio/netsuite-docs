---
id: "section_N1282176"
type: "section"
title: "Applying Discounts to UPS Shipping Rates"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > Applying Discounts to UPS Shipping Rates"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282176.html"
anchors: ["procedure_N1282230"]
sha256: "cd6e2bffdbcdec06dfe39e0f437b35ca75c5deb8b5a4f06c97fac228b56687a6"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

If you receive discounts from UPS, or want to offer a discount to your customers and cover the remainder of the cost, you can display discounted shipping rates to your customers.

Discounted UPS rates can be offered when you use real-time rates. To learn more, see [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html).

To offer free shipping, use promotions or create a shipping item with a flat rate of $0.00. Do not set the discount rate on an existing shipping item to 0.

To learn more, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html) and [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html).

#### To offer a discount for a UPS shipping item: {#procedure_N1282230}

1.  Go to _Lists > Accounting > Shipping Items_.
    
2.  Beside the shipping item to offer a discount for, click **Edit**.
    
3.  Click the **Shipping Rate** subtab.
    
4.  Select **UPS Real-Time Rate**.
    
5.  Enter the **Discount Rate**. This number is multiplied by the rate by to receive the correct discount.
    
    For example, if you want to offer a 25% discount off the real-time rate UPS returns, enter 0.75.
    
6.  Click **Save**.
    

The discounted rate now shows on transactions and on your Web site.

Note:

The UPS real-time rate is multiplied by the discount rate to calculate the discounted shipping rate.

### Related Topics

-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html)
-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
