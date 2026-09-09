---
id: "section_N2346224"
type: "section"
title: "Manufacturing Routing and Work Orders"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Routing and Work Orders"
parent: "chapter_N2341076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html"
anchors: ["procedure_N2346275", "bridgehead_N2346496", "bridgehead_N2346508", "bridgehead_3950991657"]
sha256: "2a2a99009ad54ecf8a063dc94f21f15bdb427cac872b5e88c51f26939fc4161e"
---

If you use manufacturing routing and work centers, you can use routings on work orders to manage your assembly process.

The routing you use on a work order is a template that describes the required steps to build an assembly item. The routing determines the work center, cost template, labor resources, and machine resources to use during assembly.

For more information, see [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html).

#### To use routing on a work order: {#procedure_N2346275}

1.  Create a new work order.
    
    For more information, see [Entering an Individual Work Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2329173.html).
    
2.  In the Classification section, select a **Location**.
    
3.  If you use NetSuite OneWorld, select a subsidiary.
    
4.  Check the **WIP** (Work In Process) box.
    
    When you designate a routing as WIP, NetSuite uses WIP accounting to issue materials in the designated WIP account.
    
    For more information, see [Manufacturing Work In Process (WIP)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2335392.html).
    
5.  Select a **Manufacturing Routing** option.
    
    NetSuite displays the default assembly routing based on the location. However, you can select a different routing.
    
    For more information, see [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html).
    
6.  Click **Save**.
    
    The following subtabs are displayed:
    
    -   The **Items** subtab shows components that are issued.
        
    -   The **Operations** subtab shows all operation tasks required for a particular assembly run.
        
        Operation tasks are created based on the routing. These tasks define the list of steps that must be completed to finish the assembly process. Tasks can be viewed and edited from the work order Operations subtab.
        
        For more information, see the following help topics:
        
        -   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
            
        -   [Manufacturing Operation Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2347042.html)
            

## Work Order Quantity Changes {#bridgehead_N2346496}

If you change the assembly item quantity on the work order and then re-save it, the Operations subtab information updates to reflect the changes. For example, entering a higher quantity on the work order results in more required time to complete the run.

## Routing and Time Zones {#bridgehead_N2346508}

The associated work calendar applies for all routing work orders created.

-   If you **do not use** NetSuite OneWorld, the schedule time zone is based on the time zone selected for the company.
    
    For more information, see [Configuring Company Information](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N240902.html).
    
-   If you **do use** NetSuite OneWorld, the schedule time zone is based on the time zone of the subsidiary selected on the work order.
    

## Planned Time Subtab {#bridgehead_3950991657}

When you use Manufacturing Routing and Work Center and set the **Show Planned Capacity on Work Orders** preference, note the following. Work orders show a Planned Time subtab. This subtab details work allocated to each work center. In addition, NetSuite automatically generates planned time entries. For more information, see [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html).

### Related Topics

-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Work Center Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3911875603.html)
-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html)
-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Supply Planning and Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html)
-   [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html)
-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html)
-   [Work Instructions and Traveler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_9135201182.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
