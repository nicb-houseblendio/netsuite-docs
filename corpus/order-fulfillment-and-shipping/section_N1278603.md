---
id: "section_N1278603"
type: "section"
title: "UPS Integration with Multiple Locations"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > UPS Integration with Multiple Locations"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278603.html"
anchors: ["procedure_N1278628"]
sha256: "d89a13edc289c7dd68a2cd42ba867d1cd4824ffd2a815c72601fc70d1a61a7df"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

When Multi-Location Inventory and Shipping Label Integration feature are enabled, NetSuite enables you to set up a different UPS accounts for each location.

-   You can then receive UPS real-time rates and labels specific to the shipping warehouse and define pick-up preferences for each warehouse.
    
-   When creating an sales order, you can select which location will fulfill a sales will be fulfilled.
    
-   When you fulfill the order, the shipping charges reflect the location you selected on the sales order. You cannot fulfill a sales order with items from more than one location.
    

#### To set up locations with shipping integration: {#procedure_N1278628}

1.  Go to _Setup > Accounting > Shipping_.
    
2.  Click **Add UPS Account**.
    
3.  Click **Agree**.
    
4.  Select an account **Location**. You can only create one UPS registration for each location.
    
    To learn more, see [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html).
    
5.  Complete the registration form using the selected location address.
    
    To learn more, see [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274) or [Registering a UPS Account (UK)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274638.html).
    
6.  Click **Submit**.
    

Note:

You cannot delete or inactivate a UPS account from NetSuite. If you no longer use a location that was set up with a shipping account, inactivate the location record. Contact UPS to cancel an account.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics

-   [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274)
-   [Registering a UPS Account (UK)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274638.html)
-   [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
