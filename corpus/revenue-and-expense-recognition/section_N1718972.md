---
id: "section_N1718972"
type: "section"
title: "Setting Up VSOE on an Item Record"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using the VSOE Feature > Setting Up the VSOE Feature > Setting Up VSOE on an Item Record"
parent: "section_N1718515"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718972.html"
anchors: ["procedure_N1719086"]
sha256: "e034cbf3da88faaabbfa0540b19ca0018060d8ccdc93e54117c1d0c758b3ba4c"
---

You can set up VSOE for the following types of items:

-   Assembly
    
-   Serialized Assembly
    
-   Lot Numbered Assembly
    
-   Kit/Package
    
-   Item Group (Bundle)
    
-   Inventory
    
-   Serialized Inventory
    
-   Lot Numbered Inventory
    
-   Non-Inventory for Sale/Resale
    
-   Other Charge for Sale/Resale
    
-   Service for Sale/Resale
    

Each item can have a revenue recognition template associated with it either on an item record or on a sales transaction. When you associate a revenue recognition template on an item record, that template is selected by default for that item on all transactions. For more information, see [Associating Revenue Recognition Templates with Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1687451.html).

#### To set up VSOE on an individual item record: {#procedure_N1719086}

1.  Go to _Lists > Accounting > Items_, and click **Edit** next to an item.
    
2.  In the Item record, click the **Accounting** subtab, and select an account from the **Deferred Revenue Account** list.
    
    This field must be populated for VSOE to be available for an item on transactions.
    
3.  Click the **Revenue Recognition / Amortization** subtab, and complete the following:
    
    1.  Select a template from the **Revenue Recognition Template** list.
        
        You must select a template for each item you plan to use with VSOE even if all revenue will be recognized immediately upon billing the sale. Only items with a VSOE template assigned can use VSOE revenue recognition.
        
        For more information about revenue templates, read [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html).
        
    2.  In the **VSOE Price** field, enter the VSOE price for this item if it's known.
        
        If you need to use more than one VSOE price for an item, you can set the most common price here and then manually change the price on each transaction as needed. VSOE prices are typically based on the historical sale prices of items or may be set by management.
        
    3.  In the **Deferral** field, choose how to handle deferment when this item is sold as part of a bundle:
        
        -   **Defer Bundle Until Delivered** - Until this item is marked delivered, the revenue recognition of **all** items in the bundle is deferred.
            
            A typical use for this option is to identify items whose revenue recognition depends on the delivery of the item itself, in addition to the delivery of a separate service. For example, a specified upgrade would typically be marked **Defer Bundle Until Delivered.**
            
        -   **Defer Until Item Delivered** - Until this item is marked delivered, the revenue recognition of this item is deferred. This setting is the default for this field.
            
            The deferral setting you choose for each item in a bundle works together with the deferral settings for other items in the bundle.
            
            For example:
            
            -   Member 1 - Defer Bundle Until Delivered: status is undelivered
                
            -   Member 2 - Defer Bundle Until Delivered: status is delivered
                
            -   Member 3 - Defer Until Item Delivered: status is delivered
                
            -   Member 4 - Defer Until Item Delivered: status is delivered
                
            
    4.  In the **Permit Discount** field, choose from the following to determine how discounts are handled for this item.
        
        -   **As Allowed** - Allows a portion of an applicable discount to be applied against this item when the VSOE allocation is performed. How a discount is applied depends on the scenario. For example, no discount is applied to an undelivered item when the residual method is used even if the undelivered item is set to As Allowed. In other cases, all bundle members may receive a portion of a discount, such as when all items have a VSOE price. Then, an explicit discount is applied proportionately to all bundle members. This is the default for this field.
            
        -   **Never** - Doesn't allow a discount to be applied against this item when the VSOE allocation is performed. This selection would be common for a Specified Upgrade.
            
    5.  Check the **Default as Delivered** box to automatically set this item to a Delivered status when this item is added to a transaction. Clear this box to leave the delivery status clear by default.
        
        The default for the **Default as Delivered** box is cleared.
        
        For VSOE, the fulfillment status of an item is separate from its delivery status. An item may be marked **Delivered** although fulfillment hasn't yet occurred.
        
        The VSOE delivery status is used in the following two ways:
        
        -   To determine how the sales amount of the bundle is allocated to individual members based on their VSOE settings.
            
        -   To specify that revenue recognition for the item can begin when the order has been billed.
            
4.  Click **Save**.
    

The item is now set up for VSOE revenue recognition. When the item is sold on a bundled transaction, revenue for the sale is allocated and deferred according to its VSOE settings.

When added to a transaction, the item defaults to use the assigned revenue recognition template. You can change the revenue recognition template on individual transaction lines.

For more information about the function of VSOE settings for items, read [Allocating VSOE Revenue for a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1720414.html).

### Related Topics

-   [Using the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1717900.html)
-   [Enabling the VSOE Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718707.html)
-   [Setting Up VSOE Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1718858.html)
-   [Creating VSOE Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1719451.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
