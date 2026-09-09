---
id: "section_N2345383"
type: "section"
title: "Creating a Manufacturing Routing"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Creating a Manufacturing Routing"
parent: "chapter_N2341076"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2345383.html"
anchors: ["procedure_N2345433"]
sha256: "8a38b44f0993ae9e504e9498f7f70e5982902c920b29c2fa23bb8068bbe40791"
---

A manufacturing routing is a template that contains a list of steps required to build an assembly item. Each step is in the order necessary to complete the operational sequence for completing the assembly.

After you create a routing record, that routing can be selected on a work order to direct the completion of the assembly. The routing determines the work center, cost template, labor resources, and machine resources that will be used during the assembly.

Routings are unique for each assembly item. However, routings can be shared across multiple locations.

#### To enter a manufacturing routing: {#procedure_N2345433}

1.  Go to _Lists > Supply Chain > Manufacturing Routing > New_.
    
2.  Select the **Item** you are creating an assembly sequence for.
    
3.  Enter one or more locations where this assembly will be performed.
    
4.  Enter a routing template **Name**.
    
    This name appears in the list of routings in the **Manufacturing Routing** field on records and forms. For example, enter **Beta Alternate Supply Routing**.
    
5.  Optionally, enter a **Memo**.
    
    You can search for the text you enter in this field. For example, enter **Use Beta Alternate** when primary widget supply is unavailable.
    
6.  Check the **Default** box to use this routing by default for this item on forms.
    
    When you check this box, these routing steps will be used when new special work orders and mass created work orders are created.
    
    Clear this box if you do not want this routing to be used by default.
    
7.  Check the **Inactive** box if you do not want this routing to show in routing lists on records and forms.
    
    Clear this box if you do want this routing to show in lists.
    
8.  Check the **Auto-calculate Lag** box if you want NetSuite to calculate lag times for operation tasks.
    
    For more information, see [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html).
    
9.  Click the **Routing Steps** subtab.
    
10.  Enter the **Operation Sequence** number for the step you are entering.
     
11.  For example, if you are entering the first step to be performed to build this assembly, enter 1.
     
     Sequence number determines dependencies between different operations. For example, operation 1 comes before operation 3 in the assembly process.
     
12.  Enter the **Operation Name**.
     
     For example enter Assembly Setup.
     
13.  Select a **Manufacturing Work Center**. This is the labor team that will complete this step.
     
     After you select a work center, the labor resources and machine resources are automatically entered from the work center record.
     
14.  Select a **Manufacturing Cost Template** for this operation.
     
15.  Enter the operation **Setup Time** in minutes.
     
     This is the amount of time required (fixed time per step) to prepare for this step in the sequence. For example, this could represent the time in minutes required to warm up a molding machine to bring the mold to the proper temperature.
     
     There is one setup time per order.
     
16.  Enter the operation **Run Rate** in minutes.
     
     This is the amount of time required to complete a run and produce one unit.
     
     -   NetSuite uses the **Setup Time**, **Run Rate** and the default calendar to schedule the completion of each step for work orders using this routing.
         
     -   If you use the Demand Planning feature, NetSuite uses backward scheduling to determine the appropriate start date. There is one run time per base unit.
         
     -   The **Setup Time** + **Run Rate** = total manufacturing task time.
         
17.  Select the **Connection Type**.
     
     Define operations overlapping by selecting **Finish-To-Start** or **Start-To-Finish** connection type.
     
     For more information, see [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html).
     
18.  If you did not check the **Auto-calculate Lag** box, set **Lag Type**, **Lag Amount**, and **Lag Unit**, as necessary.
     
19.  Click **Save**.
     

Tip:

You can create a new routing by clicking the **New Manufacturing Routing** button on the **Manufacturing** subtab of an assembly item record.

### Related Topics

-   [Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2341076.html)
-   [Setting Up Manufacturing Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2341463.html)
-   [Work Center Calendars](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3911875603.html)
-   [Manufacturing Routing and Work Orders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346224.html)
-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Supply Planning and Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349847.html)
-   [Production Scheduling Methods Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4000988757.html)
-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Manufacturing Routing Costing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351557.html)
-   [Work Instructions and Traveler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_9135201182.html)
-   [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
