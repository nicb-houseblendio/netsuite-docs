---
id: "section_N2330082"
type: "section"
title: "Mass Creating Work Orders"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Work Orders > Mass Creating Work Orders"
parent: "chapter_N2328390"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330082.html"
anchors: ["procedure_N2330139"]
sha256: "fb184ae51c6b2430792b5f4439741979bc686b076c57c9c47c1eb7de424f1b20"
---

You enter work orders to track the production of assembly items needed either for stock or to fill orders. The work order lists the members, or components, of the assembly item to be built. A work order is a non-posting transaction.

Some work orders in the queue aren't intended for a particular sale. Production work orders are generated when the back ordered quantity of an assembly reaches its assigned build point. After the build point is reached, a work order is added in the Mass Create Work Orders queue.

For each work order, a bill of materials (BOM) is generated to facilitate picking member items for the build. When this work order completes, the regular stock level of the assembly is increased and the finished goods are committed to open sales orders.

Special Order work orders track assemblies for a particular sale. Production work orders track assemblies to increase stock. Both use the same work order form, but production work orders don't link to a sale transaction.

After work orders are entered, completing an assembly build for the work order closes the order.

For information about entering individual work orders, see [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html).

#### To mass create work orders: {#procedure_N2330139}

1.  Go to _Transactions > Manufacturing > Mass Create Work Orders_.
    
2.  Select a **Location** to show only work orders for that location. Select **All** to show work orders for all locations.
    
    If you use Multi-Location Inventory, the location selected is the one that component inventory items are committed from.
    
    Note:
    
    All items on one work order must be committed from the same location. Items can commit only from the location specified. This is true even if there are no available items at the specified location, and there are items available at another location.
    
3.  Select a **Department** or **Class** if you track them. The selected department or class appears on the assembly build.
    
4.  Select a **Parent Item** to show only child items for that parent.
    
5.  Enter a **Minimum Quantity** to filter the list by the minimum set on the item record.
    
6.  Complete the fields on the **Time Phased Items** subtab.
    
    The **Time Phased Items** subtab displays a list of items that need to be ordered based on time-phased replenishment.
    
    Note:
    
    To use these enhancements for time-phased planned items, the Demand Planning feature must be enabled.
    
    1.  Check the box in the **Order** column next to each item you want to create a work order for.
        
    2.  Select an **Order Date**.
        
    3.  Select a **Production End Date**.
        
    4.  Check the box next to each item to order.
        
        Click the **Mark All** button to check all boxes or click the **Unmark All** button to clear all boxes.
        
    5.  Accept the suggested **Quantity** or enter a new amount.
        
        Note:
        
        When you use Demand Planning, see [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html) for information about suggested quantities.
        
        When you use Multiple Units of Measure, the quantity for members of an assembly item is always defined in base units on work orders.
        
    6.  Check the **Mark Sub-Assemblies Phantom** box to treat the sub-assemblies within the selected assembly as phantoms. The sub-assembly components are included in the assembly work order that is generated.
        
        For information about work orders and demand planning, see, [Work Orders and Sub-Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html#procedure_N2332261).
        
7.  Click the **Reorder Point Items** subtab.
    
    The **Reorder Point Items** subtab displays a list of items that need to be ordered based on designated reorder point. These items have a quantity available that is less than the reorder point indicated on the item record.
    
    Note:
    
    To use these enhancements for time-phased planned items, the Demand Planning feature must be enabled.
    
    1.  Check the box in the **Order** column next to items you want to order.
        
        Click the **Mark All** button to check all boxes or click the **Unmark All** button to clear all boxes.
        
    2.  Accept the suggested amount to order in the **Quantity** column, or enter a new quantity.
        
        The suggested NetSuite order calculation is: (preferred stock level + quantity needed) less (quantity available + quantity on order).
        
    3.  If you use Make Departments required and Allow Per-Line Departments, select a **Department**. Departments are used for the corresponding line items on generated purchase orders. For more information, see [Using Per-Line Classifications](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265988.html).
        
    4.  Check the **Mark Sub-Assemblies Phantom** box to mark an individual sub-assembly as a phantom assembly. A phantom assembly is typically a non-stocked assembly that groups together material needed to produce a subassembly. The Phantom BOM option lets you define the item source for the subassembly on a line-by-line basis.
        
        If you use the Work Orders and Demand Planning features, see [Work Orders and Sub-Assemblies](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html#procedure_N2332261).
        
8.  Click **Submit**.
    

Work Orders are generated for the items you have indicated. Work orders generated for assembly items that use the Reorder Point replenishment method use Forward Scheduling. This is true regardless of the default scheduling method set in the account preferences. For more information, see [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html).

### Related Topics

-   [Two Types of Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161538863125.html)
-   [Enabling the Work Orders Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161538373436.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)
-   [Marking Assemblies to Create Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330700.html)
-   [Planned Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3872474232.html)
-   [Component Yield Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727093231.html)
-   [Editing a Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331050.html)
-   [Printing a Work Order Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331127.html)
-   [Appending a PDF File to Print with the Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331613.html)
-   [Building Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331860.html)
-   [Work Orders and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
