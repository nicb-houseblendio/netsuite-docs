---
id: "section_N1265431"
type: "section"
title: "Shipping Integration with Pick, Pack, and Ship"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Shipping Integration with FedEx, UPS, and USPS/Endicia > Shipping Integration with Pick, Pack, and Ship"
parent: "section_N1263996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265431.html"
anchors: ["procedure_N1265455"]
sha256: "429fef1ce4335a9994c51c2634b0d89801e636caeaea7d52d113e3ff179cf6fe"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

If you use both the Shipping Label Integration and the Pick, Pack, and Ship features, you can choose where in the process you want to receive your tracking number and charge your account.

#### To select the stage of pick, pack, and ship for shipping integration: {#procedure_N1265455}

1.  Go to _Setup > Accounting > Shipping_.
    
2.  In the **Default Item Fulfillment Integration Stage** field, select one of the following:
    
    -   When the order is marked **Picked**, your shipping account is charged, a tracking number is received, and a shipping label is created.
        
    -   When the order is marked **Packed**, and ready to be shipped your shipping account is charged, a tracking number is received, and a shipping label is created.
        
        To mark orders packed, go to _Transactions > Sales > Mark Orders Packed_.
        
    -   When the order is marked **Shipped** shipped to the customer and completely fulfilled, your shipping account is charged, a tracking number is received, and shipping label is created.
        
        To mark orders shipped, go to _Transactions > Sales > Mark Orders Shipped_.
        
3.  Click **Save**.
    

Your account will now communicate with your shipping carrier at the time you designated to retrieve the shipping label and tracking information.

### Related Topics

-   [Shipping Integration with FedEx, UPS, and USPS/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html)
-   [Tracking Numbers with Shipping Label Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265305.html)
-   [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html)
-   [Shipping Integration and Third Party Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265784.html)
-   [Integrating with Multiple Shipping Carriers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html)
-   [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
