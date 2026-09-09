---
id: "section_N1259213"
type: "section"
title: "Creating Shipping Items"
branch: "order-fulfillment-and-shipping"
category: "order-management"
breadcrumb: "Order Management > Order Fulfillment and Shipping > Shipping > Setting Up Shipping > Creating Shipping Items"
parent: "section_N1257579"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1259213.html"
anchors: ["procedure_N1259259", "procedure_N1259391", "bridgehead_N1259505", "bridgehead_1543862463", "bridgehead_1543862620", "bridgehead_1543862892", "bridgehead_1543862998", "bridgehead_1543863029", "bridgehead_1543863120", "bridgehead_1543863224", "bridgehead_1543863249", "bridgehead_N1259938", "procedure_N1260235", "procedure_N1260332", "bridgehead_4448295490", "bridgehead_159706810067", "procedure_N1260371"]
sha256: "cf5b9dcf58b3881aaf702a380ec00b4f7a4b0ffd8de1097b041ab994f8280e71"
---

NetSuite enables you to create a shipping item record for each shipping method you want to offer.

-   [Charging for Shipping and Handling per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1260542.html) when you charge for shipping and charge a separate handling fee.
    
    If you do not charge a separate handling fee when you create shipping items, the Handling subtab is not displayed.
    
-   If you use Standard Site Builder without touch points, shipping and handing fees are displayed as a single amount. SCA and Site Builder sites with touch points list the items separately.
    
-   You can create multiple shipping items for a shipping method if you are working in a OneWorld account.
    
    To learn more, see [Associate Subsidiaries With Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N277674.html).
    
-   To make a shipping item inactivate, on the shipping item record check the **Inactive** box.
    
    Inactive shipping items are removed from the shipping items list and are no longer available as shipping methods on your website or on transactions.
    

#### To create a shipping item without charging for shipping: {#procedure_N1259259}

1.  Go to _Lists > Accounting > Shipping Items > New_.
    
2.  Enter a unique and descriptive item **Ship Name**.
    
3.  Enter a **Display Name/Code**.
    
    This item name appears in the Shipping Method or Ship Via field on printed forms, your web store, and all centers, such as the Customer Center. otherwise, the item Ship Name is displayed.
    
    If you are creating a UPS integrated shipping item, you cannot edit or change the display name/code.
    
4.  Enter an item **Description**.
    
5.  If you are using a OneWorld account, select a shipping item **Subsidiary**.
    
    To learn more, see [Associate Subsidiaries With Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N277674.html).
    
6.  To make this shipping item inactive, check the **Inactive** box.
    
7.  To make item available on your website, check the **Display in Web Site** box.
    
8.  If you use Shipping Label Integration but do not automatically charge for shipping, click the **Shipping Labels** subtab.
    
    1.  To charge your FedEx, UPS, or USPS account when sales orders using this shipping item are fulfilled, check the **Shipping Label Integration** box.
        
    2.  Beside the box, select the rate you want use when this shipping item is selected.
        
        This rate is charged to your account. Real-time rates will not be displayed on your web store, and customers will not automatically be charged real-time rates.
        
9.  Click **Save**.
    

#### To create a shipping item and charge for shipping and handling: {#procedure_N1259391}

1.  Go to _Lists > Accounting > Shipping Items > New_.
    
2.  Enter a unique and descriptive item **Ship Name**.
    
3.  To display this shipping item on your website and transactions field, enter a **Display Name/Code**.
    
    This item name appears in the Shipping Method or Ship Via field on printed forms, your web store, and all centers, such as the Customer Center. Otherwise, the item Ship Name is displayed.
    
4.  Enter an item **Description**.
    
5.  If you are using a OneWorld account, select a shipping item **Subsidiary**.
    
    To learn more, see [Associate Subsidiaries With Shipping Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N277674.html).
    
6.  To make this shipping item inactive, check the **Inactive** box.
    
7.  To make this item available on your website, check the **Display in Web Site** box.
    
8.  If you use Shipping Label Integration, click the **Shipping Labels** subtab.
    
    1.  To charge your FedEx, UPS, or USPS account when orders using this shipping item are fulfilled, check the **Shipping Label Integration** box.
        
    2.  Beside the box, select the rate you want use when this shipping item is selected.
        
        The selected method is used to ship an order and charge to your integrated account. You can charge customers based on either the same method or a different method on the **Shipping Rate** subtab.
        
9.  Click **Save**.
    

#### Shipping Rate {#bridgehead_N1259505}

1.  In the Shipping Rate subtab, select the **Account (Shipping)** for this shipping item.
    
