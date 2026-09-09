---
id: "section_N1278291"
type: "section"
title: "Creating Shipping Items with UPS Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > UPS > Creating Shipping Items with UPS Integration"
parent: "section_N1274266"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html"
anchors: ["procedure_N1278370"]
sha256: "499d35a6fe0f2da6b9b5e36a1e54002d7640c889ca4fdb5a343f5ff89a3576ef"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

To use UPS integration, create shipping items that are marked for integration.

Before you can create a UPS-integrated shipping item, complete the following:

1.  Enable the Shipping Label Integration feature:
    
    1.  Go to _Setup > Company > Enable Features_.
        
    2.  Click the **Transactions** subtab.
        
    3.  In the **Shipping & Receiving** section, check the **Shipping Label Integration** box.
        
    4.  Click **Save**.
        
2.  Add your UPS Account.
    
    To learn more, see [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274).
    

#### To create a shipping item with UPS Integration: {#procedure_N1278370}

1.  Go to _Lists > Accounting > Shipping Items_.
    
2.  Click **New**.
    
3.  Enter a shipping item **Ship Name**.
    
    To learn more, see [Edit a UPS Shipping Item Name](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4448295616.html).
    
4.  Enter the **Display Name/Code** to display on the printed invoices.
    
5.  Enter a shipping item **Description**.
    
6.  To hide this item from appearing on lists, click **Inactive**.
    
7.  To make this shipping item available in your website, check the **Display in Web Site** box.
    
8.  Check the **Shipping Rate** subtab.
    
9.  To record charges for this shipping item, select an income **Account**.
    
10.  Select the rate to charge your customer:
     
     -   **UPS Real-Time Rate**. To learn more, see [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html).
         
         1.  Select a UPS Real-Time Rate option.
             
         2.  Enter a number to multiply the rate by to receive the correct **Discount Rate**.
             
         
         To learn more, see [Applying Discounts to USPS Shipping Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284917.html).
         
     -   **Flat Rate** - Enter the rate to charge for shipping for all orders
         
     -   **By Weight**:
         
         1.  Enter the amount to charge and the unit of measure
             
         2.  Enter the increment. For example, 1, 1.5, 2, and so on.
             
         3.  Select the unit of measure: lb, oz, kg, or g
             
         4.  To not allow partial increments, check the **In Whole Increments** box.
             
         
         To learn more, see [Setting a Default Shipping Method Per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1263649.html).
         
     -   **By Item** - Charge based on the shipping item record cost
         
         Enter a **Default Charge** for items that do not have a shipping cost
         
     -   **Percent of total** - Enter a percent of the order total
         
     -   **Shipping Table** - Charge based on a range of **Order Totals** or **Weights**.
         
         This option enables you to enter the value (0) and charge of your first range in the list. The charge of the first line applies up to the value of the second line, and so on
         
     
     Note:
     
     If this is an integrated shipping item, UPS charges for the shipping method selected beside the Shipping Label Integration box.
     
11.  If you use shipping label integration, click the **Shipping Labels** subtab:
     
     -   To generate and print UPS shipping labels, check the **Shipping Label Integration** box
         
     -   To generate return labels for UPS shipments, check the **Return Label Integration** box
         
         Select the UPS shipping method you want to use for return shipping labels.
         
12.  Define **Handling Rate**, **Shipping and Handling Rules**, **Free Shipping Items**, and **Packaging** information for this shipping item.
     
     To learn more, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
     
13.  Click **Save**.
     

Note:

UPS only accepts packages up to 150 pounds. Packages over 150 pounds are broken into multiple shipments for calculating UPS Real-Time rate charges. For example, a shipment of 400 pounds is charged as two 150-pound shipments and one 100-pound shipment.

To learn more, see [UPS Weight and Size](http://www.ups.com/content/us/en/resources/ship/packaging/weight_size.html).

When using the UPS Developer Kit, NetSuite displays the UPS Trademark and accompanying disclaimer\* on each shipping screen and shipment notification viewed by your customer. These elements are permanent and cannot be deleted or altered.

\* UPS, UPS & Shield Design, and UNITED PARCEL SERVICE are registered trademarks of United Parcel Service of America, Inc.

### Related Topics

-   [Registering a UPS Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html#bridgehead_N1274274)
-   [UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278000.html)
-   [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
