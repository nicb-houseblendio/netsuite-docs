---
id: "section_N2214525"
type: "section"
title: "Serial and Lot Inventory with Multiple Units of Measure"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Multiple Units of Measure > Serial and Lot Inventory with Multiple Units of Measure"
parent: "chapter_N2211898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2214525.html"
anchors: []
sha256: "7473121ad7972b6b3c6796ec8370dd17c10cc93069085356c8da19e23b5227e3"
---

When you use Multiple Units of Measure with the Serialized Inventory or Lot Tracking features, you have more flexibility on sales and purchases. You can purchase, stock, sell, and handle inventory transactions for items in different units of measure.

Your purchase units for a serial or lot item might differ from the stock units, and your stock units might be different from the sale units. You can set the units of measure separately for purchasing, stocking, and selling each serial or lot item.

For example, a food distributor tracks goods by assigning a lot number and expiration date to a perishable product, item #4567. They order this lot numbered product from the vendor by the truckload. It is stocked at a central warehouse by the pallet, and it is sold to customers as single box units. By designating a purchase unit **truck**, stock unit **pallet**, and sale unit **box**, you can use the right units and quantities on each transaction.

To use Multiple Units of Measure, first set up a Units Type and define each unit you need. For example, you can set up a Units Type called Perishable and then add units like Truck, Pallet, and Box. Assign a base unit and define the other units based on it. For example, if your base unit is Box, you can define Pallet as 144 boxes.

For more information about setting up units of measure, see [Setting Up Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212143.html).

Note the following details when working with units of measure for lot or serial items on transactions and records:

-   **Serial Numbered Items**
    
    -   When selecting stock units, purchase units, and sale units on transactions, serial numbered items can't use fractional quantities.
        
    -   The base unit must be the smallest unit of measure.
        
    -   Important:
        
        When you enter transactions with serial numbered items in non-base units, you must enter serial numbers in a quantity equal to the quantity in base units.
        
        For example, if you receive one pallet of a serialized item, and a pallet has 10 base units, you must enter 10 serial numbers on the receipt.
        
        Another example:
        
        -   A purchasing manager creates a vendor bill for one case of serialized inventory.
            
        -   A case has a conversion rate of 6.
            
        -   The base unit is Each.
            
        -   For this transaction, you need six serial numbers, because the quantity of serial numbers must match the number of base units.
            
-   **Lot Numbered Items**
    
    -   Units types you use for inventory items can also be used for lot numbered items.
        
    -   The base unit doesn't have to be the smallest unit of measure.
        
    -   When selecting stock units, purchase units, and sale units on transactions, lot numbered items can use fractional quantities.
        
    -   On transactions, you must enter lot numbers in a quantity equal to the quantity of units on the transaction. This is true regardless of the unit type being used on the transaction.
        
        For example, you are receiving one pallet of a lot numbered item and a pallet is comprised of 10 base units. You must enter **one** lot number on the receipt.
        
        Another example:
        
        -   A purchasing manager creates a vendor bill for 10 cases of lot numbered inventory.
            
        -   A case has a conversion rate of 6.
            
        -   The base unit is Each.
            
        -   The entire case belongs to one single lot.
            
        -   For this transaction, the following image shows that the quantity entered for the lot in the serial/lot numbers field is **10**.
            
            ![UOM Serial Lot](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/ItemRecordManagement/UOMwSerLot3.png)
-   **Serial Numbered Items** and **Lot Numbered Items**
    
    After you set up units of measure on an item, you can edit the units, but you can't change the units type.
    
    You can add line items to the following transactions using units of measure:
    
    -   Enter Purchase Orders
        
    -   Enter Vendor Return Authorization
        
    -   Write Checks
        
    -   Use Credit Card
        
    -   Bill Purchase Orders
        
    -   Create Opportunities
        
    -   Prepare Estimates
        
    -   Enter Sales Order
        
    -   Create Invoices
        
    -   Adjust Inventory
        
    -   Transfer Inventory
        
    -   Distribute Inventory
        
    -   Issue Credit Memo
        
    
    Note:
    
    On some transactions where you can change units, only units that qualify appear in the units list.
    
    The following transactions display units of measure that cannot be changed:
    
    -   Receive Purchase Order: displays units selected on purchase order
        
    -   Fulfill Sales Orders: displays units selected on sales order
        
    -   Adjust Inventory Worksheet: displays default base units
        
    -   Replenish Location: displays base units
        
    
    **Purchase Transactions**
    
    You can enter purchase transactions with lot and serial numbered items using units of measure other than stock units. This is useful when your vendor sells items in units that are different from units you use to stock items in the warehouse.
    
    **Item Purchases**
    
    When you enter a purchase order that includes a lot numbered or serialized item, the units appear on the transaction line with the item. The unit of measure that appears by default is the purchase unit defined on the item record.
    
    You can edit the selection in the Units field, if necessary. The available units of measure are based on the available units on units type page.
    
    **Item Receipts**
    
    When you enter an item receipt with a lot numbered or serialized item, the units appear on the transaction line with the item. When you receive lot or serial numbered items, the receipt unit always comes from the unit selected on the originating purchase order. The unit of measure displayed is for reference and can't be changed.
    
    **Other Purchase Transactions**
    
    When you enter a vendor return, write a check, enter a credit card transaction, or bill a purchase order, the default unit for a lot numbered item is the purchase unit set on the item record. You can change the Units field if you need to.
    
    **Sales, Fulfillment, and Billing Transactions**
    
    You can enter transactions with lot and serial numbered items using units other than stock units. This is useful if your customer buys the items in units that are different from the units you use to stock items in the warehouse.
    
    For example, most of your customers buy item #4567 by the box, but one customer buys it by the pallet. You can enter a sales order for that customer a sell in pallet quantities instead of boxes.
    
    **Sales Transactions**
    
    When you enter a sales order, opportunity, or quote with a lot numbered or serialized item, you can select the unit of measure on the transaction line. Select any unit defined on the Units of Measure page.
    
    **Fulfillments**
    
    When you enter an item fulfillment with a lot or serial numbered item, the fulfillment unit always comes from the unit selected on the originating sales order. The unit displayed is for reference and can't be changed on the transaction line.
    
    **Billing and Credits**
    
    When you enter an invoice or credit memo for a lot or serial numbered item, you can set the unit of measure on the transaction line **and** choose from all available units of measure.
    
    **Inventory Transactions**
    
    You can enter inventory transactions with lot and serial numbered items using units other than stock units. This is useful if you adjust inventory to store defective items using units different from the regular stock units you use in the warehouse. You can view the unit of measure for lot and serial items when you enter an inventory adjustment with the adjustment worksheet.
    
    **Inventory Adjustments and Transfers**
    
    When you enter an inventory adjustment or transfer with a lot or serial numbered item, you can set the unit of measure on the transaction line **and** choose from all available units of measure. When you enter an inventory adjustment worksheet or inventory distribution, the transaction displays only base units for lot and serial numbered items. This is also true when you replenish a location.
    

### Related Topics

-   [Enabling Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163283384203.html)
-   [Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2211898.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
