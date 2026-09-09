---
id: "section_N1206555"
type: "section"
title: "Projects and Milestone Billing"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Projects and Milestone Billing"
parent: "section_N1204906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html"
anchors: ["bridgehead_N1206607", "bridgehead_N1206649"]
sha256: "1c74f5b7ead0642a1f3113c7f7aa853c5022036b1def0f69261ad108ce15e608"
---

You can bill customers for project work at milestone intervals. Instead of being based on the materials used and time worked on the project, billing amounts are based on reaching preset project goals, or billing milestones. To use milestone billing, select Fixed Bid, Milestone as the billing type on the project. Then, create a new Fixed Bid, Milestone type schedule. For more information, see [Creating a Milestone Billing Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207171.html).

Note:

You must enable Project Management and Advanced Billing to use milestone billing.

For details on consolidated projects and milestone billing, see [Fixed Bid, Milestone Project Billing with Consolidation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205308.html#bridgehead_N1205394).

## Fixed Bid, Milestone Billing Schedules {#bridgehead_N1206607}

Milestone projects bill customers when you reach preset goals, or billing milestones. Each milestone marks a point that triggers billing, so you invoice for portion of the total project amount when you hit that milestone.

For example, say you're selling and installing widgets in three phases. When you finish Phase One, you bill the customer for that phase, but not for Phase Two yet. With Milestone Billing, you can bill for each phase as the work gets done.

Billing with Fixed Bid, Milestones schedules is similar to using a standard billing schedule with custom billing dates. You can specify the bill date for a milestone or link it to the completion of a task within the project.

-   If a milestone is linked to a project task, the bill date updates automatically if the task's expected completion date changes.
    
-   When the milestone is marked complete, the amount associated with the milestone is available for billing. If the milestone is linked to a project task, then the milestone is marked as complete when the task is complete. Otherwise, you'll need to mark it complete manually on the billing schedule.
    

Define milestones when you create the billing schedule and optionally link them to project tasks. Assign a percentage of the total amount to each milestone. A Fixed Bid, Milestone schedule is always private and only used for the project it's associated with.

To create revenue recognition schedules for fixed bid milestone billing schedules, you must select revenue recognition templates whose term source is **not** based on a billing schedule. For information about revenue recognition term sources, see [Understanding Revenue Recognition Template Terms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679634.html).

## Monitoring Milestone Billing Using Saved Searches {#bridgehead_N1206649}

Create a saved search and add it to your dashboard to keep track of billing milestones for your projects. This way, you don't have to open each billing schedule to check the status of project milestones and billing. For example, you can create a saved search to track uncompleted milestones and late milestones directly on your dashboard. Or you can display a list of milestones for all projects by expected completion date.

To create a search to filter projects by billing milestones, select the appropriate milestone billing fields when setting up an advanced search for projects. Billing milestone fields exposed as related record fields in the Project search criteria include:

-   Actual Completion Date
    
-   Amount
    
-   Comments
    
-   Estimated Completion Date
    
-   Project Task
    
-   Terms
    

Then publish the saved search to your dashboard. For information, see [Defining an Advanced Search](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N646177.html) and [Displaying Saved Search Results in Dashboard Portlets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N690632.html).

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Creating a Milestone Billing Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207171.html)
-   [Billing Customers Using Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207490.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
