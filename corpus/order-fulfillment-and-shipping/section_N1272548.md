---
id: "section_N1272548"
type: "section"
title: "Printing FedEx Shipping Labels and Forms"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > Printing FedEx Shipping Labels and Forms"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html"
anchors: ["bridgehead_N1272684", "bridgehead_N1272785", "procedure_N1272836", "bridgehead_N1272913", "procedure_N1272950", "bridgehead_N1273057", "procedure_N1273133", "bridgehead_N1273993", "procedure_N1274014"]
sha256: "9c07bd5420fb47192efafa7ef55f25ba79a47d4afda38ec395ff7b21bd1844cd"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

#### To print barcode shipping labels using Shipping Label Integration:

1.  Create a sales order that includes an integrated shipping item.
    
2.  Fulfill the sales order.
    
3.  Check the generate shipping label box.
    
4.  Click **Save**.
    

Note:

If you use Shipping Label Integration with an integrated shipping carrier, you cannot override addresses to generate shipping labels. On the Address window, enter the complete shipping information in the address fields.

The first line in a **Ship From** address is taken from the **Attention** field in the location's Address window. The second line is taken from the location's **Name** field.

If you print a FedEx shipping label and have not entered information in the Address window **Attention** field, the shipping label prints the information entered on the **Name** field twice.

NetSuite enables you to print the following labels and forms for FedEx shipping items:

