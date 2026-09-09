---
id: "section_N2349668"
type: "section"
title: "Work Centers and Manufacturing Operations Tasks"
branch: "manufacturing"
category: "scm-supply-chain-management"
breadcrumb: "SCM (Supply Chain Management) > Manufacturing > Manufacturing Routing > Manufacturing Operation Tasks > Work Centers and Manufacturing Operations Tasks"
parent: "section_N2346668"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2349668.html"
anchors: ["procedure_N2349725"]
sha256: "adfc19aa2a47fd6e8b60a06e3025631bb9c4b29b6352248fe1d1e9d674d513f2"
---

You can view the Manufacturing Operations Tasks list to process work orders based on work centers. This lets you see which centers have completed tasks that are predecessors for other tasks to be worked on.

You can view the operation tasks list and filter the list to show only tasks associated with Work Center 2. Customize the view to show the Predecessor and Predecessor Completed Quantity. These fields let you see which tasks Work Center 2 is due to work on next. (Create a custom view for the task list to display specific columns and information by clicking **Edit View**.)

For example, the task list shows that two work orders have tasks for which the predecessors are completed. You know that Work Center 2 needs to work on those tasks. When Work Center 2 finishes their requirement for the tasks, click **View** next to those tasks in the task list to enter completions. The completions entered then update associated work orders with new predecessor data. The work center task lists display the updated task statuses.

After completions are entered for tasks, scheduling is updated for labor and machines to reflect calculations based on the new entries.

For example, you complete work earlier than anticipated. Therefore, subsequent tasks move up and start and end dates reschedule to be earlier. However, if a completion reflects that work is falling behind, subsequent tasks move out and start and end dates reschedule to be later.

#### To view the operation tasks list: {#procedure_N2349725}

1.  Go to _Transactions > Manufacturing > Manufacturing Operations Tasks_.
    
2.  Optionally filter the list by selecting a work center.
    

### Related Topics

-   [Manufacturing Operation Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2346668.html)
-   [Operations Overlap](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4048453519.html)
-   [Manufacturing Operation Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2347042.html)
-   _Manufacturing Task Scheduler_
    

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
