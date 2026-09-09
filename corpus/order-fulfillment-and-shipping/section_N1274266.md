---
id: "section_N1274266"
type: "section"
title: "UPS"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS"
parent: "chapter_N1257369"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html"
anchors: ["bridgehead_N1274274", "procedure_N1274362"]
sha256: "f929f2fe30e5863b864547012b909458eca6a2a2e9f417580cf61ee7ff3e0d0d"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

## Registering a UPS Account {#bridgehead_N1274274}

You can offer UPS shipping items with real-time rates on all origin and destination locations by registering your active UPS account in NetSuite.

After registration, a new option for real-time rates when creating new shipping items is displayed. When a shipping item using UPS real-time rates is created, the current rates are applied to the Amount field in your website and on the transaction pages for the item purchase. The rate is a close estimate of the final shipping cost, but may vary slightly depending on the package size.

The Shipping Label Integration feature can automatically charge your account with each fulfilled order, receive tracking numbers, and print UPS barcode shipping labels and return labels from your NetSuite account. To learn more, see [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html).

To use UPS Developer Kit, on the Set Up Shipping page, select the Charge for Shipping box.

UPS can validate the shipping address during the order fulfillment stage. Address validation is only available for U.S. and Canada shipments. If the address is not valid, you receive a prompt to verify and correct the shipping address. To use address validation, check the UPS Address Validation box on the Set Up Shipping page. See [Setting Shipping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html#bridgehead_N1257598).

For UPS international shipments, you should enter both Shipper Email Address and Receiver Email Address (Ship Notification Email Addresses) to help reduce cross-border delays and enable faster issue resolution. Enter these addresses on the Carrier subtab of the item fulfillment before generating an integrated shipping label.

#### To register your UPS account in NetSuite: {#procedure_N1274362}

1.  Go to _Setup > Accounting > Shipping_.
    
    This procedure applies to all editions of NetSuite. The address field names will change based on the shipping location country.
    
    To learn how to register a UPS Account in the United Kingdom, see [Registering a UPS Account (UK)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274638.html).
    
2.  Click **Add UPS Account**.
    
3.  Read the consent form for the UPS Device ID and click **OK**.
    
4.  Read the terms of agreement, and then select **I Accept**.
    
5.  If you use the Multiple Location Inventory feature, select the **Location** this UPS account should be associated with.
    
6.  Enter **Name** of the person responsible for the UPS account.
    
7.  Enter the job **Title** for the person responsible for the UPS account.
    
8.  Enter your **Company** name as it appears on the UPS carrier account registration form.
    
9.  Enter the name of the company contact in the **Ship to Attention** field.
    
10.  Enter the company location information as it appears on the UPS account registration form.
     
     -   **Address**
         
     -   **Town**
         
     -   **Zip** code
         
     -   **Country**
         
     -   **State**
         
11.  Enter the contact information for the person responsible for the UPS account:
     
     -   **Phone** number
         
     -   **Email** address
         
12.  Select whether to receive **Notification** when login information is about to expire.
     
13.  Enter the **Company URL** for the company website.
     
14.  Select the **UPS Pickup Type**.
     
15.  Select the **UPS Label** print method. To learn more, see [Printing UPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html).
     
16.  If customers want to pay when receiving deliveries, select a **UPS COD Method**.
     
17.  To print PDF labels and print one label per 8.5' by 11" sheet of paper, check the **Single Label per Page**
     
     This lets you fold the paper to use the label rather than separating the two labels.
     
18.  In the **Shipper Account** section, enter your **UPS Account Number**, **Zip** code, and **Country**.
     
19.  In the **Invoice Information** section, if you want a UPS Sales representative to contact you check the **Yes** box.
     
20.  Click **Print Agreement** to keep a hard copy of this agreement.
     
21.  Click **Submit**.
     

You can now create UPS shipping items with real-time rates and recalculate those rates on transactions before you ship.

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer\* on each shipping screen and shipment notification viewed by your customer. These elements are permanent and cannot be deleted or altered.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics:

-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [Printing UPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
