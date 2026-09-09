---
id: "section_N2212390"
type: "section"
title: "Assigning Units of Measure to Items"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Multiple Units of Measure > Setting Up Units of Measure > Assigning Units of Measure to Items"
parent: "section_N2212143"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212390.html"
anchors: ["procedure_N2213514"]
sha256: "44d49292280d0d14437c71d38f77ed208bdca47bf1336d7aa78777ac25074176"
---

Assign a units type to an item record to set the default unit of measurement you use to purchase, stock, and sell the item.

Note:

After you assign a units type to an item, you can't change the item's unit type. Also, after a units type is assigned to any item, you can only add more units. You can't edit the type itself.

#### To assign a units type to an item: {#procedure_N2213514}

1.  Go to _Lists > Accounting > Items_.
    
2.  Click **Edit** next to the name of the item you want to assign a units type to.
    
3.  On the **Main** subtab of the item record, in the **Units Type** field, select a units type.
    
    For example, if the item is **cable**, then you might choose **Length** as the units type.
    
    The units type you choose determines which purchase, stock, and sale units you can use.
    
    When you select a units type, the purchase, stock, and sale units all default to the base unit for that type.
    
4.  Select the **Stock Units** you use to track this item's inventory.
    
    The stock unit you choose here is the default for calculating and displaying the following counts for the item:
    
    -   **Reorder Point**
        
    -   **Quantity on Hand**
        
    -   **Quantity Committed**
        
    -   **Quantity on Order**
        
    -   **Quantity Available**
        
    -   **Quantity Backordered**
        
    -   **Average Cost**
        
5.  Select the **Purchase Units** you use to purchase this item.
    
    When you choose this item on a purchase transaction, it defaults to this unit and shows the purchase price for this unit.
    
    The purchase unit you choose here is used to display the **Last Purchase Price** for this item.
    
6.  Select **Sale Units** you use to record sales of this item.
    
    When this item is selected on a sale transaction, it defaults to this unit.
    
    The sale unit you choose here is the default for displaying the following counts for the item:
    
    -   **Sale Price**
        
    -   **Shipping Cost**
        
    -   **Handling Cost**
        
    -   **Item Weight**
        
7.  Select the default **Consumption Unit** of measure for inventory.
    
8.  Click **Save**.
    

Default units you choose on the item record show on purchase and sales transactions, but you can change them if needed. You can't edit units on inventory transactions, however.

Not all item types can have all types of units assigned to them. For example, Non-Inventory for Resale items can have Sale units and Purchase Units but not Stock units.

The table below shows which items can have units assigned, and which types you can assign.

| **Item Type** | **Units Type** | **Stock Units** | **Sales Units** | **Purchase Units** |
| --- | --- | --- | --- | --- |
| Inventory | Y | Y | Y | Y |
| Lot or Serialized Inventory | Y | Y | Y | Y |
| Non-Inventory for Purchase | Y | N | N | Y |
| Non-Inventory for Resale | Y | N | Y | Y |
| Non-Inventory for Sale | Y | N | Y | N |
| Other Charge for Purchase | Y | N | N | Y |
| Other Charge for Resale | Y | N | Y | Y |
| Other Charge for Sale | Y | N | Y | N |
| Service for Purchase | Y | N | N | Y |
| Service for Resale | Y | N | Y | Y |
| Service for Sale | Y | N | Y | N |

On item records for an Item Group or Kit/Package, the units of measure for member items show on the Members subtab. Items are assigned to the group or kit in base unit quantities.

To see the Units Type, Stock Units, Purchase Units and Sales Units for all items, go to _Lists > Items_ and select All in the View field.

### Related Topics

-   [Setting Up Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212143.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
