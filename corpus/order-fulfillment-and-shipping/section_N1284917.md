---
id: "section_N1284917"
type: "section"
title: "Applying Discounts to USPS Shipping Rates"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > U.S. Postal Service/Endicia > Applying Discounts to USPS Shipping Rates"
parent: "section_N1283121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284917.html"
anchors: ["procedure_N1284971"]
sha256: "721d3de05f75aa0cb7a9c2f7149420e374dcc363b828d6c9bd71c607976f80ba"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

If you receive discounts from U.S. Postal Service (USPS) or want to offer a discount to your customers and cover the remainder of the cost, you can display discounted shipping rates to your customers.

Discounted USPS rates can be offered when you use real-time rates. To learn more, see [USPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html).

To offer free shipping, use promotions or create a shipping item with a flat rate of $0.00. Do not set the discount rate on an existing shipping item to 0. To learn more, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html) and [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html).

#### To offer a discount for a USPS shipping item: {#procedure_N1284971}

1.  Edit the shipping item record for the method on which you want to offer a discount.
    
2.  On the **Shipping Rate** subtab, in the **Discount Rate** field next to the USPS rate, enter a number to multiply the rate by to receive the correct discount.
    
    For example, if you want to offer a 25% discount off the real-time rate USPS returns, enter 0.75.
    
3.  Click **Save**.
    

The discounted rate now shows on transactions and in your Web site.

Note:

The USPS real-time rate is multiplied by the discount rate to calculate the discounted shipping rate.

### Related Topics

-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html)
-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
