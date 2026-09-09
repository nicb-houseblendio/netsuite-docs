---
id: "section_N1272384"
type: "section"
title: "Applying Discounts to FedEx Rates"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > Applying Discounts to FedEx Rates"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272384.html"
anchors: ["procedure_N1272439"]
sha256: "14ecc80572455f8fe77286015202cdb2bc58ce890e2bb19127c919d9ceb741ee"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

NetSuite enables you to display discounted shipping rates to your customers if you receive discounts from FedEx or you want to offer a discount to your customers.

Discounted FedEx rates can be offered when you use real-time rates. To learn more, see [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html).

To offer free shipping, use promotions or create a shipping item with a flat rate of $0.00. Do not set the discount rate on an existing shipping item to 0. To learn, see [Promotions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4690873883.html) and [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html).

#### To offer a discount for a FedEx shipping method: {#procedure_N1272439}

1.  Go to _Lists > Accounting > Shipping Items_.
    
2.  Edit the shipping item record for the method on which you want to offer a discount.
    
3.  Click the **Shipping Rate** subtab.
    
4.  Select **FedEx Real-Time Rate**.
    
5.  In the **Discount Rate** field, enter a number to multiply the rate by to receive the correct discount.
    
    For example, to offer a 25% discount, enter 0.75.
    
6.  Click **Save**.
    
    The discounted rate is displayed on transactions and in your website.
    

### Related Topics

-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html)
-   [Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1258840.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
