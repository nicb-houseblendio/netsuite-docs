---
id: "section_N2349847"
type: "section"
title: "Supply Planning and Routing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Supply Planning and Routing"
parent: "chapter_N2341076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html"
anchors: ["bridgehead_N2349881", "bridgehead_N2349947", "bridgehead_4035339358"]
sha256: "0f65a34d2935ee5cc86348ff2cd86f58d9d523c336598ab6e3995917342442ea"
---

If you use the Demand Planning and Manufacturing Routing and Work Center features, routings on work orders can affect your supply planning. This is because supply planning uses backwards scheduling to meet manufacturing due dates.

Note:

Procurement lead times do not affect these time requirement calculations.

The supply planning method used depends on whether a default routing is identified.

## Without a Default Routing {#bridgehead_N2349881}

When you generate a supply plan on the Generate Supply Plan page, NetSuite calculates the order date (or release date). NetSuite bases the calculation on the due date using the following formula for assembly items that are required to be built:

Order Date = Due Date - (Quantity x Work Order Lead Time)

-   Quantity = Quantity of items required
    
-   Work Order Lead Time = Number of days required to build, per unit
    
-   Due Date = Date when the additional supply is required
    
    ![Diagram of order date and due date without a default routing.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Manufacturing/routingSupplyPlanning1.png)
    
    Note:
    
    Without a default routing, NetSuite makes calculations without reference to any calendar or resource requirements.
    

## With a Default Routing {#bridgehead_N2349947}

When you use Manufacturing Routing and Work Center, the supply planning engine considers the default routing and associated work calendar for scheduling purposes.

When an assembly build is required and a default routing is defined, NetSuite calculates the cumulative lead time across all operation sequences. NetSuite uses the following formula:

Total time =

\[Sum of Setup Time for all operation tasks + (Sum of Run Rate x Quantity)\] x Total Hours per day

**Note**:

-   Setup Time = Total cumulative setup time across all operation sequences in the default routing
    
-   Run Rate = Total cumulative run time across all operation sequences in the default routing
    
-   Total Hours per day = Total number of hours available on the associated work calendar
    

NetSuite calculates the order by backward scheduling from the due date. NetSuite does consider the associated work calendar for days available, including holidays.

![Diagram of order date and due date with a default routing.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Manufacturing/routingSupplyPlanning2.png)

If changes are made to the associated work calendar or to the routing record, you should regenerate the supply plan. These changes can include:

-   modifying the work calendar (such as to increase/decrease the working days or add/remove holidays)
    
-   editing the routing to increase/decrease a setup time or run rate
    

After regeneration, NetSuite modifies the order dates to reflect the new requirements and still meet the due date deadline.

## Routings and the Generate Work Order in Supply Plan Preference {#bridgehead_4035339358}

NetSuite supply plan processing for an assembly with a routing defined depends on your setting for the Generate Work Order in Supply Plan preference.

| **Generate Work Order in Supply Plan Setting** | **Default Scheduling Method** | **Result** |
| --- | --- | --- |
| **Do Not Generate** | \- | The supply plan uses backward scheduling to determine order date. In this case, NetSuite creates only the supply plan line, not the Work Order. |
| **Not Do Not Generate** | Forward | The supply plan uses backward scheduling to determine the order date. Within the supply plan run, NetSuite automatically creates a work order, and sets the production start date the same as the order date. When the work order is created, NetSuite uses forward scheduling to calculate the work order production end date and sets the production start date. In this case, the supply plan creates an order. |
| **Not Do Not Generate** | Backward | NetSuite creates a work order using the receipt date from the demand plan. The production end date is set at one day prior to the receipt date. This allows time to complete production and be available on the required date. The work order uses backward scheduling to calculate the work order production start date. In this case, the supply plan creates an order. |

For information about setting the Generate Work Order in Supply Plan preference, see [Setting Routing Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3950900044.html).

### Related Topics

-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Work Center Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3911875603.html)
-   [Creating a Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html)
-   [Manufacturing Routing and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html)
-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html)
-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html)
-   [Work Instructions and Traveler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_9135201182.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
