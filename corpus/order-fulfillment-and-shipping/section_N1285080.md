---
id: "section_N1285080"
type: "section"
title: "Printing USPS Shipping Labels and Forms"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > U.S. Postal Service/Endicia > Printing USPS Shipping Labels and Forms"
parent: "section_N1283121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html"
anchors: ["bridgehead_N1285147", "procedure_N1285186", "bridgehead_N1285339", "bridgehead_N1285384", "procedure_N1285411"]
sha256: "bff854feb6fd3cfa555178676c0fa6ceffc72043e2e90efc958db6e3e50d218a"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

If you use the Shipping Label Integration feature, you can print a barcode shipping label after you have created a sales order that includes an integrated shipping item, and fulfilled that sales order with the box checked to generate a shipping label.

Note:

If you use the Shipping Label Integration feature and an integrated shipping carrier, you cannot use override addresses to generate shipping labels. On the Address window, enter the complete shipping information in the address fields.

You can print the following labels and forms for UPS shipping items:

-   [Printing USPS Shipping Labels](#bridgehead_N1285147)
    
-   [Printing USPS SCAN Forms](#bridgehead_N1285384)
    

Note:

If you use a thermal printer for shipping labels, you must install the thermal printer driver. For more information, see [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).

## Printing USPS Shipping Labels {#bridgehead_N1285147}

If you enable the Shipping Label Integration feature, you can print a U.S. Postal Service (USPS) bar code shipping label. To be able to print a label, you must create an integrated shipping item, create a sales order using an integrated shipping item, and fulfill the sales order with the Integrated Shipping Label box checked.

Note:

The shipping rate is not included on the shipping label.

Integrated shipping labels should be printed on 8.5" x 5.5" labels when you are printing using PDF format. However, you can also use a 8.5" x 11" piece of paper and fold the sheet of paper in half.

You also have the option to print domestic labels in EPL format using an Eltron thermal printer. The EPL label type can only be 4' x 6' thermal label without doc tabs. For more information about setting up this process, see [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).

Select the type of label you want to use at _Setup > Accounting > Shipping_. Click the account you want to edit, select your label type choice in the USPS Label field, and click Submit.

#### To print an integrated USPS shipping label in PNG format: {#procedure_N1285186}

1.  After you fulfill the order, go to _Receiving > Receiving > Print Checks and Forms_.
    
2.  Click **Integrated Shipping Labels**.
    
3.  In the **Starting Label** field, do one of the following:
    
    -   Enter **1** to begin printing on the first label of the first sheet of labels.
        
    -   Enter **2** to begin printing on the second half, or second label, on the sheet of labels.
        
4.  The USPS Shipping Labels in Queue field shows the number of labels you have marked for printing.
    
5.  Check the **Allow Reprinting** box to print any of your shipping labels more than one time.
    
    Important:
    
    When you create a pre-paid USPS label, its value is deducted from your Endicia account balance. Each label may be used to ship only one package, regardless of how many times you reprint it. Reusing the same label on more than one package may be considered mail fraud.
    
6.  The Ship Date field, controls the list of labels displayed on the page. The Ship date refers to the date the fulfillment was entered.
    
7.  In the **Print** column, check the box next to each order you want to print a label for:
    
    -   Click **Mark All** to check the boxes for all items.
        
    -   Click the **Order Date** for an order to view the sales order.
        
    -   Click the **Ship Date** to view the Item Fulfillment for that order.
        
8.  Click **Print**.
    
    A window opens with instructions on how to download your label.
    
9.  Attach the label to the package for the order, and it is ready for drop-off or pick-up.
    

Note:

Labels from a third party (integrated shipping labels), cannot be amended after generated. If you need to amend the label, you will first need to delete the item fulfillment to void the shipment. Then, create a new item fulfillment to generate a new integrated label.

## USPS Customs Documentation {#bridgehead_N1285339}

When you print a shipping label for an international shipment, up to four copies of the shipping label will be printed:

| **Australia, Canada, and Costa Rica** | 
-   One copy for Customs Declaration
-   One Sender's Copy

 |
| --- | --- |
| **Rest of World** | 

-   Two copies for Customs Declaration
-   One Dispatch Note
-   One Sender's Copy

 |

## Printing USPS SCAN Forms {#bridgehead_N1285384}

When you use U.S. Postal Service (USPS) processing to ship packages in your NetSuite account, you can choose to use a Shipment Confirmation Acceptance Notice (SCAN) form to process packages. The SCAN form is a shipping manifest that helps streamline your shipping process by getting information to the USPS driver quickly.

The SCAN Form has a primary barcode that represents all the packages in a shipment. When the Postal Service representative scans this form, all of the associated packages are entered into the USPS database as 'Shipment Accepted.'

You and the recipient can use the Track & Confirm tool at usps.com to confirm the date the package was shipped and track its progress.

Important:

After you generate a SCAN form, you cannot void any of the packages that appear on the manifest. The SCAN form closes out all the packages that are included in the manifest.

#### To generate a SCAN form: {#procedure_N1285411}

1.  Go to _Receiving > Receiving > Print Checks and Forms_.
    
2.  Click **USPS SCAN** Forms.
    
3.  All existing SCAN Forms display in the list with information in the columns as described below:
    
    **Manifest Date** - the Date the SCAN Form was generated.
    
    **Manifest Time** - the Time the SCAN Form was generated.
    
    **Manifest file** - URL to display the SCAN Form.
    
4.  Click **Generate SCAN Form**.
    

You can use the Date filters at the bottom of the page to filter the list of existing SCAN Forms, so you can find what you need to print. Click Refresh to re load the page with the date filter applied.

### Related topics

-   [Printing USPS Shipping Labels](#bridgehead_N1285147)
-   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
