---
id: "bridgehead_N2172023"
type: "bridgehead"
title: "Sales Information for Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Using Item Records > Creating Item Records > Sales and Shipping Information for Items > Sales Information for Items"
parent: "section_N2171993"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2172023.html"
anchors: []
sha256: "5bc8a7c5fbba14f104263b7c8e0c66cdb8507fde52fa221b0ddc5e64651425c6"
---

**Sales Description** - Enter a sales description using up to 999 characters of letters, numbers or basic HTML code. When your customers click an item's store display name for more information, they see this description.

This field appears only on the following items:

-   Download
    
-   Gift Certificate
    
-   Inventory
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale or resale
    
-   Service for sale or resale
    

**Cost Estimate Type** - The Cost Estimate Type determines what value NetSuite uses to calculate estimated Gross Profit. The estimated Gross Profit for Items on a transaction provides the data needed to calculate the total estimated Gross Profit on that transaction. The individual line items that you enter in a transaction determine the amounts that post in NetSuite when you process that transaction. The following Cost Estimate Types on Items are available:

-   **Item Defined Cost** - a user-defined amount, entered into the Item Defined Cost field on the Item definition page.
    
-   **Average Cost** - NetSuite calculates an average cost of the units purchased. With Multi-Location Inventory enabled, NetSuite calculates the average across all locations. Otherwise, the average calculation uses location-specific costs.
    
-   **Last Purchase Price** - This field displays the most recent purchase price of the item as determined by purchase order receipt transactions. Multiple purchases on the same day using different rates display the highest purchase price on that day, per location, if applicable, in this field. When you use the Multiple-Location Inventory feature, the last purchase price reflects the most recent receipt at any location. If you track inventory costs, NetSuite identifies the cost of the item based on your inventory costing settings.
    
    Note:
    
    Gross Profit transactions apply the last purchase price including landed cost when the Include Landed Cost in Last Purchase Price preference is enabled.
    
-   **Purchase Price** - Enter the price that you pay for this item. If you don't enter a price, then the most recent purchase price from purchase orders provides the price for this item by default.
    
-   **Preferred Vendor Rate** - This option is meaningful only if the Multi-Vendor feature is enabled and multiple vendors supply the same item. In order of precedence:
    
    -   Preferred vendor rate, if defined on the Item record
        
    -   Purchase price
        
    -   Purchase Order Rate - Initially uses the Preferred Vendor Rate cost, Then, after a purchase order is entered, this type uses the most recent purchase order rate. Special orders and drop-shipped items use this cost information.
        
-   **Derived from Member Items** - Total costs of items currently included in a kit. This type applies to kits, and sums the estimated costs of each item in the kit, based on each of their individual Cost Estimate Types. Uses the latest definition of the kit, not its historical definition.
    

**Item Defined Cost** - A user-defined amount, entered into the Item Defined Cost field on the Item definition page.

**Billing Schedule** - Choose the billing schedule you want to associate with this item. When you associate an item with a billing schedule, that schedule appears by default when you add the item to an order.

To create a new billing schedule, go to _Lists > Accounting > Billing Schedules_. Click New to enter a new billing schedule. Forms must be customized to show schedules on lines. See [Applying Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253848.html).

**Days Before Expiration** - To set this item to expire, enter the number of days it should remain active after purchase. If this item is and the same customer purchases this item more than one time, the countdown to expiration restarts with each purchase. This field appears only on Download and Gift Certificate items.

Note:

If a gift certificate buyer lives in California, Connecticut, Louisiana, Massachusetts, New Hampshire, Rhode Island or Washington, by law the gift certificate cannot expire.

**Number of Allowed Downloads** - Enter the maximum number of times a customer who has purchased this item can download it from the Customer Center. If a customer purchases this item more than one time, note the following. The number of available downloads is multiplied by the number of times the item has been purchased. This field appears only on Download items.

**Immediate Download** - Check this box if you want customers to be able to download the item immediately after checking out. Clear this box to make download available after the order is billed. Customers then receive email that the download is available through the My Account tab of your site.

This field shows only on Download items.

**Soft Descriptor** - Select the brand name or name that should appear on customers' credit card statements when this item is purchased. Enter soft descriptors to select in this field at Setup > Accounting > Payment Processing > Credit Card Soft Descriptors.

**Minimum Quantity** - Enter the lowest amount of this item that you want customers can purchase in the Web store. When a customer adds this item to the shopping cart, the quantity defaults to this minimum amount. If the customer lowers this amount, a warning is displayed, and the customer is not able to check out. Leave this field empty to allow customers to check out with no minimum quantity restrictions.

This field appears only on the following items:

-   Assembly
    
-   Inventory
    
-   Kit/Package
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale
    
-   Service for sale
    

Note:

You can also require a minimum return quantity on return authorizations. See [Preferences for Customer Returns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1305008.html) for more information.

**Enforce Internally** - Check this box to apply the minimum quantity to sales orders placed internally in addition to those placed in the Web store. When you add the item to an order, the quantity defaults to the minimum. If the quantity is edited to below the minimum, the item cannot be added to the order.

This field appears only on the following items:

-   Assembly
    
-   Inventory
    
-   Kit/Package
    
-   Non-inventory for sale or resale
    
-   Other Charge for sale
    
-   Service for sale
    

Note:

You must indicate a minimum quantity to check this box.

### Related Topics

-   [Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2172307.html)
-   [Sales and Shipping Information for Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2171993.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
