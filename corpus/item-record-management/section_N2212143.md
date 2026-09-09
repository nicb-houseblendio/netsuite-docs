---
id: "section_N2212143"
type: "section"
title: "Setting Up Units of Measure"
branch: "item-record-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Item Record Management > Multiple Units of Measure > Setting Up Units of Measure"
parent: "chapter_N2211898"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212143.html"
anchors: ["procedure_N2212170", "subsect_1014012756"]
sha256: "63f0064da66f4957f1ac02450237067b9b01829de1ee30df9b97fcc3192d26ef"
---

To set up units of measure, first create a record for each units type you want to assign to your items. For example, you can create a units type named Length. Then, create units for the units type. Each unit type can have several units. For example, you can create units like Inch, Foot, and Yard for Length.

You can also use the Import Assistant to add or update units type records and their units. For more information, see [Units Type Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_0622010835.html).

If you are creating a unit of measure for a statistical account, see [Creating a Unit Type for a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3861070181.html).

#### To create a unit type: {#procedure_N2212170}

1.  Go to _Lists > Accounting > Units of Measure > New_.
    
2.  On the Units Type page, in the **Type Name** field, enter the name of the kind of unit you are creating.
    
    For example, you could name it **Length**.
    
3.  In the **Name** column, enter a name for the unit you want to create.
    
    For example, you could have a Length unit called **Inch**.
    
4.  In the **Plural Name** column, enter the plural name for the unit.
    
    For example, the plural for Inch is **Inches**.
    
5.  In the **Abbreviation** field, enter the abbreviation for the singular unit.
    
    For example, the abbreviation for Inches is **in**.
    
6.  In the **Plural Abbreviation** field, enter the abbreviation for the plural unit.
    
7.  Check the box in the **Base Unit** column if the unit you are entering is used to define the other units in this group.
    
    For example, inch is the base unit for the Length units Foot and Yard.
    
    Each units type must have a base unit and can have only one unit designated as the base.
    
8.  In the **Conversion Rate** field, enter the quantity of base units that equal one unit of the current line.
    
    When the **Base Unit** box is checked, the conversion rate for the unit is set and locked at one.
    
9.  Click **Add**.
    
10.  Repeat these steps for each unit you want to add to this type.
     
     Note:
     
     You can't create more than 650 units of the same type,
     
11.  Click **Save**.
     
     Now you can assign the units type to item records.
     

Note:

After you assign a units type to an item, you can't change the item's unit type. Also, after a units type is assigned to any item, you can only add more units. You can't edit the type itself.

After you mark and save a base unit, you can change it by clearing the Base Unit box on the current one and checking that box on the new base unit.

Next, assign a units type to an item to define quantities for purchasing, stocking, and selling the item. For example, when you assign the units type of Length to your inventory item cable, you can purchase the cable in yards. Then you can stock the cable in feet, and sell the cable in inches.

Important:

If you change the purchase unit on the item record, NetSuite automatically converts the prior standard cost in prior units to the new standard cost in new units when you save.

For example, the standard cost field is $1 per inch and you change the purchase unit to cm, the standard cost field changes to $1 x conversion units, or $0.39, when you save.

## Transaction Quantity Limit in Base Units {#subsect_1014012756}

You cannot enter a quantity that exceeds 9,999,999,999 base units in a single transaction line. If this limit is exceeded, you might see an error saying **You've gone over the maximum allowed quantity of 9,999,999,999 base units for this line**. You cannot save the transaction until you fix this error.

This limitation can arise unexpectedly when you use small base units (like Each) together with big conversion rates in other units (like Kg). For example, if your base unit is **Each** and 1 Kg equals 1000 Each, entering a large quantity in Kg may quickly surpass the allowed quantity in base units.

For assembly items on work orders, the quantity is always calculated and stored in base units. Ensure to check your conversion rates and quantities so you don't go over the 10-digit limit for base units.

### Related Topics

-   [Assigning Units of Measure to Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2212390.html)
-   [Enabling Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_163283384203.html)
-   [Serial and Lot Inventory with Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2214525.html)
-   [Multiple Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2211898.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
