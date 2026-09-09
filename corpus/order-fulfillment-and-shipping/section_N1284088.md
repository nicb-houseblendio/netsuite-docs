---
id: "section_N1284088"
type: "section"
title: "USPS Real-Time Rates"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > U.S. Postal Service/Endicia > USPS Real-Time Rates"
parent: "section_N1283121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html"
anchors: ["procedure_N1284419", "procedure_N1284460"]
sha256: "305ee55fc91deffa487295907fbbaccbfab826411e3ee54e8db58120858edd3a"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

Registering your U.S. Postal Service (USPS) account with NetSuite, enables you to offer USPS shipping options with real-time rates for world-wide shipping. When a customer ships a purchase by USPS, the current rate for the customer's location fills in the Shipping field in your website and the Shipping Cost field on transaction pages.

Note:

The rate is a close estimate of the final shipping cost but may vary slightly depending on the package size.

Your administrator can add a USPS account to NetSuite. To learn more, see [United States Postal Service (USPS) Services through Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283121.html#bridgehead_N1283130).

After adding a USPS account, you can create shipping items to charge customers USPS real-time rates. To learn more, see [Creating Shipping Items with USPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283792.html).

To offer USPS real-time rates, select one of the following real-time shipping item rate options:

To learn more, see [USPS](https://www.usps.com/ship/first-class-mail.htm)

-   **USPS First-Class Mail** - Deliver packages weighing 13 ounces or less, including boxes, thick envelopes, or tubes. If your package weighs more than 13 ounces, use Priority Mail.
    
-   **USPS Priority Mail** - Two-day delivery service for documents and packages to mailboxes, mail slots, and P.O. Boxes. Saturday delivery and residential delivery available at no extra cost.
    
-   **USPS Priority Mail Express** - Overnight delivery guaranteed to most locations or your money back. Delivery to most destinations 365 days a year including Sundays and holidays, no Saturday charge, no fuel surcharge, free tracking information, and signature proof of delivery upon request.
    
    **USPS Bound Printed Matter** - Deliver small and large packages containing permanently bound sheets of directory, advertising, or editorial matter, such as catalogs or phone books. Permanently bound sheets should be secured with staples, spiral binding, glue, or stitching. Prices based on weight and distance.
    
-   **Shipping for Business** - Economical ground delivery service for large and medium sized shippers. Parcel Select packages can weigh up to 70 pounds and measure up to 130 inches in combined length and distance around the thickest part. Rates are based on weight, distance, and shape. A surcharge applies to certain items including packages weighing over 35 pounds (25 pounds for books and printed matter) and certain shapes. For example, tubes, rolls, and large packages.
    
-   **USPS Retail Ground™** - Deliver small and large packages, thick envelopes, and tubes containing gifts and merchandise, available for retail and USPS approved shippers. Standard Post packages can weigh up to 70 pounds and measure up to 130 inches in combined length and distance around the thickest part. Rates are based on weight, distance, and shape. A surcharge applies to certain items including packages weighing over 35 pounds (25 pounds for books and printed matter) and certain shapes. For example, tubes, rolls, and large packages.
    
    Note:
    
    USPS Retail Ground was formerly known as USPS Standard Post. If you used the shipping item, USPS Standard Post, you should inactivate it and add a new shipping item for USPS Retail Ground.
    
-   **USPS Media Mail** - Deliver books, sound recordings, recorded video tapes, printed music, and recorded computer-readable media. For example, CDs, DVDs, and diskettes. Media Mail can not contain advertising except for incidental announcements of books. The maximum weight for Media Mail is 70 lbs.
    
-   **USPS Express Mail International** - Deliver documents and packages around the world with service guaranteed to Australia, China, Hong Kong, Japan, and Korea (the Republic of) (South Korea).
    
-   **USPS Priority Mail Express International** - Deliver correspondence and merchandise up to 70 pounds to over 190 countries and territories worldwide.
    

Your preferences in the following fields override the real-time rates:

-   Free if total is over
    
-   Minimum shipping amount
    
-   Maximum shipping amount
    

## NetSuite calculates USPS rates based on the following: {#procedure_N1284419}

-   If the packaging material is provided by the shipper
    
-   If the destination is a commercial destination. Residential rates are higher in some delivery areas.
    
-   If multiple products are placed in one package, the package weight may be less than the estimated rate submitted due to weight rounding
    
-   The rate is determined by product weight only. Some packages may incur additional USPS fees based on package dimensions or additional services
    

#### To ship an order with a USPS real-time rate option: {#procedure_N1284460}

1.  Select the USPS real-time rate **Shipping Method**.
    
2.  There is a pause when NetSuite receives the real-time rate from USPS, then displays the price.
    
3.  Complete order.
    
4.  Authorize and then fulfill the sales order.
    
    Before saving the item fulfillment, click **Recalculate Shipping** to update the real-time rate.
    
5.  After the package is dropped off or picked up by USPS, you can retrieve a tracking number to track the status of the shipment. You can share this tracking number with your customer.
    
6.  You can manually enter the tracking number on a sales order page one time, and the number then appears everywhere the order appears, including in the confirmation email to the customer and in the Customer Center.
    
7.  The tracking number appears as a link in the confirmation email to the customer.
    

### Related Topics

-   [United States Postal Service (USPS) Services through Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283121.html#bridgehead_N1283130)
-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [Creating Shipping Items with USPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283792.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
