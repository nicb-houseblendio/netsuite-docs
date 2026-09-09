---
id: "chapter_N2332509"
type: "chapter"
title: "Bill of Materials Member Control for Assembly Items"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Bill of Materials Member Control for Assembly Items"
parent: "book_1506002637"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2332509.html"
anchors: []
sha256: "21919742b3477db128da3f9c25a69029df4c69023e981ef96d8c28b3e2fc4208"
---

Important:

With the release of NetSuite 2023.1 Bills of Materials, where components are embedded to an Assembly Item, will no longer be supported. Only business critical issues will be fixed. To continue working with this functionality you should transition to the [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html) feature, which is free of charge. After you enable this feature, NetSuite will automatically migrate all of your Bill of Materials to the new structure.

When you use the Assembly Items feature, the components needed for assemblies are identified in the Bill of Materials (BOM). Components required for an assembly can change due to engineering changes, vendor supply, availability, or seasonal requirements.

BOM member control helps you ensure that the right components are included in assembly builds at the right time. You can use BOM controls to plan for the utilization and purchase of components that are effective or obsolete within specific time frames.

To use BOM component member control, define effective and obsolete dates for member items on assembly records. NetSuite determines whether a component is valid for an assembly based on these date.

-   **Effective Date/Revision** - Defines the first date an item can be used for an assembly. Before the effective date, the item is not included in the BOM.
    
-   **Obsolete Date/Revision** - Defines the last date an item can be used for an assembly. After the obsolete date, the item is not included in the BOM.
    

After a work order is created, NetSuite determines which components are required based on the transaction date. If you use the Demand Planning feature, NetSuite considers the production start date and determines which components are required on that date.

On assembly item records, choose a BOM control method and set up effective and obsolete dates. NetSuite uses them to determine which member items are needed to create an assembly based on the date the item is produced.

For example, Wolfe Manufacturing assembles bicycles for distribution throughout the year. The mountain bike component item includes the following:

-   Disk brake 1: has an effective date of 4/1/2020
    
-   Disk brake 2: has obsolete date of 3/31/2020
    

Wolfe creates a work order dated 3/31/2020 that includes a Mountain Bike assembly. NetSuite examines the effective and obsolete dates for the components on the assembly record and determines the following:

-   The BOM won't include Brake 1 because it is not effective.
    
-   The BOM will include Brake 2 because it is not obsolete.
    

Wolfe enters a work order dated 4/1/2020 that includes a Mountain Bike assembly, and NetSuite determines the following:

-   The BOM will include Brake 1 because it is currently effective.
    
-   The BOM won't include Brake 2 because it is obsolete.
    

The appropriate assembly BOM items are shown on work orders at the appropriate dates without having to manually change each work order.

For BOM management to track which components are needed at specific times, identify effective and obsolete dates for member items. To do this, select a BOM control method on assembly item records. Select to set dates individually for components or to create revision records to assign to items. When a new work order is created, NetSuite can determine the member items required based on the work order production date. For more information, see [Setting Up BOM Control on Assembly Item Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334154.html).

You can choose to set an assembly to use revision control. For more information, see [Setting an Assembly to Use Revision Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2334812.html).

If you choose to manage assembly BOMs with revision records, set up revision records. For more information, see [Creating Revision Records for BOM Control](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2335150.html).

### Related Topics

-   [Manufacturing Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1506100009.html)
-   [Assembly Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2319010.html)
-   [Assembly Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2328390.html)
-   [Advanced Bill of Materials](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1501506444.html)
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
