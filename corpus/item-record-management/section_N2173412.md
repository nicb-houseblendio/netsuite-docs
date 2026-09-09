---
id: "section_N2173412"
type: "section"
title: "Entering Preferences on Item Records"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Using Item Records > Creating Item Records > Entering Preferences on Item Records"
parent: "section_N2166469"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173412.html"
anchors: []
sha256: "acff20b37ea922522d9e2ec2614c0e49d81111f6c4e47dbc523b715b1feb9ea9"
---

The fields and subtabs that appear depend on the features you have enabled and the type of record you view.

#### To set up your preferred preferences for each item:

1.  Check the **Available to Adv. Partners** to make this item record available in the Advanced Partner Center.
    
2.  Check the **Offer Support** box to offer support for this item.
    
    By offering support for an item, customers can select the item they are having trouble with on case records.
    
    This field appears only on the following items:
    
    -   Assembly/Bill of Materials
        
    -   Inventory
        
    -   Kit/Package
        
    -   Non-inventory for sale or resale
        
    -   Other Charge for sale or resale
        
    -   Service for sale or resale
        
3.  Check the **Can be Fulfilled/Received** box to allow the item to be fulfilled and received during order processing.
    
    Clear this box if you prefer this item doesn't require being received and fulfilled. Even non-inventory items require the customer to enter a shipping address.
    
    Editing the **Can be Fulfilled/Received** box on an item record after creating a source transaction with that item doesn't affect whether that transaction can be fulfilled or received. For information about how this preference works with Advanced Revenue Management, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).
    
    This field appears only on the following items:
    
    -   Inventory
        
    -   Non-inventory for sale or resale
        
    -   Other Charge for sale or resale
        
    -   Service for sale or resale
        
    
    Note:
    
    The **Can Be Fulfilled/Received** box must be checked before you can check the **Generate Accruals** box.
    
4.  Check the **Generate Accruals** box to automatically generate and post an accrual to the general ledger.
    
    When this box is checked, Inventory items, Non-inventory items, Other Charge items, and Service items can generate journal postings based on variances in vendor bills. For more information, see [Vendor Bill Variances](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2371184.html).
    
    The **Generate Accruals** setting can be changed on an item record after transactions have posted with a previous setting. However, past transactions maintain the setting used at the time the transaction was processed.
    

### Related Topics

-   [Item Record Header Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161918187368.html)
-   [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html)
-   [Sales and Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2171993.html)
-   [Account Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2172688.html)
-   [Revenue Recognition and Amortization Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173064.html)
-   [Tax and Tariff Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173187.html)
-   [Copying and Importing Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173669.html)
-   [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
