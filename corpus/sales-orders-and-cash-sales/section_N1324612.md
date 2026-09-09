---
id: "section_N1324612"
type: "section"
title: "Setting Up Maintenance/Support for Contract Renewals"
branch: "sales-orders-and-cash-sales"
category: "order-management"
breadcrumb: "Order Management > Sales Orders and Cash Sales > Software Vertical Contract Renewals > Setting Up Contract Renewals > Setting Up Maintenance/Support for Contract Renewals"
parent: "section_N1320628"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1324612.html"
anchors: ["procedure_N1324680", "procedure_N1324736"]
sha256: "d18ad177fc82818599d356314c6098155126fd3f6ccad130c420eb03ad278420"
---

Before you begin using the Software Vertical Contract Renewals SuiteApp, you should set up your maintenance and support items. Maintenance and support is often abbreviated as M/S on preferences and in other settings.

By default, maintenance and support costs ignore any discounts. If you want to consider customer discounts when calculating the cost of maintenance or support, you can enable the M/S Customer In-Line Discount preference on the Contract Renewals Preferences page. The M/S Customer In-Line Discount preference applies in-line discounts before calculating maintenance and support costs.

First, set your maintenance and support preferences at Contract Renewals > Setup > Contract Renewals Preferences:

-   Default M/S Pricing Option
    
-   Item Categories Skipped on Renewal Calculations
    
-   M/S Customer In-Line Discount
    
-   M/S In-Line Discount
    

For information about these preferences, see [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html).

Next, an administrator can create maintenance and support types to represent the tiers of maintenance and support that you offer.

#### To create a maintenance and support type: {#procedure_N1324680}

1.  Go to Setup > Custom > Maintenance/Support Types > New.
    
2.  Enter a name for the maintenance and support tier.
    
3.  If you calculate maintenance or support as a percentage of license, enter the percentage for this tier.
    
4.  Click **Save**.
    
5.  Repeat these steps for each tier that you offer.
    

Finally, set up your support and maintenance items.

#### To create a maintenance or support item: {#procedure_N1324736}

1.  Go to Lists > Accounting > Items > New.
    
2.  Select the item type for the M/S item that you want to create.
    
3.  On the item form, make sure that the Contract Renewals custom form is selected in the **Custom Form** field. For more information, see [Setting Preferred Forms for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N1321283.html).
    
4.  Enter values in the fields on the Primary Information and Classification sections as you would in a standard item form. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
    
5.  On the Vertical Classification section:
    
    1.  In the **Term/Contract Pricing Type** field, select a pricing type for the item.
        
    2.  In the **Product Line** field, select which product line this item belongs to.
        
    3.  In the **Item Category** field, select the item category where this item should be included in. Choose one of these categories for M/S items:
        
        -   Maintenance - New
            
        -   Maintenance - Renewal
            
        -   Support - New
            
        -   Support - Renewal
            
    4.  In the **Quantity Type** field, select **M/S Entitlement**.
        
    5.  In the **Renew With** field, select an item to replace the current item when it is renewed. If this item renews with itself, you can select this item in this field after you saved the item record.
        
    6.  In the **Maintenance/Support Type** field, select the tier this item belongs to. The **Maintenance/Support %** field shows the percentage of the maintenance or support type that you selected.
        
        If your role grants you permission, click the plus sign icon to create a new maintenance or support tier.
        
6.  In the **M/S Pricing Option** field, select the pricing option that you want to use for this M/S item. By default, this field shows the value that you set in the Default M/S Pricing Option preference. If you set this field to blank, the value in the Default M/S Pricing Option preference will be applied whenever this item is used on contracts.
    
7.  On the **Pricing** subtab, enter the price of this item:
    
    -   If the M/S pricing option is set to either **M/S as a % of License List Price** or **M/S as a % of License Net Price**, enter the base price as 0.00.
        
    -   If the M/S pricing option is set to **Itemized M/S Price**, enter the price of this item.
        
8.  Enter other information related to this item. For information about setting up items for Contract Renewals, see [Setting Up Items for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325048.html).
    
9.  Click **Save**.
    

Note:

If a contract includes a maintenance item and a support item from the same product line, only one of these items will be renewed. The Contract Renewals SuiteApp renews the M/S item with the highest internal ID and with an aggregated quantity greater than zero.

### Related Topics

-   [Software Vertical Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1319596.html)
-   [Contract Renewals Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4442063121.html)
-   [Setting Up Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1320628.html)
-   [Setting Up Contract Renewals Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1321619.html)
-   [Setting Up Items for Contract Renewals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325048.html)
-   [Contract Creation Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1325604.html)
-   [Contract Renewals Process](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1326010.html)
-   [Managing Contracts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4460985489.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
