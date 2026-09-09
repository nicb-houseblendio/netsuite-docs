---
id: "section_N1265937"
type: "section"
title: "Integrating with Multiple Shipping Carriers"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Shipping Integration with FedEx, UPS, and USPS/Endicia > Integrating with Multiple Shipping Carriers"
parent: "section_N1263996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html"
anchors: ["bridgehead_N1265950", "bridgehead_N1265983", "procedure_N1266004"]
sha256: "9d678c47713cc8c18d93f3d70e5b9ac3854be1e38a3ccc036b59ecda95ff17c3"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

NetSuite enables you to integrate with each carrier you use to track shipments and print labels.

## Selecting a Default Shipping Carrier {#bridgehead_N1265950}

When you set up shipping, you also select a default shipping carrier. You can display any of the following based on the shipping accounts you set up: More, FedEx, FedEx/More, FedEx/USPS, FedEx/USPS/More, USPS/More, USPS.

For example, if you set up a FedEx account only and do not define any NetSuite shipping items, then you can select either UPS or FedEx as the default shipping carrier. If you set up accounts with UPS, FedEx, USPS, and set up NetSuite shipping items, you can then select either UPS or FedEx/USPS/More as the default shipping carrier. If you do not integrate with any shipping carriers, your choices are UPS or More.

The Default Shipping Carrier preference in NetSuite does not restrict you to using only one carrier. You can always change the carrier. When you create a sales order or other transaction, the carrier name is automatically displayed. If you use multiple carriers, select the shipping option that you use most frequently for the Default Shipping Carrier so you do not have to change the carrier as often when entering transactions.

To learn more, see [Setting Shipping Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html#bridgehead_N1257598).

## Printing Shipping Labels for Multiple Carriers {#bridgehead_N1265983}

If you integrate with multiple carriers, set up printers to print labels for each carrier because each carrier requires different drivers to print labels. Otherwise, you have to reinstall the carrier-specific driver every time you want print different labels.

#### To print labels for multiple shipping carriers: {#procedure_N1266004}

1.  Set up a separate printer for each shipping carrier you use.
    
2.  Install the carrier-specific driver for each printer.
    
    To learn more, See [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html).
    
3.  Load labels and printing supplies.
    
4.  Fulfill a sales order.
    
    The sales order must use an integrated shipping item as the shipping method or Ship Via.
    
5.  Check the **Shipping Label Integration** box.
    
6.  Go to _Transactions > Management > Print Checks and Forms_.
    
7.  Print labels using one of the following procedures:
    
    -   [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html)
        
    -   [Printing FedEx Shipping Labels in PNG Format](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html#bridgehead_N1272913)
        
    -   [Printing UPS Shipping Labels as PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1282339.html#bridgehead_N1282454)
        
    -   [Printing USPS Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1285080.html)
        

### Related Topics

-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html)
-   [Shipping Integration with FedEx, UPS, and USPS/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html)
-   [Printing FedEx Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
