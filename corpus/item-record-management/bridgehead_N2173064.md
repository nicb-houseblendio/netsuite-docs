---
id: "bridgehead_N2173064"
type: "bridgehead"
title: "Revenue Recognition and Amortization Information about Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Using Item Records > Creating Item Records > Revenue Recognition and Amortization Information about Items"
parent: "section_N2166469"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173064.html"
anchors: []
sha256: "a5ebc06885e4e204cde3f7ad2f8f13ceb10cf35e43a7711af051e1a22e8e415d"
---

If you use Advanced Revenue Management, see [Item Configuration for Advanced Revenue Management (Essentials) and (Revenue Allocation)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4340443927.html).

The following fields show if you use the Revenue Recognition feature and other legacy revenue recognition features:

**Revenue Recognition Template** - Select a revenue recognition template to associate with this item by default on sales transactions.

This field appears only on the following items:

-   Assembly
    
-   Download
    
-   Inventory
    
-   Kit/Package
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale or resale
    
-   Service for sale or resale
    

**VSOE Price** - Enter the VSOE price for this item if it is known. To use more than one VSOE price for an item, enter the most common price, and then manually change the price on each order.

**Deferral** - In this field, choose how to handle deferment when this item is sold as part of a bundle:

-   **Defer Bundle Until Delivered** - Until this item is marked delivered, the revenue recognition of all items in the bundle is deferred.
    
    Use this option to identify items whose revenue recognition depends on the delivery of the item, in addition to the delivery of a separate service. For example, a specified upgrade would typically be marked Defer Bundle Until Delivered.
    
-   **Defer Until Item Delivered** - Until this item is marked delivered, the revenue recognition of this item is deferred. This is the default setting for this field.
    

Note:

The deferral setting you choose for each item in a bundle works together with the deferral settings for other items in the bundle.

**Permit Discount** - In this field, choose from the following to determine how discounts are handled for this item.

-   **If Delivered** - A portion of an applicable discount is applied against this item if its status is Delivered when the VSOE allocation is performed.
    
-   **Never** - Doesn't allow a discount to be applied against this item when the VSOE allocation is performed. This selection would be common for a Specified Upgrade.
    

**Default as Delivered** - Check this box to automatically set this item to a Delivered status when this item is added to a transaction. Clear this box to leave the delivery status clear by default.

### Related Topics

-   [Item Record Header Fields](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_161918187368.html)
-   [Entering Purchasing and Inventory Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2167714.html)
-   [Sales and Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2171993.html)
-   [Account Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2172688.html)
-   [Tax and Tariff Information about Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2173187.html)
-   [Entering Preferences on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173412.html)
-   [Copying and Importing Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2173669.html)
-   [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
