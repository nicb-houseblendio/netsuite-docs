---
id: "section_N1278765"
type: "section"
title: "UPS Real-Time Rates"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > UPS Real-Time Rates"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html"
anchors: ["bridgehead_1548359998", "procedure_N1279158"]
sha256: "beafa780a20caa5522fc60aa1d678dc527d663369020035007d2ad3e71f68496"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

Registering your UPS account in NetSuite enables you to offer UPS shipping options with real-time rates. When a customer purchase is to be shipped by UPS, the customer location current rate appears in the Amount field in your website and on transaction pages. The rate is a close estimate of the final shipping cost but may vary slightly depending on the package size.

To learn more, see [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274).

Real-time rates are calculated based on item weight, the selected shipping method, pickup frequency, sender zip code, and recipient zip code.

If you have enabled Shipping Label Integration, you can choose to automatically charge orders to your UPS account. You can also receive tracking numbers and print UPS barcode labels directly in your account. To learn more, see, [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html).

If you UPS Real-Time Rate, select one of the following:

To learn more, see [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html).

**U.S. Domestic**

-   **UPS 2nd Day Air** - delivery by the end of the second business day from order placement in the United States, including Puerto Rico, excluding intra-Alaska shipments
    
-   **UPS 2nd Day Air A.M.** - delivery by noon of the second business day to commercial addresses where Next Day Air delivery is committed by 10:30 am
    
-   **UPS 3 Day Select** - delivery within three business days for every address in the contiguous United States
    
-   **UPS Ground** - ground delivery for every address in the contiguous United States guaranteed by the selected date
    
-   **UPS Next Day Air** - delivery by 10:30 am, noon, or 1:30 pm on the next business day to every address in all 50 states and Puerto Rico. Time of day depends on the destination
    
-   **UPS Next Day Air Saver** - more affordable next day delivery by 3:00 pm or 4:30 pm to commercial locations where Next Day Air is available by 10:30 am or noon, respectively
    
-   **UPS Next Day Early A.M.** - delivery by 8:00 am the next day on weekdays to major cities in the 48 contiguous states and by 8:30 am in other major cities, such as Anchorage, Alaska
    

For domestic options in other countries, please visit the UPS Web site at [www.ups.com](https://www.ups.com/us/en/Home.page).

**International**

-   **UPS Express Saver**SM - guaranteed delivery during the day, including shipments to, from, and within Europe. Economical alternative to UPS Express service
    
-   **UPS Standard** - day-definite delivery to Canada
    
-   **UPS Worldwide Expedited** - delivery to more than 61 international destinations in 2-5 days
    
-   **UPS Worldwide Express** - delivery by 10:30 am or 12:00 noon. Next business day delivery to Canada, and for documents to Mexico. Second business day delivery to Europe and Latin America, and within two to three business days to Asia. Delivery to over 60 countries and territories
    
-   **UPS Worldwide Express Plus** - next day delivery by 8:30 am to Canada. Delivery by 9:00 am within two business days to Europe and by 9:00 am within two or three business days to Asia. Delivery to over 25 countries and territories in Canada, Europe, and Asia
    
-   **UPS Worldwide Saver** - delivery by end of day. Next business day delivery to Canada, and for documents to Mexico. Second business day delivery to Europe and Latin America, and within two to three business days to Asia. Delivery to 215 countries and territories
    

To learn more, see [www.ups.com](http://www.ups.com).

Your preferences in the Free if total is over, Minimum shipping amount, and Maximum shipping amount fields override the real-time rates.

## NetSuite UPS Rate Calculation {#bridgehead_1548359998}

NetSuite considers the following factors when calculating UPS shipping rates:

-   Whether the package is picked up during regular daily UPS pickup
    
-   Whether the packaging material is provided by the shipper
    
-   Whether the destination is a commercial destination. Residential rates are higher in some delivery areas
    
-   Whether multiple products are placed in one package. The weight of the package may be less than the estimated rate submitted due to weight rounding
    
-   Whether the rate determined by product weight only. Some packages may incur additional UPS fees based on package dimensions or additional services, such as Saturday delivery
    

Weight and size limits apply to all packages sent by UPS domestic air and ground services. The maximum size for a package is 130 inches combined length (the longest side of the package), girth (the distance all the way around the package at its widest point perpendicular to the length), and the maximum length per package is 108 inches.

#### To ship an order using UPS real-time rate process: {#procedure_N1279158}

1.  In the **Shipping Method** field, select a UPS real-time rate option.
    
    NetSuite pauses to receive the real-time rate from UPS and then display the price.
    
2.  The customer completes the order.
    
3.  The order is authorized and fulfilled.
    
    Before saving the item fulfillment, to update the real-time rate, click **Recalculate Shipping**.
    
4.  After UPS obtains the package, you are given a tracking number to help you, and your customer, to follow the shipment status. UPS's Worldship software enables you to generate your own shipment tracking number.
    
5.  Enter the tracking number on a sales order page and the number then appears everywhere the order appears. This includes the customer confirmation email and in the Customer Center.
    
6.  The tracking number appears as a link in the confirmation email to the customer.
    
    Click the link to display the order status in the UPS website.
    

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer\* on each shipping screen and shipment notification viewed by your customer. These elements are permanent and cannot be deleted or altered.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics

-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [Applying Discounts to USPS Shipping Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284917.html)
-   [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html)
-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
