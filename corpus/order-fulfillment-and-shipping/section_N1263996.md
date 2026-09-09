---
id: "section_N1263996"
type: "section"
title: "Shipping Integration with FedEx, UPS, and USPS/Endicia"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Shipping Integration with FedEx, UPS, and USPS/Endicia"
parent: "chapter_N1257369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html"
anchors: ["bridgehead_N1264175"]
sha256: "21d82f4eae2b402f0caec02649982fc2e0189409fd11e762559074d6e331c22e"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

The Shipping Label Integration feature enables you to generate tracking numbers and shipping labels in your NetSuite account. After you register your FedEx, UPS, or USPS/Endicia account with NetSuite, you can create real-time rate shipping items so that the shipping charges on orders are always up to date.

Note:

If you use the Shipping Label Integration feature and an integrated shipping carrier, you cannot override addresses to generate shipping labels. Make sure that you enter the complete shipping information in the Address window, address fields.

#### To set up shipping label integration:

1.  Go to _Setup > Company > Enable Features_.
    
2.  Click the **Transactions** subtab.
    
3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
    
4.  Click **Save**.
    

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer on each shipping screen and shipment notification. These elements are permanent and cannot be deleted or altered.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

## Shipping Carrier Integration Options {#bridgehead_N1264175}

Real time rates and shipping label integration are available for the following carriers based on shipment origin and destination:

| Ship From | Ship To | Carriers |
| --- | --- | --- |
| U.S. | U.S. | FedEx, UPS, USPS/Endicia |
| U.S. | International | FedEx, UPS, USPS/Endicia |
| Canada | U.S. | FedEx, UPS |
| International | U.S. | UPS\* |
| International | International | UPS\* |

\*available in countries where carrier provides service

Important:

When you use the Shipping Label Integration in NetSuite Sandbox or Release Preview accounts, you must use the same production carrier account used in your production NetSuite account.

Any labels generated in Sandbox or Release Preview are live, shippable labels and may incur carrier charges. Contact your carrier directly to understand billing and how to avoid unintended charges.

For more information, see [Important Update: Shipping Label Integration in Sandbox and Release Preview](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046102/kw/1046102) (SuiteAnswers article 1046102).

### Related Topics:

-   [Tracking Numbers with Shipping Label Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265305.html)
-   [Shipping Integration with Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265431.html)
-   [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html)
-   [Shipping Integration and Third Party Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265784.html)
-   [Integrating with Multiple Shipping Carriers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html)
-   [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html)
-   [FedEx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html)
-   [UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html)
-   [U.S. Postal Service/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283121.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
