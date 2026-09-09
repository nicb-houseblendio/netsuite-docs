---
id: "chapter_N2319010"
type: "chapter"
title: "Assembly Items"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Items"
parent: "book_1506002637"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html"
anchors: []
sha256: "a27dac0a8846a8e1a355034c9a42b9844f8621201a43dfeaf21526b9cd5d17be"
---

An assembly item is an inventory item made up of several components, but identified as a single item. Assemblies are manufactured by combining raw materials that you stock.

Note:

For details about distinctions between Groups, Kits, and Assemblies, see [Groups, Assemblies, and Kit/Packages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2318089.html).

After you create assembly item records that define the members of an assembly, you can track the raw materials and the assembled items separately.

For example, Wolfe Manufacturing sells the LogLeaper mountain bike that they assemble in-house. The LogLeaper is assembled from the following inventory components:

-   one aluminum bicycle frame
    
-   one set of handlebars
    
-   one saddle
    
-   one gearing assembly
    
-   two wheel assemblies
    
-   two sets of brakes
    
-   two pedals
    

NetSuite tracks the stock of the LogLeaper and each component item separately. This enables Wolfe to track the stock levels of LogLeaper mountain bikes in inventory and available to ship to customers. Wolfe can also track the quantity of materials available to assemble more bicycles.

To use assembly items, you must complete the following tasks:

1.  Enable the Assembly Items feature. For more information, see [Enabling Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319428.html).
    
2.  To create assembly item records that define the assembly components, select the parts that make up the assembly. For more information, see [Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2319594.html).
    
    -   To create an assembly item record, go to _Lists > Accounting > Items > New_
        
    -   On the **New Item** page, click **Assembly**. For more information, see [Creating Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2166469.html).
        
3.  Record an assembly build:
    
    -   After you create an assembly item record, enter an assembly build to record assembly production. Physically manufacturing assemblies in a production run increases your stock of assembled items.
        
    -   To record inventory level changes, go to _Transactions > Inventory > Build Assemblies_ to enter an assembly build for each production run. For more information, see [Building Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2321340.html).
        
    -   After you create your assembly item, build the assembly in NetSuite to replenish stock. To record an assembly build, go to _Transactions > Inventory > Build Assemblies_.
        
    
    NetSuite tracks assembly item and member component records separately. It also tracks the assembly and member item stock status individually. For each assembly build you record:
    
    -   the assembly item stock level increases
        
    -   the member items' individual stock levels decrease
        

### Related Topics

-   [Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1506002637.html)
-   [Manufacturing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1506100009.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)
-   [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html)
-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)
-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Outsourced Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157833700001.html)
-   [SuiteAnalytics Manufacturing Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1549896702.html)
-   [Engineering Change Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1531288763.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
