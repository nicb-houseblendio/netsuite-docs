---
id: "chapter_N2341076"
type: "chapter"
title: "Manufacturing Routing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing"
parent: "book_1506002637"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html"
anchors: ["procedure_N2341107", "procedure_N2341145", "procedure_N2341182", "svg_1", "svg_1background", "svg_1Node", "svg_1Straight_Thin"]
sha256: "fff283b310f4aae1e343c69c128c8b2b28aa8fed8896b74a905cb5b9e7728e33"
---

Manufacturing Routing and Work Center lets you schedule and record manufacturing operational activities against a work order that requires multiple employees, or work centers. For example, you may have a set of operations for the following: a preparation team, an assembly run team, and a quality assurance team.

You can use the Manufacturing Routing and Work Center feature to record quantity assembly completions and team resource costs. You can also use it to process overhead costs against individual work order operations.

The following roles represent members of your organization who can benefit from using Manufacturing Routing.

## Operational Planner or Production Manager {#procedure_N2341107}

Your Operational Planner or Production Manager can benefit from this improved planning efficiency:

-   Set up a routing record that defines multiple steps for building a complex assembly.
    
-   Assign default scheduling parameters against each step.
    
-   Use backward scheduling to establish a supply plan based on manufacturing scheduling requirements.
    

## Production Manager {#procedure_N2341145}

Your Production Manager can refine the shop floor tracking activities using the following:

-   Facilitate scheduling by assigning work center groups to operation steps.
    
-   Record progress of activities such as completion and component issue against multiple tasks or one task at a time
    
-   Record actual machine and labor times against anticipated times.
    

## Cost Accountant {#procedure_N2341182}

Your Cost Accountant can identify opportunity areas:

-   Assign labor and machine overheads against completion activities.
    
-   Develop a costing template for standard rates used in multiple routings.
    
-   Track cost variances between actual and standard at a per service item and cost category level.
    

Important:

Be aware of the following:

-   Manufacturing Routing can be used only with assembly items using standard costing or average costing.
    
-   Manufacturing Routing can be used only with work orders that are marked as Work In Process (WIP).
    
-   Manufacturing Routing creates variances based on per-service item and cost categories.
    

To use the Manufacturing Routing and Work Center feature, a user with sufficient permission must do the following:

-   enable the feature
    
-   define cost categories
    
-   define charge items
    
-   create cost templates
    
-   define resources
    
-   create routings
    
-   set up standard costing, if required
    

The following tasks must be completed:

-   Complete the [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html) procedures.
    
    This lets you use routings on WIP designated work orders.
    
-   The steps required to complete the assembly are detailed in operation task records. For more information, see [Manufacturing Routing and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html).
    
    These task records designate what needs to be done and when, how much has been done, and how much remains to be done. They define how much time you expect to spend on the task and the rates to be charged for it. Task records designate work centers to assign tasks to certain labor resources.
    
-   During the assembly process, NetSuite logs time against tasks to show progress towards completion. By entering data on the completion form you determine the following:
    
    -   **Starting and Ending Operation** - operation tasks that are done
        
    -   **Quantity Completed** - time logged against each operation
        

Completion records show the time machines and labor used. When time is entered against an operation task, the scheduling for all tasks related to the work order automatically update. This update accurately portrays progress against each operation. For more information, see [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html).

Values for assets and expenses associated with a routing work order post to the designated Work In Process (WIP) account during the assembly process.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       

Values are added to the WIP account based on time logged against operation tasks or quantity produced in a run. After the assembly process completes, the values are removed from the WIP account and added to the Asset for Assembly account. For more information, see [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html).

### Related Topics

-   [Work Center Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3911875603.html)
-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498757185.html)
-   [Manufacturing Routing and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html)
-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Supply Planning and Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html)
-   [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html)
-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1498757185.html)
-   [Manufacturing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1506100009.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)
-   [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html)
-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)
-   [Outsourced Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157833700001.html)
-   [Manufacturing Preferences Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159112534056.html)
-   [SuiteAnalytics Manufacturing Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1549896702.html)
-   [Advanced Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1506521222.html)
-   [Manufacturing Mobile](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_158644016906.html)
-   [Engineering Change Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1531288763.html)
-   [Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1506002637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
