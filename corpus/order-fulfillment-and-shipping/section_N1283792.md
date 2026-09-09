---
id: "section_N1283792"
type: "section"
title: "Creating Shipping Items with USPS Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > U.S. Postal Service/Endicia > Creating Shipping Items with USPS Integration"
parent: "section_N1283121"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283792.html"
anchors: ["procedure_N1283828"]
sha256: "1607375bb1c2af9edcf7978574e4f8ba2825628f5fb847b8aed97440622f9d7c"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

Using shipping items that are integrated with the U.S. Postal Service (USPS), enables you to enter sales orders that select the integrated shipping item in the Ship Via field. When you fulfill an order, your Endicia account is charged the rate for the USPS shipping method.

The real-time rate quoted at the time of sale is only an estimate. The charge may vary based on factors such as package size, service additions on the shipment, and account-specific discounts.

To learn more, see [USPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html).

#### To create a shipping item with USPS integration: {#procedure_N1283828}

1.  Go to _Lists > Accounting > Shipping Items_ > New.
    
2.  Check the **Shipping Label Integration** box.
    
    If this is an integrated shipping item, your Endicia account is charged for the selected shipping method. Shipping Rate represent the amount your customer will be charged.
    
    To charge the customer the same amount you are charged, in the **USPS Real-Time Rate** field, select the same method as you selected in the **Shipping Label Integration** field.
    
3.  Check the **Display in Web Site** box to make this shipping item available in your Web site.
    
4.  Click the **Shipping Rate** subtab.
    
5.  Select the rate you want to charge your customer:
    
    -   **USPS Real-Time Rate** - Select which real-time option you want to use for this shipping item. Set this option for USPS integrated shipping items.
        
        USPS fills in the shipping charge when the customer completes the order. This rate is an estimate, and may change slightly when the order is fulfilled
        
        For information about offering a discount rate, see [Applying Discounts to USPS Shipping Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284917.html).
        
    -   **Flat Rate** - Enter the amount to charge for each order you ship
        
    -   **By Weight**:
        
        -   Enter the amount to charge and the unit of measure
            
        -   Enter the increment. For example, 1, 1.5, 2, and so on
            
        -   Select the unit of measure: lb, oz, kg, or g
            
        -   To not allow partial increments, check the **In Whole Increments** box
            
    -   **By Item** - Enter the default amount to charge for shipping on a per-item basis
        
    -   **Percent of Total** - Enter a percent in the % field
        
    -   To charge shipping based on a range, select **Shipping Table**
        
        -   To charge shipping based on ranges of order totals, select **Order Total**
            
        -   To charge shipping based on ranges of package weight, select **Weight** and then select a unit of measurement
            
            To learn more, see [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html).
            
6.  Click **Save**.
    

### Related Topics

-   [U.S. Postal Service/Endicia](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283121.html)
-   [Create an Endicia (USPS) Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283210.html)
-   [Register a USPS Account with NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283332.html)
-   [Setting Up Shipping](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1257579.html)
-   [USPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
