---
id: "section_N1278000"
type: "section"
title: "UPS Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > UPS Integration"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html"
anchors: ["procedure_N1278060"]
sha256: "32f3189fc0a6bc07c68e1f8b831178427afb5f400f972134c40c499f1e235f76"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

UPS Integration enables you to connect your NetSuite account directly to your UPS account.

After you fulfill and orders with UPS integrated shipping, your UPS account is charged, and the tracking number is saved with the item fulfillment. You can then print a UPS barcode label for your package. To learn more, see [Printing UPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html).

Before you begin, note the following:

-   Make sure that you registered a UPS account. To learn more, see [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274) or [Registering a UPS Account (UK)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274638.html).
    
-   If you have already registered with UPS to use real-time rates, record your UPS account number as it will be required to activate your account for UPS Integration.
    

#### To get started with UPS Integration: {#procedure_N1278060}

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  In the **Shipping & Receiving** section, and check the **Shipping Label Integration** box.
    
4.  Click **Save**.
    
5.  Go to _Setup > Accounting > Shipping_
    
6.  In the **Default Shipping Carrier** select **UPS**.
    
7.  Click **Save**.
    
8.  Go to _Lists > Accounting > Shipping Items > New_
    
9.  To create a UPS integrated shipping item, click **New**. To learn more, see [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html).
    

After you have created a UPS integrated shipping item, you can enter sales orders with the integrated shipping item selected in the Ship Via field. After you fulfill the order, your UPS account is charged with the rate for the UPS shipping integration method.

Note:

The real-time rate quoted at the time of sale is only an estimate. The charge may vary based on factors such as package size, service additions on the shipment, and account-specific discounts.

If the Multiple Location Inventory feature is enabled, you can set up each location with a separate UPS account number. To learn more, see [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html).

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer\* on each shipping screen and shipment notification viewed by your customer. These elements are permanent and may not be deleted or altered in any way.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics

-   [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274)
-   [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html)
-   [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html)
-   [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
