---
id: "section_N2351146"
type: "section"
title: "Time and Status Updates on Tasks"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Routing Completions and Time Entry > Time and Status Updates on Tasks"
parent: "section_N2350143"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2351146.html"
anchors: ["bridgehead_N2351241", "bridgehead_N2351347"]
sha256: "3aec7c8b73f96f339f71c044b76564d62cd0be0536adb9c824b6d83e9ccdb954"
---

Time entered against an operation task ensures scheduling for all related tasks are updated to accurately portray progress against each operation.

Often machine and labor resources working concurrently are fully used against a certain operation task. In such cases, both resource types are weighted equally to determine the true time recorded on the operation task record.

Sometimes, one resource may have a higher value than the other resource for a certain task. For example, on a task, the machine run time is less than labor run time. In such a case, the critical path is the labor time because it is the greater of the two. NetSuite updates the production schedule based on the larger requirement of the two. This applies to setup time and run time.

In another example, the recorded machine time is larger than the labor time because the machine can run without constantly being overseen by labor. In this case, the machine time is the critical path, and NetSuite uses it to update scheduling. NetSuite uses the labor time for costing purposes.

For an operation, if the labor run time is larger than the machine run time, NetSuite uses the labor run time as the true hours.

Note:

The default values that show for machine run and labor run times can be modified to accommodate individual run times.

After the appropriate time values are determined, the amount appears in the **Actual Hours** field on the operation task record. Based on the hours recorded, NetSuite adjusts the schedule of subsequent tasks to provide a realistic view for completions.

## Operation Task Status Updates {#bridgehead_N2351241}

NetSuite updates the status of an operation task based on data entered for the work order or tasks. Possible status options include the following:

-   **Not Started**
    
    -   No time is recorded against the task.
        
    -   No quantity completed is recorded on the task.
        
-   **In Progress**
    
    -   Some time is recorded against the task.
        
    -   Some quantity completed is recorded on the task **and** the completed quantity is less than the input quantity required.
        
-   **Completed**
    
    The completed quantity is equal to or greater than the input quantity required **or** the work order is closed.
    

## Mark a Routing Work Order as Built or Closed {#bridgehead_N2351347}

For some orders, you may want to show the items as being assembled without finishing all the individual steps for each operation task. In such a case you can do one of the following:

-   **Mark an Order Built**
    
    When you mark an order as built, the required items are marked built and added to inventory. Note that associated variances **aren't** created.
    
    To mark a work order built, go to _Transactions > Manufacturing >Mark Work Orders Built_.
    
    For more information, see [Marking Work Orders Built](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2322811.html).
    
-   **Mark an Order Closed**
    
    When you mark an order as closed, the required items are marked built and added to inventory. Note that associated variances **are** created.
    
    To mark a work order closed go to _Transactions > Manufacturing >Mark Work Orders Built._.
    
    For more information, see [Marking Work Orders Closed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2323037.html).
    

After you mark an order as built or closed, the operational task record associated with that order displays a task status displays as Completed.

### Related Topics

-   [Manufacturing Routing Completions and Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350143.html)
-   [Routing Work Order Completions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350305.html)
-   [Routing Completion Labor and Machine Time Entry](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2350729.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
