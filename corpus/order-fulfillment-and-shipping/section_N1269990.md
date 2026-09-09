---
id: "section_N1269990"
type: "section"
title: "Shipping Dangerous Goods and Hazardous Materials"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > Shipping Dangerous Goods and Hazardous Materials"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1269990.html"
anchors: ["procedure_N1270082", "procedure_N1270193", "procedure_N1270287"]
sha256: "b3e0005f4067a3d5b3689b11b6699c5310058a3189f36668d1005f112a8f6d9a"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

FedEx integration supports Dangerous Goods and Hazardous Material shipments. To learn about shipping these types of materials, see the [FedEx Service Guide](http://www.fedex.com/us/service-guide/).

-   Only ship dangerous goods using FedEx Express shipping. Special packaging and documentation are required. You cannot use FedEx packaging.
    
-   Hazardous materials can be sent using FedEx Ground within the contiguous United States only. Some ORM-D designated materials can be shipped into Canada.
    
    Hazardous materials must be shipped in a single package. Non-hazardous materials cannot be shipped in the same package. A FedEx Account Executive must qualify you to ship hazardous materials. To learn more, contact FedEx Ground Customer Service.
    

In NetSuite, refer to the following topics to learn how to ship dangerous goods and hazardous materials:

-   [To set up shipping for dangerous goods and hazardous materials:](#procedure_N1270082)
    
-   [To set up items for dangerous goods and hazardous materials:](#procedure_N1270193)
    
-   [To ship hazardous materials and dangerous goods:](#procedure_N1270287)
    

#### To set up shipping for dangerous goods and hazardous materials: {#procedure_N1270082}

1.  Go to _Setup > Accounting > Shipping_.
    
2.  On the **Preferences** subtab, **Carrier Basics** section, check the **Hazmat/Dangerous Goods Shipping** box.
    
    This makes the **HazMat/Dangerous Goods** subtab available on the Item and Item Fulfillment records.
    
    Note:
    
    In your NetSuite account. use **Pick, Pack and Ship** to enable shipping for hazardous materials and dangerous goods.
    
    To learn more, see [Setting Up Pick, Pack, and Ship](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1230197.html).
    
3.  On the **Carrier Registration** subtab, click your FedEx account link.
    
4.  Add your emergency contact information to your FedEx registration:
    
    To learn more, see [Registering a FedEx Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html#bridgehead_N1267326).
    
    1.  **Dangerous Goods Contact** - enter the name of the person responsible for the dangerous goods shipment
        
    2.  **Dangerous Goods Contact Title** - enter the title of your dangerous goods contact
        
    3.  **Dangerous Goods Contact Place** - enter the location of your dangerous goods contact
        
    4.  **Dangerous Goods Contact Phone** - enter the phone number to use for the contact in the event of an emergency
        
    5.  **Dangerous Goods Offeror** - according to per DOT regulations, enter the offeror's name or contract number
        
    6.  **Infectious Substance Contact** - enter the name of the person who handles infectious substances in the dangerous goods shipment
        
    7.  **Infectious Substance Contact Phone** - enter the phone number for your infectious substance contact
        
    8.  **Regulation** - the type of documentation FedEx expects to accompany the specific hazmat item shipment.
        
    9.  **Option Type** - the hazardous material you are shipping.
        
5.  Click **Submit**.
    

#### To set up items for dangerous goods and hazardous materials: {#procedure_N1270193}

1.  Go to _Lists > Accounting > Items._.
    
2.  Beside the item you want to setup, click **Edit**.
    
3.  On the **HazMat/Dangerous Goods** subtab, check the **Hazmat/Dangerous Goods** box.
    
    This box is available only on inventory items and inventory assembly items. All Hazmat/Dangerous Goods items must be shipped separately.
    
4.  From the **Federal Express Ground Hazardous Materials Shipping Guide**, enter the commodity **ID** (regulatory identifier).
    
    The format is UNXXXX where XXXX is a four digit number.
    
5.  From the **Federal Express Ground Hazardous Materials Shipping Guide**, enter the ID **Hazmat Shipping Name**.
    
    This item appears on the OP950 form.
    
6.  Enter the DOT **Hazmat Hazard Class**.
    
7.  Based on the degree of danger the item presents, select the item **Hazmat Packing Group**.
    
8.  Enter the **HazMat Item Units** (unit of measure). For example, kg or ml.
    
9.  Enter **HazMat Item Units Quantity**.
    
10.  Enter the proper **Technical Name** for the dangerous goods or hazardous materials.
     
11.  Click **Save**.
     

#### To ship hazardous materials and dangerous goods: {#procedure_N1270287}

1.  **Prerequisite:** On the shipping item, check the **HazMat/Dangerous Goods** box.
    
    You must pick, pack, and ship dangerous goods or hazardous materials goods separately from all other items that you ship.
    
2.  Go to _Lists > Accounting > Items._.
    
3.  Beside the item you want to setup, click **Edit**.
    
4.  On the **HazMat/Dangerous Goods** subtab, check the **Hazmat/Dangerous Goods** box.
    
5.  Complete the **Carrier** subtab.
    
    To learn more, see the Carrier subtab section of [Fulfilling Orders with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1271195.html).
    
6.  On the **HazMat** subtab:
    
    -   Select a HazMat **Type**
        
    -   Select an **Accessibility** option
        
    -   If item must be shipped by cargo aircraft, check the **Cargo Aircraft Only** box
        
7.  Print the shipping documentation. For example Shipper's Declaration of Dangerous Goods, OP-900 Shipping Paper, or the OP-950 certification form.
    

### Related Topics:

-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [Creating Shipping Items with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268691.html)
-   [Fulfilling Orders with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1271195.html)
-   [Printing FedEx Shipping Labels and Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1272548.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
