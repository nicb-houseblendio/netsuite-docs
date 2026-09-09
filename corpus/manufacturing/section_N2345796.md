---
id: "section_N2345796"
type: "section"
title: "Standard Costing for Manufacturing Routing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Creating a Manufacturing Routing > Standard Costing for Manufacturing Routing"
parent: "section_N2345383"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345796.html"
anchors: ["bridgehead_N2345964"]
sha256: "f0838e38d945f4672f504086283f7db0e9b39b33f16bb30be05f156e97de7d54"
---

If you use the Standard Costing and Manufacturing Routing and Work Centers features, NetSuite performs calculates the assembly cost. NetSuite incorporates the labor and machine costs, based on the default routing.

Standard Costing with routings requires the following:

1.  **Cost Version**
    
    Verify that you have created a cost version.
    
    For more information, see Defining Cost Versions [Defining Cost Versions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2202327.html).
    
2.  **Planned Standard Cost Rollup**
    
    Run a cost rollup to calculate assembly cost. When you run a cost rollup, NetSuite checks for a default routing to calculate costs for the assembly. If you have no defined default routings, NetSuite uses the first routing created as the default routing to calculate the assembly cost.
    
    Planned Standard cost is a consolidation of cost based on the component and cost category.
    
    For subassemblies, each of the cost categories are rolled up to the next level in the Bill of Materials (BOM) hierarchy. The difference between the cost categories of this level and lower levels in the roll up depend on the items associated with the rollup.
    
    Note the following when you review the cost of an assembly item based on the cost rollup. The lower level routing cost of building the subassembly is denoted with the subassembly item as a component on the planned standard cost record. The routing cost of building this level final assembly is denoted as follows. The Service and Other charge items appear as a component on the planned standard cost record.
    
    For more information, see [Standard Cost Rollup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2204939.html).
    
3.  **Inventory Revaluation**
    
    When you use Standard Costing features, run update production cost to establish a standard cost in production.
    
    For more information, see [Revalue Standard Cost Inventory](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2205401.html).
    

## Manufacturing Routing Cost Calculation {#bridgehead_N2345964}

NetSuite calculates the cost of each step in a routing as follows:

-   Part 1: Definition of Time / Quantity
    

Total Setup Time = (number of resources x setup time)

Total Run Time = (number resources x run time)

-   Part 2: Rate
    

Based on the manufacturing charge item, the quantity is the total hours required.

The total unit cost is derived at a component level per cost category and per operation sequence.

-   Number of resources (from the work center) x Setup Time (from the routing record) x Manufacturing Charge Item Unit Cost (from the item record)
    
-   Number of resources (from the work center) x Run Rate (from the routing record) x Manufacturing Charge Item Unit Cost (from the item record)
    

For more information about costing, see [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html).

### Related Topics

-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
