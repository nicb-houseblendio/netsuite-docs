---
id: "section_N2332170"
type: "section"
title: "Work Orders and Demand Planning"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Work Orders > Work Orders and Demand Planning"
parent: "chapter_N2328390"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html"
anchors: ["bridgehead_N2332181", "procedure_N2332209", "procedure_N2332261", "svg_1", "svg_1Layer_2", "svg_1Layer_1"]
sha256: "df409373c9ac54ba3691fdd877047a951e44b3f49589ce5d881201eb6a3fbf7c"
---

When you use the Work Orders and Demand Planning features, you can create work orders to replenish stock, based on demand for assembly items. These work orders use information from item records to calculate lead times for orders.

## Lead Time for Supply Planning {#bridgehead_N2332181}

When you use the Work Orders and Demand Planning features, assembly item records show the **Work Order Lead Time** field.

In the **Work Order Lead Time** field, enter the lead time (in days) to build one assembly in the base unit. Then, NetSuite calculates the lead time for a work order using the following:

Lead time for a work order=

Work Order Lead Time on Item Record \* Quantity in base unit of measure

## Work Order Start and End Dates {#procedure_N2332209}

When you use Demand Planning, if either the start date or end date is left blank, it can be calculated in the following way:

-   When an **End Date** is entered but the **Start Date** is blank, the start date is calculated as follows:
    
    Start Date = End Date - (Work Order Lead Time from the item record \* Quantity in base unit of measure)
    
-   When a **Start Date** is entered but the **End Date** is blank, the end date is calculated as follows:
    
    End Date = Start Date + (Work Order Lead Time from the Item Record \* Quantity in base unit of measure)
    

Note:

The natural rounding method is used to determine the start and end date of work orders.

## Work Orders and Sub-Assemblies {#procedure_N2332261}

When you generate a new supply plan for an assembly item, it calculates material requirements based on the lowest level of component items needed. This is true for assembly items that have the **Mark Sub-Assemblies Phantom** box checked on the item record. For example, the following diagram depicts the Coffee Gift Set assembly item and has the following component structure.

<a id="svg_1"></a>

                                                                                                                                                                                                                                                                                                                                   

-   Assembly Item A: Coffee Gift Set
    
    -   Component B: Coffee Bean Pair
        
        -   Component E: Bag of Regular Beans, 1 lb.
            
        -   Component F: Bag of Decaf Beans, 1 lb.
            
    -   Component C: Coffee Grinder
        
    -   Component D: Travel Mug
        

The **Mark Sub-assemblies Phantom** box is checked on the item record for Item A: Coffee Gift Set. When a planned work order is generated for a Coffee Gift Set, the component assembly requirements are for items E, F, C and D. And, the purchase order created shows these items. Notice that Item B: Coffee Bean Pair isn't a requirement itself, only its member components are required.

Also, the Mass Create Work Order page displays the lines from the supply plan with the Mark Sub-assemblies Phantom box disabled.

By contrast, the **Mark Sub-assemblies Phantom** box is clear on the item record for Item A: Coffee Gift Set. The work order is created only for items B, C, and D. If B isn't available, NetSuite doesn't create a work order.

### Related Topics

-   [Two Types of Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161538863125.html)
-   [Enabling the Work Orders Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161538373436.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)
-   [Mass Creating Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330082.html)
-   [Marking Assemblies to Create Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330700.html)
-   [Planned Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3872474232.html)
-   [Component Yield Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727093231.html)
-   [Editing a Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331050.html)
-   [Printing a Work Order Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331127.html)
-   [Appending a PDF File to Print with the Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331613.html)
-   [Building Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331860.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)

window.addEventListener("load", function() { svgPanZoom('#svg\_1', { zoomEnabled: true, controlIconsEnabled: true }); },false); window.addEventListener("resize", function(){ svgPanZoom('#svg\_1').resize(); svgPanZoom('#svg\_1').fit(); svgPanZoom('#svg\_1').center(); },false);
