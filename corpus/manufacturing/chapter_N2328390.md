---
id: "chapter_N2328390"
type: "chapter"
title: "Assembly Work Orders"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Assembly Work Orders"
parent: "book_1506002637"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html"
anchors: ["subsect_161547480815", "subsect_161547483640", "subsect_161547487068", "article_161538429435"]
sha256: "028efb89509c7f039be90a83a6d17dab15393f00bd766121d07c602d582aaf9f"
---

When you enable the Work Orders feature, you can use assembly work orders for your assembly items.

Assembly work orders track the production of assembly items needed for stock, or to fill orders. Work orders track the quantities of assemblies that need to be built, and the quantities of components, or member items, needed to do so.

For example, if you stock and sell mountain bikes, you can enter a work order to do the following:

-   Track the quantity of mountain bikes that need to be assembled
    
-   Commit member items available in stock to the work order
    
-   Track when the mountain bikes are assembled and the work order is completed to ensure mountain bikes can be stocked or sold
    

## Sales Orders Linked to Work Orders {#subsect_161547480815}

If a work order is created from a sales order, the two transactions are linked. Please note the following about making changes on sales orders or work orders that are linked:

-   If you close a line on a sales order that links to an assembly, the link to the work order remains. The work order remains open and the finished assembly from the build is added to general inventory.
    
-   If you change the quantity on a work order line, note the following. If the quantity exceeds the amount on the corresponding sales order line, the link to the sales order remains. When the build is completed, the excess assemblies are added to general inventory.
    
-   Sales orders that are cancelled are no longer linked to work orders.
    

## Assemblies and Advanced Inventory Management Calculations {#subsect_161547483640}

If you use Advanced Inventory Management and auto-calculation for inventory items that are components of assemblies, note the following. NetSuite bases demand on work orders as well as sales using the following calculation:

Qty of assembly \* qty per assembly

Orders for finished assemblies are included in calculations of demand, reorder points, and preferred stock levels for member inventory items.

You can choose to base demand on sales instead of sales orders if you use the **Transactions to Consider** preference. This preference determines if work orders and builds are included in demand calculations for assembly components. For more information, see [Setting Up Advanced Inventory Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2285514.html).

Note:

For transaction customization purposes, assembly work order forms are classified as sales forms. If you create a custom transaction field and apply it to sales transactions, it shows on work order forms.

**Assemblies and Units of Measure**

If you use Multiple Units of Measure, see [Assemblies and Units of Measure](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2320172.html).

You can make changes on work orders after you create them. For more information, see [Editing a Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331050.html).

## Assembly Work Orders Workflow Chart {#subsect_161547487068}

![Diagram of the assembly work orders workflow.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Manufacturing/AssemblyWorkflowChart.png)

## Work Order Statuses {#article_161538429435}

Work orders can have the following statuses:

-   **Planned** - No components are committed regardless of commit option settings.
    
-   **Released** - No transaction has posted and no activities have been recorded. Components can be committed based on commit option settings.
    
-   **In Process** - A transaction has been posted.
    
-   **Built** - The quantity built is equal to the quantity planned.
    
-   **Closed**
    

### Related Topics

-   [Two Types of Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_161538863125.html)
-   [Enabling the Work Orders Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_161538373436.html)
-   [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html)
-   [Mass Creating Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330082.html)
-   [Marking Assemblies to Create Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2330700.html)
-   [Planned Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3872474232.html)
-   [Component Yield Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3727093231.html)
-   [Printing a Work Order Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331127.html)
-   [Appending a PDF File to Print with the Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331613.html)
-   [Building Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2331860.html)
-   [Work Orders and Demand Planning](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2332170.html)
-   [Manufacturing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1506100009.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html)
-   [Bill of Materials Member Control for Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html)
-   [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html)
-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Outsourced Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_157833700001.html)
-   [Manufacturing Preferences Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_159112534056.html)
-   [SuiteAnalytics Manufacturing Workbook](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1549896702.html)
-   [Advanced Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/preface_1506521222.html)
-   [Manufacturing Mobile](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/part_158644016906.html)
-   [Engineering Change Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1531288763.html)
-   [Manufacturing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/book_1506002637.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
