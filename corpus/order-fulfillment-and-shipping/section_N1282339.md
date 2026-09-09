---
id: "section_N1282339"
type: "section"
title: "Printing UPS Shipping Labels and Forms"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > Printing UPS Shipping Labels and Forms"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html"
anchors: ["bridgehead_N1282454", "procedure_N1282504", "bridgehead_N1282650", "procedure_N1282724", "bridgehead_N1282768", "procedure_N1282842", "bridgehead_N1282885", "procedure_N1282941", "bridgehead_N1282984", "procedure_N1283011"]
sha256: "735cb62216a7b18113d1c7e3eb7982a4d9bb5eb74d9d6ae417b5e720a177767f"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

To print UPS barcode shipping labels, enable the Shipping Label Integration feature. After you create a sales order that includes an integrated shipping item, fulfilled the sales order, and check the Generate Shipping Label box.

Note:

If you use Shipping Label Integration with an integrated shipping carrier, you cannot override addresses to generate shipping labels. On the Address window, enter the complete shipping information in the address fields.

Before printing a UPS label for an international shipment, ensure you've added emails addresses in the Shipper Email Address and Ship Notification Email Addresses on the Carrier subtab of the item fulfillment. UPS uses these addresses for shipment and customs notifications.

You can print the following labels and forms for UPS shipping items:

