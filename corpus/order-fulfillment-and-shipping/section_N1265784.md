---
id: "section_N1265784"
type: "section"
title: "Shipping Integration and Third Party Billing"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Shipping Integration with FedEx, UPS, and USPS/Endicia > Shipping Integration and Third Party Billing"
parent: "section_N1263996"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265784.html"
anchors: []
sha256: "436d652b34ca5e122807f74822e96bb7235045331065ba74bed3ffcee047b40f"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

You can bill third party FedEx, UPS, or USPS accounts for orders. You may need FedEx, UPS, or USPS to bill recipient accounts directly, or bill the distributor for shipping.

#### To enable third party billing:

1.  Go to _Setup > Accounting > Shipping_.
    
2.  Check the **Preferences** subtab.
    
3.  In the **Third Party Billing** section, check the **Third Party Billing** box.
    
4.  Optionally, decide whether to charge for shipping or handling on the order when a third party is being billed:
    
    1.  Check the **Do Not Charge Shipping on Third Party Billing Orders** box.
        
    2.  Check the **Do Not Charge Handling on Third Party Billing Orders** box.
        
5.  Click **Save**.
    

#### To enter third party billing in the company information:

1.  Go to _Setup > Company > Company Information_.
    
2.  Enter your company default third party account information.
    
    You can use this as the production account for all locations.
    
    When you select Third Party Billing or Bill Third Party on item fulfillments, this account is billed by default. You can override this default account number on item fulfillments.
    
3.  Click **Save**.
    

To learn more, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).

#### To enter third party billing in the customer form:

1.  Go to _Lists > Relationships > Customers_.
    
2.  Beside the customer you want to update, click **Edit**.
    
3.  In the **Financial** subtab, enter third party billing information.
    
    Use this information about item fulfillments when you select Third Party Billing or Consignee Billing. You can override the default on item fulfillment account number.
    
4.  Click **Save**.
    

To learn more, see [Entering Financial Information for the Customer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1078064.html).

### Related Topics:

-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [Shipping Integration with FedEx, UPS, and USPS/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263996.html)
-   [Tracking Numbers with Shipping Label Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265305.html)
-   [Shipping Integration with Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265431.html)
-   [Integrating with Multiple Shipping Carriers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265937.html)
-   [Printing Integrated Shipping Labels With a Thermal Printer](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1266244.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
