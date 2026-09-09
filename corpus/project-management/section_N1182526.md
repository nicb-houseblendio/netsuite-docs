---
id: "section_N1182526"
type: "section"
title: "Project Management Records"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Project Management Records"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182526.html"
anchors: ["subsect_156296935424", "bridgehead_N1182554", "bridgehead_N1182592", "bridgehead_N1182615", "bridgehead_N1182646", "bridgehead_N1182667", "bridgehead_N1182679", "procedure_N1182691"]
sha256: "973ac3d917b754507e1d2256a8429982bdc34c85b6556d8bb99edac53bf340f8"
---

With Project Management, you can use project records to track everything about your projects from start to finish.

By setting up data for each project in an organized manner, you can maintain and access information when you need it, as well as use the data to update schedules and generate transactions or reports that help you track your project's progress.

When you maintain accurate information for each project record, you are better able to accomplish goals not only for the one project, but for all company projects. Since you often have to split limited resources across projects, having up-to-date information makes it easier to balance margins and risks.

Important:

You should break up long, multi-year projects into smaller parts to improve performance when working with project records.

## Project Scheduling Methods {#subsect_156296935424}

When you first create a project record, even if you don't have all the details yet, you can enter the project name, status, and perhaps the start and end dates. As the project moves forward, the record becomes your workspace where you can manage details.

As you begin planning your project, you must decide the best method to create your project schedule. NetSuite offers two methods for project scheduling, forward and backward.

Important:

The Planned Work feature is required for backward project scheduling. For more information, see [Planned Work](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530301667.html).

Forward scheduling lets you define a start date for your project and schedule tasks from there. NetSuite uses the start date, task order, durations, and lag time to calculate an estimated end date for your project. Forward planning works best when you know exactly when your project needs to start.

Backward scheduling lets you define an end date for your project and schedule tasks backward based on the end date. NetSuite uses the end date, task order, durations, and lag time to calculate an estimated start date for your project. Backward planning works best when you have a hard deadline for finishing your project.

As data is available, you can also do the following on the project record to define and refine the project:

## Schedule subtab {#bridgehead_N1182554}

On the schedule subtab of project records, you can identify and schedule necessary work tasks. After tasks are created, you can see various basic or customizable views of the tasks, also known as a project plan. A [Gantt Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html#bridgehead_N1202133) view is also available. The project plan helps you plan, manage, and run your project schedule. For more information, see [Working with the Project Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html).

Note:

The Schedule subtab only appears after you save a project record. It lists project tasks in the same order as the project plan, and you can't sort or reorder tasks from the Schedule subtab.

## Resources subtab {#bridgehead_N1182592}

On the Resources subtab, you can assign the resources needed to complete project tasks and designate their role on the project. You can select multiple roles for a single resource. To price and schedule resources, you need to select resources on specific task records. Read [Assigning Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html).

If you use Resource Allocations, you must first allocate resources to your project before they can be assigned to tasks. For more information, see [Resource Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html).

## Financial subtab {#bridgehead_N1182615}

On the Financial subtab, you can define the project billing behavior by selecting a billing type and billing schedule, if you use Advanced Billing. The Financial subtab provides labor data for estimated, actual, and remaining work, as well as the percent of the project completed based on labor hours. You'll also see estimated costs, revenue, and profits. Lastly, you can find the revenue recognition plans related to the project on this subtab.

## Preferences subtab {#bridgehead_N1182646}

On the Preferences subtab, choose settings for time and expense preferences related to the project. You can let anyone enter time or limit time entry to assigned resources only. Classify project time entries as utilized, productive or exempt to customize utilization calculations. You can also choose to allow expense entries and to create planned time entries. If you use NetSuite OneWorld, you can select a subsidiary for the project. For more information, see [Working with Project Management in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182865.html).

## Related Records subtab {#bridgehead_N1182667}

The Related Records subtab contains most of the same basic information found on Related Records subtabs on records throughout NetSuite, such as information about contacts and partners.

## Communication subtab {#bridgehead_N1182679}

The Communication subtab is where you can attach and send messages and schedule phone calls. You can also link projects with opportunities so that project items can be included in estimates and sales orders and billed along with other sales items.

The following workflow is the best practice for incorporating projects into the sales process.

Note:

This specific workflow is possible only if you don't enable the Consolidate Projects on Sales Transactions preference. For more information, read [Using the Project Consolidation Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186943.html).

#### Best Practice: Incorporate the Project Record into your Sales Process {#procedure_N1182691}

1.  Create an opportunity for a prospect.
    
    On the **Items** subtab of the opportunity form, add all non-project items. This is any items except service items. Project items, or service items, are derived from the project record.
    
    If you'd rather, you can wait to add non-project items on the estimate.
    
    For more information, see [Opportunity Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1066171.html).
    
2.  Set up the project by creating a project record.
    
    From within the project record, add and manage service items related to the opportunity, create project tasks, and define the billing type.
    
    For more information, read [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html).
    
3.  Link the project to the opportunity.
    
    After you create a project record, you can link the opportunity record to the project by selecting the project on the opportunity.
    
    When you connect a project to an opportunity, the project items automatically source into the transaction rows of the opportunity record. These rows can't be edited on the opportunity but you can remove them. To make changes, update the project record first, then reopen the opportunity to refresh the items. Read [Refreshing Project Items on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204541.html).
    
    For information, read [Linking a Project to an Opportunity](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187364.html).
    
4.  Generate one or more estimates from the opportunity.
    
    An estimate created from a linked opportunity merges the non-inventory and other items with the service items for the project.
    
    Note:
    
    If you create an estimate from the project record, it only includes service items from the project.
    
    For more information, read [Generating an Estimate from a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187267.html).
    
5.  Create a sales order from a project estimate.
    

### Related Topics:

-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html)
-   [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Planned Work](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530301667.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
