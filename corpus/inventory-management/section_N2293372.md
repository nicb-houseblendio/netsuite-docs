---
id: "section_N2293372"
type: "section"
title: "Creating Item Supply Plans"
branch: "inventory-management"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Inventory Management > Advanced Inventory Management > Demand Planning > Creating Item Supply Plans"
parent: "section_N2286970"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293372.html"
anchors: ["procedure_N2293414", "bridgehead_4036165701"]
sha256: "0637e8d4d33e570dc5558d2374fbe9a15c11a8ad1546845c7582bfb324b635c3"
---

After you create demand plans, you can create individual supply plans for specified items. A supply plan lists orders for items based on beginning inventory, safety stock, lead time, and projected demand.

Important:

The NetSuite [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution replaces Time-Phased Planning and offers more features and better performance.

New customers should use the [Supply Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_159171867422.html) (MRP) solution. Existing customers should plan to move from Time-Phased Planning to MRP.

When you generate supply plans from demand plans, NetSuite creates work orders or purchase orders that replenish items in the appropriate quantities.

For more information about which orders are included in demand plan calculations, see [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html).

#### To create item supply plans: {#procedure_N2293414}

1.  Go to _Transactions > Demand Planning > Generate Item Supply Plan_.
    
2.  If you use NetSuite OneWorld, select a subsidiary.
    
3.  If you use the Multi-Location Inventory feature, select a location.
    
    The list only shows time-phased replenishment items for the selected location.
    
4.  Select a department, if you track them.
    
5.  Select a class, if you track them.
    
6.  If you use the Distribution Resource Planning feature, choose a setting for the **Plan Through Distribution Network** box.
    
    If you check this box, NetSuite runs demand planning for all items and locations in the network.
    
    -   First, NetSuite evaluates affected items based on the selection
        
        -   All assemblies associated with this item
            
        -   All components associated with this item
            
    -   Next, NetSuite evaluates all locations based on the selection
        
        -   All source locations in the Bill of Distribution associated with this location
            
        -   All destination locations in the Bill of Distribution associated with this location
            
7.  The **Start Date** field sets the earliest transaction date for new orders created. Verify the default current date or enter another date.
    
8.  In the **End Date** field, enter the last date in the range you want to create orders through. Orders are created for item demand on or before the end date you select.
    
    For example, if you enter **July 30**, supply plans are created based on demand between the current date and July 30th.
    
9.  Select all items you want to create supply plans for.
    
10.  Click **Submit**.
     

When you click **Submit**, NetSuite creates supply plans for the selected items.

Note:

If you use the Assemblies feature, linked items also get supply plans. For example, if an assembly has a component item that uses time-phased replenishment, NetSuite creates the supply plan for the component item too.

In the Item Supply Plan list, to open an individual plan, click the plan name.

When you open an individual plan, the Item Supply Plan page shows the orders NetSuite will create based on information from the Generate Supply Plan page.

When NetSuite calculates the supply plan, it treats prior transactions as existing supply orders on the planning start date:

-   A purchase order that is not closed
    
-   A purchase order that is not fully received
    
-   A purchase order that has a date that is before the start date
    

If an existing purchase order doesn't have an expected receipt date, NetSuite uses the transaction date as the receipt date.

For more information, see [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html).

## Manufacturing Routings {#bridgehead_4036165701}

If you generate orders and use the Manufacturing Routing and Demand Planning features, you can set production scheduling methods on work orders. For more information, see [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html) and [Supply Planning and Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html).

### Related Topics

-   [Setting Up Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2288536.html)
-   [Demand Planning on Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2289082.html)
-   [Calculating Item Demand](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2290234.html)
-   [Monitoring the Demand Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291615.html)
-   [Viewing, Editing, and Deleting a Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2291961.html)
-   [Manually Entering an Item Demand Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2292418.html)
-   [Monitoring the Supply Plan Status](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2293790.html)
-   [Viewing, Editing, and Deleting a Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294140.html)
-   [Manually Entering an Item Supply Plan](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294552.html)
-   [Creating Orders from Supply Plans](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2294794.html)
-   [Reporting on Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2295256.html)
-   [Distribution and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2296427.html)
-   [Demand Planning and Inventory Allocation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740808760.html)
-   [Time Fences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3848058018.html)
-   [Planning Action Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3865354301.html)
-   [Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2286970.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