-   [Electronic Trade Documents (ETD) for International FedEx Shipments](#bridgehead_N1272684)
    
-   [Printing FedEx Commercial Invoices](#bridgehead_N1272785)
    
-   [Printing FedEx Shipping Labels in PNG Format](#bridgehead_N1272913)
    
-   [Printing FedEx Shipping Labels as PDFs](#bridgehead_N1273057)
    
-   [Printing FedEx Shipping Manifests](#bridgehead_N1273993)
    

Note:

If you use a thermal printer for shipping labels, install the thermal printer driver. To learn more, see [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).

## Electronic Trade Documents (ETD) for International FedEx Shipments {#bridgehead_N1272684}

FedEx shipping integration enables you to electronically submit trade documents for international shipments. After you fulfill an order using FedEx, FedEx generates an electronic version of the trade documents and then transmits them with your shipment. PDF versions of the documents are attached to the fulfillment record order.

Important:

NetSuite does not support uploading letter head images. This is mandated for shipping to certain countries.

FedEx can electronically generate and submit the following trade documents:

-   Certificate of Origin
    
-   Commercial Invoice
    
-   NAFTA Certificate of Origin
    
-   Pro Forma Invoice
    

The Origin Air Waybill label (Origin AWB Copy) is included with the electronically generated documents.

#### To use the FedEx ETD service, enable the Shipping Label Integration feature:

1.  Go to _Setup >Accounting > Shipping > Preferences_.
    
2.  Select FedEx as the **Default Shipping Carrier**.
    
3.  In the **Preferences** subtab, **Carrier Basics** section, check the **International Shipping** box.
    
4.  Click **Save**.
    
5.  Go to _Lists > Accounting > Items_.
    
6.  Beside the item you ship internationally that you want to update, click **Edit**.
    
7.  Click the **Purchasing/Inventory** subtab,
    
8.  Update the **Manufacturing** and **Shipping** sections, with information required for trade documents.
    
9.  Click **Save**.
    

To learn more, see [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html).

After you fulfill an order using one of the supported international FedEx shipping methods, the Item Fulfillment International subtab displays the trade documents to be generated by FedEx for the shipment.

-   The documents selected by default are based on international shipping guidelines. Verify that the documents are correct for the shipment.
    
-   Check the documentation requirements for the countries you are shipping from, shipping through, and shipping to. Verify that all documents are checked for the shipment. All documents will be generated electronically.
    
-   You do not need to attach a printed version of the trade documents to a shipment.
    
-   After you print the shipping label for an order, FedEx generates the electronic trade documents and stores a PDF version on the Item Fulfillment record.
    
    You can use the print option, Print ETD Copy, available on the Item Fulfillment, if you want to print a paper copy of the trade documents for your reference.
    

Note:

To display all international FedEx ETD documents, enable pop-ups in your Chrome browser.

You cannot print copies of the official FedEx generated electronic trade documents from the Print Checks and Forms page.

## Printing FedEx Commercial Invoices {#bridgehead_N1272785}

All international FedEx shipments with commercial value require commercial invoices. Paper documents with little or no commercial value do not require commercial invoices.

Provide the Shipper's export declaration number for international shipments valuing over $2,500 USD.

After you fulfill integrated orders for international shipment using Shipping Label Integration and have an FedEx account, commercial invoices are generated electronically. You do not need to attach a printed copy to the shipment.

To learn more, see [Electronic Trade Documents (ETD) for International FedEx Shipments](#bridgehead_N1272684).

To print commercial invoices for your reference, you can:

-   On the Item Fulfillment page, click Print option, Print ETD Copy .
    
-   Print a copy from the Print Checks and Forms page.
    

Note:

Commercial invoices printed from the Print Checks and Forms page are not official documents. Do not attach them to a shipment.

#### To print commercial invoices from Print Checks and Forms: {#procedure_N1272836}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **FedEx Commercial Invoices**.
    
3.  To view invoices over a time period, enter the **From** and **To** dates.
    
4.  In the **Print** column, clear the box next to each invoice you do not want to print.
    
5.  Click **Print**.
    

## Printing FedEx Shipping Labels in PNG Format {#bridgehead_N1272913}

After you create an integrated shipping item, fulfill the sales order, and check the Integrated Shipping Label box, you can print a FedEx barcode shipping label.

To select the label type, go to _Setup > Accounting > Shipping_. Click the account you want to edit, and enter your label type choice.

#### To print an integrated shipping label in PNG format: {#procedure_N1272950}

1.  After you have fulfilled the order, go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Integrated Shipping Labels**.
    
3.  To begin printing on first label of the first sheet of labels, enter 1 in the **Starting Label** field.
    
4.  Enter the start date for range of fulfilled sales orders you want to ship, in the **From** field.
    
5.  Enter the end date for range of fulfilled sales orders you want to ship, in the **To** field.
    
6.  Beside the order you want to print a label for, check the **Print** column box.
    
    -   To select all items, click **Mark All**.
        
    -   To print by date, click **Order Date**.
        
    -   To view the order Item Fulfillment, click **Ship Date**.
        
7.  Click **Print**.
    
    A window opens describing how to download your label.
    
8.  Attach the label to the package for the order, and it is ready for drop-off or pick-up.
    

## Printing FedEx Shipping Labels as PDFs {#bridgehead_N1273057}

After you create an integrated shipping item, fulfill the sales order, and check the Integrated Shipping Label box, you can print a FedEx barcode shipping label.

Integrated shipping labels can be printed using the PDF format on 4' x 6' or 8.5" x 11" labels.

To learn how to print **PNG** labels, see [Printing FedEx Shipping Labels in PNG Format](#bridgehead_N1272913).

You select the type of label you want to use at _Setup > Accounting > Shipping_. Click the account you want to edit, and enter your label type choice.

#### To print an integrated shipping label in PDF format: {#procedure_N1273133}

1.  After you fulfill an order, go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **Integrated Shipping Labels**.
    
3.  To begin printing on first label of the first sheet of labels, enter 1 in the **Starting Label** field.
    
    Enter 2 to begin printing on the second half, or second label, on the sheet of labels.
    
4.  To print any of the shipping labels more than one time, check the **Allow Reprinting** box.
    
5.  To print PDF labels, one label per sheet on 8.5" x 11" paper, check the **Single Label Per Page** box.
    
    The Single Label Per Page option enables you to fold 8.5" x 11" paper in half and slide the label into the packaging cover or tape the label to the package.
    
    To use 8.5" x 5.5" labels or to print 2 labels per page, clear this box.
    
6.  To print shipping labels by location, select a **Location**.
    
7.  Enter the **Order Number**.
    
8.  Select a **Ship Date**.
    
9.  To view invoices over a time period, enter the **From** and **To** dates.
    
10.  Beside the order you want to print a label for, check the **Print** column box.
     
     -   To select all items, click **Mark All**.
         
     -   To print by date, click **Order Date**.
         
     -   To view the order Item Fulfillment, click **Ship Date**.
         
     
     The **FedEx Shipping Labels in Queue** field shows the number of labels you have marked for printing.
     
11.  Click **Print**.
     
     A window opens with instructions on how to download your label.
     
12.  Attach the label to the package for the order, and it is ready for drop-off or pick-up.
     

## Printing FedEx Shipping Manifests {#bridgehead_N1273993}

A FedEx Shipping Manifest lists all domestic FedEx ground shipments by day for a shipping location. The FedEx driver signs this document when picking up the packages to ensure that each package is shipped.

#### To print a shipping manifest: {#procedure_N1274014}

1.  Go to _Transactions > Management > Print Checks and Forms_.
    
2.  Click **FedEx Shipping Manifests**.
    
3.  The date range in the **From** and **To** fields defaults to today's date.
    
    You can change this if you are also shipping packages fulfilled previously.
    
4.  To view and print your list of packages in manifest or report format, select a **Manifest Type**.
    
5.  To view and print the shipping manifest including all packages for the date range, slick **Generate Manifest**.
    
    To view and print the manifest as a report, click **Generate Report**.
    

### Related Topics:

-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html)
-   [Fulfilling Orders with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1271195.html)
-   [FedEx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
