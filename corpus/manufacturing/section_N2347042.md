---
id: "section_N2347042"
type: "section"
title: "Manufacturing Operation Task"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Operation Tasks > Manufacturing Operation Task"
parent: "section_N2346668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2347042.html"
anchors: ["procedure_N2347133", "subsect_0625022531", "subsect_0625023413"]
sha256: "48789918745a65e9ef768e20976a7c7c23ac86985f512ace547719b4a84bc02f"
---

For any work order with a status of **Pending Build**, you can make changes to operation tasks on the order. For example, due to specifications particular to one order, you may need to change information defaulted on tasks from the routing template.

After work is logged against the order and the status is In Process, you can no longer edit the operation tasks.

On individual task records, you can view the following:

-   **Manufacturing charge items** - Charge items are derived from the routing template, but can be modified as necessary for individual orders.
    
-   **Estimated time required for completion**
    
    When you enter a setup time or run time on the task record, these times are planned estimates and are used for scheduling. It is only after completion time is entered against a task is the actual time updated in the Actual Hours field.
    

Task dependencies are assigned based on the numeric order of the operation sequence and aren't editable.

#### To edit operation tasks: {#procedure_N2347133}

1.  Go to _Transactions > Manufacturing > Manufacturing Operations Tasks_.
    
2.  Click **Edit** next to the operation you want to modify.
    
3.  You can enter a new **Operation Name**.
    
    Note:
    
    When you modify task settings, labor and machine scheduling reflects calculations based on the new entries after you save the task changes.
    
    The following fields **Primary Information** aren't editable:
    
    -   The **Work Order** identifier related to this operation task.
        
    -   The **Insert Before** field identifies the next step in the sequence.
        
    -   The operation sequence **Status**. For example, Not Started, Started, Completed.
        
4.  You can enter any additional **Comments** that you want to accompany this operation task. For example, "use Shimano spokes when Bontrager spokes aren't available."
    
    The following **Operation Overview** fields aren't editable:
    
    -   NetSuite calculates **Estimated Hours** as the expected time to complete a task based on total setup time + quantity x run rate.
        
    -   **Actual Hours** displays the time in hours it took to complete this task.
        
    -   The **Remaining Hours** of work needed to complete this task are displayed.
        
    -   **Input Quantity** represents the number of items entered or created during this task.
        
    -   **Completed Quantity** is the total number of items created during this task.
        
5.  You can change the operation **Setup Time** (in minutes) for the working day as defined in the work calendar.
    
6.  You can change the operation **Run Rate** (in minutes). This is the amount of time required to complete a run and produce one unit.
    
    The following **Operation Schedule** fields aren't editable:
    
    -   The **Start Date** represents the date you expect to begin assembly production. This field defaults to today's date.
        
    -   **End Date** is the date you expect to complete assembly production. This field defaults to today's date plus lead time.
        
    -   Check the **Auto-Calculate Lag** box if you want NetSuite to calculate lag times for operation tasks. For more information, see the [Autocalculate Lag](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html#bridgehead_4048469702) help topic.
        
7.  Unless it is the first operation, you can change operations overlapping in the **Predecessors** subtab. For more information, see the [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html) help topic.
    
8.  Click **Save**.
    

## Work Order Operation Start and End Dates {#subsect_0625022531}

**Operation Start Date** is set to the start time for the working day as defined in the working calendar.

To set an **Operation End Date**, the remaining operation time is added to the operation start of the next working day after the completed time.

When the remaining time exceeds the available working time, any outstanding time is added to the beginning of the next working calendar working day.

## Completions on Non-Working Days {#subsect_0625023413}

**Operation Start Date** is set to the start time for the working day as defined in the working calendar.

To set an **Operation End Date**, the remaining operation time is added to the start of the next working day as defined in the working calendar.

You can also modify tasks from the work order. Go to Transactions > Manufacturing > Enter Work Orders > List. Click **Edit** next to the work order to be edited. Click the **Operations** subtab to view a list of operation tasks.

### Related Topics

-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html)
-   [Work Centers and Manufacturing Operations Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349668.html)
-   _Manufacturing Task Scheduler_
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
