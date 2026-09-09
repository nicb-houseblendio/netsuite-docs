---
id: "section_N1268691"
type: "section"
title: "Creating Shipping Items with FedEx Integration"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > FedEx > Creating Shipping Items with FedEx Integration"
parent: "section_N1267302"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268691.html"
anchors: ["procedure_N1268778"]
sha256: "069d6bbdd6b1cfaf8fee0e2bd5d9defa89bc3b3be299c14b0b72ea3ed3112f7a"
---

Important:

NetSuite Ship Central is NetSuite's standard shipping solution. For more information, see [NetSuite Ship Central](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_90092747693.html).

The Shipping Integration with FedEx, UPS, and USPS/Endicia is not available to new customers. It is available with limited support only for existing customers before they transition to NetSuite Ship Central.

For more information about transitioning to NetSuite Ship Central, including the self-service procedure, see [Upgrading from Integrated Shipping to NetSuite Ship Central](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1015202/kw/1015202) (SuiteAnswers ID 1015202).

Depending on business requirements, you can use the ShipStation Connector in NetSuite Connector as an alternative. For more information, see [Managing the ShipStation Connector in NetSuite Connector](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163162030389.html).

For more information about selecting the best shipping solution for your needs, see [Comparing NetSuite Shipping Options](https://suiteanswers.custhelp.com/app/answers/detail/a_id/1046701/kw/1046701) (SuiteAnswers ID 1046701).

To use FedEx integration, create shipping items that are marked for integration.

After you create a FedEx integrated shipping item, you can enter sales orders with the integrated shipping item selected in the Ship Via field. When you fulfill an order, your FedEx account is charged with the FedEx shipping method rate.

Before you can create a FedEx-integrated shipping item, you must [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)

#### To create a shipping item with FedEx Integration: {#procedure_N1268778}

1.  Go to _Lists > Accounting > Shipping Items > New_.
    
2.  Enter a shipping item **Ship Name**.
    
3.  Enter the shipping item **Display Name/Code** to appear on invoices, your Web store, and centers such as the Customer Center.
    
    In all other places, the Ship Name is displayed.
    
4.  Enter a shipping item **Description**.
    
5.  To make this shipping item no longer appear on a list, check the **Inactive** box.
    
6.  To make this shipping item available in your website, check the **Display in Web Site** box.
    
7.  On the **Shipping Labels** subtab, check the **Shipping Label Integration** box.
    
    In the list beside the Shipping Label Integration box, select a shipping method.
    
    This selection determines the rate FedEx charges your account and which barcode shipping label will be created.
    
8.  In the **Shipping Rate** subtab, select the **Account** to record income for this shipping item.
    
9.  Select the rate you want to charge:
    
    -   **FedEx Real-Time Rate** - Select which real-time rate to use for this shipping item.
        
        1.  Enter a decimal form discount rate in the **Discount Rate** field.
            
            For example, to offer a 25% discount, enter 0.75.
            
        2.  If this item qualifies, check the **FedEx One Rate** box.
            
            To learn more, see [FedEx One Rate](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4452532276.html).
            
    -   To charge shipping fees by item weight, select **By Weight**.
        
        1.  Enter the amount to charge.
            
        2.  Enter the Increment. For example, 1, 1.5, 2, and so on.
            
        3.  Select the unit of measure: lb, oz, kg, or g.
            
        4.  To not allow partial increments, check the **In Whole Increments** box.
            
    -   To charge a shipping fee for each item, select **By Item** and then enter the **Default Charge** amount for shipping on a per-item basis.
        
        You can enter custom, per-item shipping charges on individual item records.
        
    -   To charge a percentage of the total charge as the shipping fee, select **Percent of Total** and then enter a number in the **%** field.
        
    -   To charge shipping based on a range, select **Shipping Table**.
        
        -   To charge shipping based on ranges of order totals, select **Order Total**.
            
        -   To charge shipping based on ranges of package weight, select **Weight** and then select a unit of measurement.
            
10.  Click **Save**.
     

### Related Topics

-   [FedEx](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1267302.html)
-   [Creating Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html)
-   [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html)
-   [Shipping Integration with Multiple Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1265568.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
