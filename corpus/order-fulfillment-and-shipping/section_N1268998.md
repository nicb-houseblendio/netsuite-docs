---
id: "section_N1268998"
type: "section"
title: "FedEx Real-Time Rates (U.S. and Canada)"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > FedEx Real-Time Rates (U.S. and Canada)"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html"
anchors: ["procedure_N1269384", "procedure_N1269440"]
sha256: "845268e67601bdb240aed4419bedbd1d82dcdc72fcffff369de3d830438dd6a8"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

After you register your FedEx account with NetSuite, you can offer FedEx shipping options with real-time rates. When a customer ships with FedEx, the customer's location current rate is automatically entered into in the Amount field on your website and transaction pages.

Note:

Rates for orders to be shipped from a Canadian location do not include Canadian tax.

During the order fulfillment, FedEx can validate the package shipping address. Address validation is available for more than 40 countries. If the address is not valid, an error message is sent to verify and correct the shipping address. To learn more, See [Setting Shipping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html#bridgehead_N1257598).

After adding a FedEx account, you can create shipping items that charge customers FedEx real-time rates. Real-time rates are calculated based on the item's weight, the selected shipping method, the frequency of pickups, and the zip code.

To offer FedEx real-time rates, select one of the following real-time rate shipping item options:

-   **FedEx First Overnight** - Overnight delivery in the contiguous U.S. by 8:30 am to most major markets
    
-   **FedEx First Overnight Freight** - Next business day delivery available in all 50 U.S. states including Hawaii (to the island of Oahu)
    
-   **FedEx Priority Overnight** - Overnight delivery in the U.S. by 10:30 am for most addresses, with later times of day in rural areas or on Saturday
    
-   **FedEx Standard Overnight** - Overnight delivery in the U.S. by 3 pm, or 4:30 pm in rural areas. This option is not available for Canadian accounts
    
-   **FedEx 2Day** - Delivery in the U.S. by 4:30pm (7:00 pm to residences) in two business days
    
-   **FedEx Express** - Package weight must be under 10 pounds
    
-   **FedEx Express Saver** - Delivery in the contiguous U.S. by 4:30 pm (7:00 pm to residences) in three business days. This option in not available for Canadian accounts
    
-   **FedEx Ground** - Delivery in one to five business days in the contiguous U.S., three to seven days to or from Alaska or Hawaii
    
-   **FedEx Economy** - Delivery by 5:00 pm in one to three business days. Available in Canada only
    
-   **FedEx 2Day A.M.** - Delivery by 10:30 am in two business days, except some shipments to Alaska and Hawaii in three business days
    
-   **FedEx Home Delivery** - Delivery to residences in one to five business days in the contiguous U.S., three to seven business days to or from Alaska or Hawaii. This option is not available for Canadian accounts
    
-   **FedEx International First** - Delivery by 8:30 am in two business days to Basel, Brussels, Frankfurt, London, Milan, or Paris
    
-   **FedEx International Priority** - Time definite delivery in one to three business days to more than 210 countries
    
-   **FedEx International Economy** - Delivery in two to five business days (three to ten business days to Mexico or Puerto Rico) to more than 205 countries
    
-   **FedEx International Priority Freight** - Time definite delivery in one to three business days to more than 50 countries for packages over 150 pounds
    
-   **FedEx International Economy Freight** - Time definite delivery in four to five business days to more than 45 countries for packages over 150 pounds
    
-   **FedEx 1Day Freight** - Delivery between 10:30 am-12:00 pm the next business day in the U.S., except Hawaii, for packages over 150 pounds
    
-   **FedEx 2Day Freight** - Delivery between 12 pm-3:00 pm in two business days in the U.S., except Hawaii, for packages over 150 pounds. This option is not available for Canadian accounts
    
-   **FedEx 3Day Freight** - Delivery by 3:00 pm in three business days in the contiguous U.S. for packages over 150 pounds. This option is not available for Canadian accounts
    
-   **FedEx Ground Economy parcel select lightweight** - Delivery in two to seven business days in the U.S. (longer if outside the contiguous U.S.). Final delivery handled by USPS, including Saturdays. This option is not available for Canadian accounts
    
-   **FedEx Ground Economy Bound Printed Matter** - Cost-efficient delivery of bound printed matter. Final delivery handled by USPS, including Saturdays. This option is not available for Canadian accounts
    
-   **FedEx Ground Economy Media Mail** - Cost-efficient delivery of media mail items. Final delivery handled by USPS, including Saturdays. This option is not available for Canadian accounts
    
-   **FedEx Ground Economy parcel select** - Delivery in two to seven business days in the U.S. (longer if outside the contiguous U.S.). Final delivery handled by USPS, including Saturdays. This option is not available for Canadian accounts
    

Your preferences in the **Free if total is over**, **Minimum shipping amount**, and **Maximum shipping amount** fields override the real-time rates.

## NetSuite calculates FedEx rates based on the following: {#procedure_N1269384}

-   Packages picked up during your regular daily FedEx pickup
    
-   Whether packaging material is provided by the shipper
    
-   If the destination is a commercial destination. Residential rates are higher in some delivery areas
    
-   Multiple products are placed in one package, the weight of the package may be less than the estimated rate submitted due to weight rounding
    
-   The rate is determined by product weight only and some packages may incur additional FedEx fees based on package dimensions or additional services
    

Note:

Weight and size limits apply to all packages that are not sent by FedEx Express Freight. The maximum weight limit for packages is 150 pounds. The maximum size for a package equals 130 inches in combined length (the longest side of the package) and girth (the distance all the way around the package at its widest point perpendicular to the length), and the maximum length per package equals 108 inches. Packages over these weight and size limits can be sent by FedEx Express Freight, which has a 2200 pound weight limit.

#### The FedEx real-time rate option shipping process: {#procedure_N1269440}

1.  The customer selects a FedEx real-time rate **Shipping Method**.
    
2.  NetSuite may pause when receiving real-time rates from FedEx before the price is displayed.
    
3.  The customer completes the order.
    
4.  The sales order is authorized and fulfilled.
    
    Before saving the fulfillment, click **Recalculate Shipping** to update the real-time rate and validate the shipping address.
    
5.  After the package is received by FedEx, a tracking number enables you and your customer to track the shipment status.
    
6.  You can manually enter the tracking number on a sales order page one time. The number then appears everywhere the order appears, including in the confirmation email to the customer and the Customer Center.
    
7.  The tracking number appears as a link in the customer confirmation email.
    

### Related Topics

-   [FedEx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Registering a FedEx Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html#bridgehead_N1267326)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