2.  Select one of the following shipping methods:
    
    ## FedEx {#bridgehead_1543862463}
    
    1.  If you added your FedEx account to NetSuite, select **FedEx Real-Time Rate**.
        
        To learn more, see [Getting Started with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268430.html).
        
    2.  Select a **FedEx Real-Time Rate**.
        
    3.  Enter a **Discount Rate**.
        
    4.  If this item qualifies, check the **FedEx One Rate** box.
        
    
    ## UPS {#bridgehead_1543862620}
    
    1.  If you added your UPS account to NetSuite, select **UPS Real-Time Rate**.
        
        To learn more, see [UPS](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1274266.html).
        
    2.  Select a **UPS Real-Time Rate**.
        
    3.  Enter a **Discount Rate**.
        
        UPS is populated with the shipping charge when the customer completes the order.
        
    
    ## USPS {#bridgehead_1543862892}
    
    If you added your USPS account to NetSuite, select **USPS Real-Time Rate**.
    
    USPS is populated with the shipping charge when the customer completes the order.
    
    To learn more, see [Register a USPS Account with NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283332.html).
    
    ## Flat Rate {#bridgehead_1543862998}
    
    1.  To charge a single rate for shipping, select **Flat Rate**.
        
    2.  Enter the amount to charge for every item you ship.
        
    
    ## By Weight {#bridgehead_1543863029}
    
    1.  To charge shipping fees by item weight, select **By Weight**.
        
    2.  Enter the amount to charge.
        
    3.  Enter the increment. For example, 1, 1.5, 2, and so on.
        
    4.  Select the unit of measure: lb, oz, kg, or g..
        
    5.  To not allow partial increments, check the **In Whole Increments** box.
        
    
    To enter item default weights, go to _Setup > Accounting > Shipping_.
    
    ## By Item {#bridgehead_1543863120}
    
    1.  To charge a shipping fee for each item, select **By Item**.
        
    2.  Enter the **Default Charge** amount for shipping on a per-item basis.
        
        You can enter custom, per-item shipping charges on individual item records.
        
    
    ## Percent of Total {#bridgehead_1543863224}
    
    1.  To charge a percentage of the total charge as the shipping fee, select **Percent of Total**.
        
    2.  Enter a number in the **%** field.
        
    
    ## Shipping Table {#bridgehead_1543863249}
    
    1.  To charge shipping based on a range, select **Shipping Table**.
        
        -   To charge shipping based on ranges of order totals, select **Order Total**.
            
        -   To charge shipping based on ranges of package weight, select **Weight** and then select a unit of measurement.
            
    2.  To set a **Range Value** of weight or order total, enter the first line as the minimum charge.
        
        The value for the first line must be zero.
        
    3.  The second value is the maximum total or weight for the first line's **Charge**.
        
        For example, in the following chart, orders that total $0 to $9.99 cost $3.00 to ship. Orders totaling $10.00 to $24.99 cost $5.00 to ship.
        
        | Range Value | Charge |
        | --- | --- |
        | 0.00 | 3.00 |
        | 10.00 | 5.00 |
        | 25.00 | 10.00 |
        | 50.00 | 15.00 |
        
    
    **Default Shipping Method** - This shipping method determines the shipping cost if a real-time shipping rate for UPS, FedEx, or USPS integrated shipping items cannot determined.
    
3.  Click **Save**.
    

#### To define a Handling Rate method: {#bridgehead_N1259938}

1.  Select the shipping item handling fee income **Account (Handling)**.
    
2.  Select one of the following fee handling methods:
    
    -   To only charge shipping, select **Handling- No Handling Charge**.
        
    -   To charge for every item you ship, select **Handling-Flat Rate** and then enter a rate.
        
    -   To charge by weight, select **Handling-By Weight**:
        
        1.  Enter the amount to charge.
            
        2.  Enter the increment. For example, 1, 1.5, 2, and so on.
            
        3.  Select the unit of measure: lb, oz, kg, or g.
            
        4.  To not allow partial increments, check the **In Whole Increments** box.
            
        
        To enter item default weights, go to _Setup > Accounting > Shipping_.
        
    -   To charge shipping on an item, select **Handling-Per Item** and then enter the **Default Charge**.
        
        You can enter custom, per-item handling charges on individual item records.
        
    -   To charge a percentage of the total charge as the shipping fee, select **Handling-Percent of Total** and then enter an amount.
        
    -   To charge shipping based on a range, select a **Handling-Table** option;
        
        -   To charge shipping based on ranges of order totals, select **Order Total**.
            
        -   To charge shipping based on ranges of package weight, select **Weight** and then select a unit of measurement.
            
            1.  To set a **Range Value** of weight or order total, enter the first line as the minimum charge.
                
                The value for the first line must be zero.
                
            2.  The second value is the maximum total or weight for the first line's **Charge**.
                
                For example, in the following chart, orders that total $0 to $9.99 cost $3.00 to ship. Orders totaling $10.00 to $24.99 cost $5.00 to ship.
                
        
        To set ranges of weight or order total, enter the first line as the minimum charge. The value for the first line must be zero. The second value is the maximum total or weight for the first line's charge.
        
        For example, in the following chart, orders that total $0 to $10.00 cost $3.00 for handling. Orders totaling $10.01 to $25.00 cost $5.00.
        
        | Range Value | Charge |
        | --- | --- |
        | 0.00 | 3.00 |
        | 10.00 | 5.00 |
        | 25.00 | 10.00 |
        | 50.00 | 15.00 |
        