-   [Printing UPS Shipping Labels as PDFs](#bridgehead_N1282454)
    
-   [UPS Commercial Invoices](#bridgehead_N1282650)
    
-   [UPS Shipper's Export Declaration (SED)](#bridgehead_N1282768)
    
-   [UPS Certificates of Origin](#bridgehead_N1282885)
    
-   [UPS High Value Report](#bridgehead_N1282984)
    

Note:

If you use a thermal printer for shipping labels, install the thermal printer driver. To learn more, see [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).

## Printing UPS Shipping Labels as PDFs {#bridgehead_N1282454}

You can print a UPS barcode shipping label after you complete the following:

-   Create an integrated shipping item.
    
-   Create a sales order with the shipping item.
    
-   Fulfill the sales order and have checked the generate an integrated shipping label box.
    

If you generate return labels, they are included when you print shipping labels.

Integrated shipping labels should be printed on a 8.5" x 5.5" sheet when you are printing using PDF format. However, you can also use a 8.5" x 11" piece of paper and fold the sheet of paper in half.

You can also print labels in EPL or ZPL formats using a thermal printer. The label type must be 4' x 6' thermal label without doc tabs. To learn more, see [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).

#### To set a default shipping label format:

1.  Go to _Setup > Accounting > Shipping_.
    
2.  Click the UPS account link.
    
3.  In the UPS Developer Kit Registration window, select the **UPS Label** type.
    
    To learn more, see [UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html).
    
4.  Click **Save**.
    

#### To print an integrated shipping label in PDF format: {#procedure_N1282504}

1.  After fulfilling an order, go to _Transactions > Management >Print Checks and Forms_.
    
2.  Click **Integrated Shipping Labels**.
    
3.  To begin printing on the first label of the first sheet of labels, in the **Starting Label** field, enter 1.
    
    Enter 2 to begin printing on the second half, or second label, on the sheet of labels.
    
4.  To print any of the shipping labels more than one time, check the **Allow Reprinting** box.
    
5.  To print PDF labels on 8.5" x 11" paper, with one label printed per sheet of paper, check the **Single Label Per Page** box.
    
    To use 8.5" x 5.5" labels or to print 2 labels per page, clear this box.
    
6.  To print shipping labels by location, select a **Location**.
    
7.  Select a **Ship Date**.
    
8.  Alternatively, enter a **From** and **To** date to create a date range to filter the list of fulfilled sales orders.
    
9.  In the **Print** column, check the box next to each order you want to print a label for.
    
    -   To check the boxes for all items, click **Mark All**.
        
    -   To view the sales order, click the **Order Date**.
        
    -   To view the item fulfillment for that order, click the **Ship Date**.
        
    
    The UPS Shipping Labels in the Queue field shows the number of labels you have marked for printing.
    
10.  Click **Print**.
     
     A window opens with instructions on how to download your label.
     
11.  Attach the label to the package for the order, and it is ready for drop-off or pick-up.
     

Note:

After an integrated shipping label has been generated for a particular order, the format of the print label cannot be revised. For example, if ZPL was used as the label printing format it cannot subsequently be changed to PDF.

## UPS Commercial Invoices {#bridgehead_N1282650}

The commercial invoice acts as a bill of sale between the shipper/seller and the receiver/buyer. Commercial invoices include the following:

-   The products being shipped
    
-   The origin of the products
    
-   The use of the products
    
-   The total value of each item
    
-   The number of packages
    
-   The total weight
    

Commercial invoices are used for international shipments containing items that are not documents. The invoice is the primary document for import control, valuation, and duty determination.

Information about commercial invoices is pulled from fields on the International subtab of item fulfillments and the Basic subtab of item records.

Note:

To print UPS international forms, you must have international shipping enabled at _Setup > Accounting > Shipping_. Select the Preferences subtab.

#### To print a commercial invoice for a UPS-integrated order: {#procedure_N1282724}

1.  Go to _Transactions > Management >Print Checks and Forms_.
    
2.  Click **UPS International Forms**.
    

## UPS Shipper's Export Declaration (SED) {#bridgehead_N1282768}

Shipper's Export Declarations (SEDs) are used for developing export statistics controls. SED forms are required to ship single commodities valued over US$2,500 or commodities requiring a license or license exception. To learn more, see [www.census.gov/foreign-trade](http://www.census.gov/foreign-trade).

The shipment value is the Declared Value listed on an order's Packages subtab. This may be different than the item price.

SEDs are required in the following instances:

-   Shipments from the United States to all foreign countries, Puerto Rico, and the U.S. Virgin Islands. SEDs are not required from the U.S. to Canada if an export license is not required.
    
-   Shipments from Puerto Rico to all foreign countries, the U.S. and the U.S. Virgin Islands.
    
-   Shipments from the U.S. Virgin Islands to foreign countries.
    

#### To enable international shipping:

1.  Go to _Setup > Accounting > Shipping_
    
2.  Click the **Preferences** subtab.
    
3.  In the **Carrier Basics** section, check the International Shipping box.
    
4.  Click **Save**.
    

Enclose a printed SED form with your package or with the lead package in a multi-package shipment. NetSuite does not electronically send SEDs.

Important:

Printed SEDs must conform to the official form in every respect, including paper color. Forms must be printed on buff (yellow) or goldenrod colored paper. They will not be accepted on white paper.

#### To print Shipper's Export Declaration forms for UPS: {#procedure_N1282842}

1.  Go to _Receiving > Receiving >Print Checks and Forms_.
    
2.  **Click UPS International Forms**.
    

## UPS Certificates of Origin {#bridgehead_N1282885}

For any order with items manufactured in the United States or Puerto Rico, a certificate of origin is automatically generated when the order is fulfilled.

Additionally, if the order is being shipped under the North American Free Trade Agreement (NAFTA), a NAFTA certificate of origin is generated. The NAFTA Certificate of Origin authenticates the country of origin of the merchandise being shipped under the North American Free Trade Agreement (NAFTA). A NAFTA Certificate of Origin is required for shipments between the U.S., Canada, and Mexico for the reduced or eliminated duty allowed under NAFTA.

Shipments requiring a NAFTA Certificate of Origin should be valued at greater than:

-   US$1,000 from the U.S. to Mexico
    
-   US$1,600 from the U.S to Canada
    
-   US$2,500 from Mexico or Canada to the U.S.
    

#### To print Certificates of Origin: {#procedure_N1282941}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **UPS International Forms**.
    

## UPS High Value Report {#bridgehead_N1282984}

To insure UPS shipments with a declared value over US$999, complete a High Value Report and have the sender and UPS driver sign it. Each report defines the value of the shipments' contents for a single order. If an order has multiple packages, one report contains information for all packages.

#### To print a UPS High Value Report: {#procedure_N1283011}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  **Click UPS High Value Report**.
    

### Related Topics

-   [Printing Shipping Labels](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262680.html)
-   [UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html)
-   [Fulfilling Orders with UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1279306.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