3.  Click **Save**.
    

#### To define Shipping and Handling rules: {#procedure_N1260235}

1.  To offer free shipping for orders over a specified dollar amount, check the **Free if Total Order is Over** box, and then enter the amount.
    
2.  To charge a minimum shipping amount, check the **Minimum Shipping Amount** box, and then enter the amount.
    
3.  To restrict the amount to charge your customers, check the **Maximum Shipping Amount** box, and then enter that amount.
    
4.  Select the shipping item **Web Site Rules**:
    
    1.  To make this shipping method available online only if the order total amount is over or under a certain amount, check the **Available if Order Total Is** box.
        
        1.  Select **Over** or **Under**.
            
        2.  Enter the amount.
            
    2.  To make this shipping method available online only if the order weight is over or under a certain amount, check the **Available if Order Weight is** box.
        
        1.  Select **Over** or **Under**.
            
        2.  Enter the weight.
            
        3.  Enter the unit of measure.
            
    3.  To restrict the shipping item availability to a specific web site, select a site or sites in the **Limit to Sites** field.
        
        If this field is empty, the shipping item is available on all web sites. You can select sites in this field and then to specify the sites where the shipping item will not be available, check the **Exclude** box.
        
5.  Specify shipping restrictions in the **Shipping Restrictions** section:
    
    1.  Select the countries you ship to in the **Countries** field.
        
        If you do not select any countries, then this shipping item is available to ship to all countries. To identify countries you do not ship to using this shipping item, select a country or countries and then check the **Exclude** box.
        
    2.  To restrict the states you ship to, select one or more states in the **States** field.
        
        If you do not select any states, the shipping item can ship to all states. To restrict shipping to specific states, select the country in the **Countries** field and do not check the **Exclude** box.
        
        Note:
        
        Some states may not be available in the system. To add a state within a country, go to _Setup > Company > States/Provinces/Counties > New_
        
6.  If this shipping item is taxable, select a **Charge Tax on this Shipping Portion of Item**.
    
7.  If this shipping item is taxable, select a **Charge Tax on this Handling Portion of Item**.
    
8.  Click **Save**.
    

#### To designate Free Shipping Items: {#procedure_N1260332}

1.  To offer free shipping on an order when certain items are purchased, click the **Free Shipping Items** subtab.
    
2.  To require that every item you select be on an order before free shipping is offered, check the **All items must be purchased** box.
    
    Otherwise, any item on an order qualifies the order for free shipping.
    
3.  To add several items at the same time, select each item that qualifies an order for free shipping, and then click **Add Multiple**.
    
4.  Click **Save**.
    

## Packaging {#bridgehead_4448295490}

When you fulfill a sales order, the system automatically generates the number of packages required for your order. However, there is a limit of 50 packages per order. If you fulfill an order that exceeds this amount, the order will not save and the system will display an error.

In the **Packaging** subtab, to disable the automatic packaging logic that occurs during item fulfilment and creates only one package for the order, check the **Omit Packaging** box.

Note:

Omit packaging is not available for all integrated shipping carriers (FedEx, UPS, and UPS) and web store orders.

## Cross-Subsidiary Rules {#bridgehead_159706810067}

When you enable the Intercompany Cross-Subsidiary Fulfillment feature in NetSuite OneWorld accounts, shipping item records display a Cross-Subsidiary Rules subtab.

This subtab enables you to define rules for shipping items that are fulfilled between subsidiaries.

#### To define cross-subsidiary fulfillment rules:

1.  Select a **Subsidiary**.
    
2.  To define the method to use when fulfilling items from a subsidiary, select a **Shipping Item**.
    
3.  Click **OK**.
    
4.  To define shipping items for additional subsidiaries, click **Add Row**.
    
5.  Click **Save**.
    
    To learn more, see [Intercompany Cross-Subsidiary Fulfillment](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1515621767.html).
    

#### To complete the translation subtab: {#procedure_N1260371}

1.  If you use the Multi-Language feature, in the Translation subtab enter the translated text for specific shipping item fields.
    
2.  Click **Save**.
    

### Related Topics

-   [Charging for Shipping and Handling per Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1260542.html)
-   [Free Shipping With an Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1262298.html)
-   [Creating Shipping Items with FedEx Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268691.html)
-   [FedEx Real-Time Rates (U.S. and Canada)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1268998.html)
-   [Creating Shipping Items with UPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278291.html)
-   [UPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1278765.html)
-   [USPS Integration](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1283711.html)
-   [USPS Real-Time Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1284088.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
