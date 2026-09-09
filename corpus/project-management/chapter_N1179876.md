---
id: "chapter_N1179876"
type: "chapter"
title: "Using Project Management"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management"
parent: "part_3746040281"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html"
anchors: ["bridgehead_N1179930", "bridgehead_0405020100", "bridgehead_4532423110", "bridgehead_3745092865", "bridgehead_3898925217", "bridgehead_159541348286", "bridgehead_N1179996", "bridgehead_3735731090", "bridgehead_3898923829", "bridgehead_N1180061", "bridgehead_N1180158", "bridgehead_N1180231", "bridgehead_N1180277", "bridgehead_N1182101"]
sha256: "1b279704cabc2aa3c131c51baf9a3f0904284af54d09d917d4a626793c2a8c8d"
---

With Project Management, you get everything from the basic Projects feature, and more. To get started, this topic will help familiarize you with ways to get the maximum use from Project Management.

Project management records are created and tracked separate from customer records. However, you can associate projects with customers by selecting the customer on the project record.

You can create project management records manually or have them made automatically from service items. Read [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html) and [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html).

## Project Records as a Workspace {#bridgehead_N1179930}

Project management records function as a workspace and help you with each step of the project management workflow, from the earliest planning stages to the final tasks and customer billing. With all your data and transactions processed in one place, the project information is always accurate and up to date.

When you create a project record, you create a place to organize data based on information from your customer, ideally from the opportunity record.

The Project Manager field is in the header area of the project record, making it clear who's in charge of the project.

As you enter project task records, a project schedule is created on the Schedule subtab of the project record. The project schedule is the heart of the project workspace, where you can assess and process many aspects of the project as it moves forward. From the Schedule subtab, you can add new tasks, edit tasks and set up task hierarchies to organize project work phases. For more information, see [Working with the Project Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html).

When you are done [Setting a Project Baseline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202427.html), work can start and time is entered against project tasks. Then, you can view a [Gantt Chart](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html#bridgehead_N1202133) that compares actual progress against your original baseline goals. Using the Gantt Chart you can view your projects critical path and if time or costs are running over for the project, you can make adjustments accordingly.

NetSuite calculates the actual work spent on the project and the remaining work. The Percent Time Complete field calculates how much of the project is finished and the Estimated Labor Cost field calculates your labor investment for the project. Labor costs estimates are based on the time budget and labor rates for resources assigned to project tasks.

After you create a project record, you can link the project to the appropriate opportunity record. This keeps your items and records in sync during the project. Read [Refreshing Project Items on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204541.html).

## Project Plan Recalculation {#bridgehead_0405020100}

Project plan recalculation helps you track what projects or timesheets are awaiting to be recalculated. You can find the project recalculation information in the Project Plan subsection of the System Information tab. It shows the project plan recalculation data, such as:

-   the last project plan recalculation date and time
    
-   if the project plan is being recalculated
    
-   last project plan recalculation time
    
-   average project plan recalculation time
    
-   project plan recalculation triggers.
    

The System Information tab shows the System Notes subtab, which shows what's changed during recalculation.

Here is a list of the project plan recalculation triggers:

-   Manual trigger - You can trigger this project plan recalculation manually.
    
-   Project task modification
    
    -   If a project task has been created, updated, deleted, or imported.
        
    -   You can import project tasks at Activities > Scheduling > Project Tasks > Import.
        
-   Task modification
    
    -   If a task has been created, updated, or deleted.
        
    -   You can create a project task at Activities > Scheduling > Project Tasks > New.
        
-   Project modification
    
    -   If a project has been created, updated, deleted, or imported.
        
    -   To can access the project record at Lists > Relationships > Jobs.
        
-   Customer modification, if the customer assigned to the project has been changed.
    
-   Employee timesheet modification, if an employee's timesheet has been created, updated, or deleted.
    
-   Employee time entry modification, if an employee's time entry has been created, updated, or deleted.
    
-   Employee time record modification, if an employee's time record has been created, updated, or deleted.
    
-   Planned Work feature modification, if the Planned Work feature has been changed.
    
-   Employee's resource allocation modification, if an employee's resource allocation has been created, updated, or deleted.
    
-   Resource allocation modification
    
    -   If the Resource Allocation feature has been enabled or disabled.
        
    -   You can access the resource allocation record at Activities > Scheduling > Resource Allocations.
        

### Asynchronous Project Plan Recalculation {#bridgehead_4532423110}

You can enable a preference allowing your project plans to recalculate in the background:

-   when time is tracked against that project
    
-   if you don't use the Planned Work feature, when you approve time off for your employee
    

When you don't use the Planned Work feature, enabling the Asynchronous Project Plan Recalculation preference can speed up the time-off approval process for an employee assigned to your project since the project plan recalculates with this time-off approval. This is especially useful for large projects with many tasks, charge rules, or assignees. If you do use the Planned Work feature, approving time off doesn't affect project plan recalculation.

When project plans recalculate asynchronously, you can still use NetSuite and your project plans.

Note:

Because recalculations are asynchronous, project plan data may be out of date if you access them before the recalculations are complete.

When recalculation finishes, you'll see the updated project plan the next time you open it. If recalculation fails, you'll get a warning at the top of the project when you open it.

To enable the preference, go to _Setup > Company > General Preferences_. Check the Asynchronous Project Plan Recalculation box, and click Save.

## Project Center {#bridgehead_3745092865}

With Project Management, you can assign project resources a standard Consultant role with access to the Project Center. The Project Center gives them a special NetSuite interface with the most important project tools right on the home page.

The Project Center has the following tabs: Home, Activities, Projects, Time & Expenses, Reports, Documents, and Support. Each tab offers access to links and information that deal directly with project management in NetSuite.

For information about giving access to employees, see [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html).

## Project Dashboard {#bridgehead_3898925217}

Similar to your main NetSuite Home dashboard, you can also access a project dashboard with information specific to an individual project.

The project dashboard offers portlets and quick links for creating project tasks, managing resources, viewing the Gantt chart, and entering time and expenses.

There are visual indicators to quickly give you an idea of the project's status. You can view a list of project tasks and resource allocations directly from the Project Dashboard. You can also view the Project Manager role.

You can customize the dashboard with additional standard and custom portlets and rearrange how they appear by clicking Personalize Dashboard at the top of the page.

To view a project's dashboard, click the Dashboard icon at the top of the project record or in the Projects list. For more information, see [Project Dashboard](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3900008958.html).

## Project Indicators {#bridgehead_159541348286}

On the project dashboard, the Project Indicators portlet shows you the project's status, any changes or issues, and required actions. It has three types of notifications:

-   **Expense To Approve** notifies you about unapproved expense lines against the project. Each color represents how many unapproved expense lines need resolving:
    
    -   Red - 5 or more expense lines
        
    -   Yellow - from 1 to 5 expense lines
        
    -   Green - no unapproved expense lines
        
-   **Time Not Tracked** notifies you about untracked planned time. Each color represents the percentage of already tracked time replaced by actual hours against the planned time:
    
    -   Red - 0% to 49% of planned time
        
    -   Yellow - 50% to 99% of planned time
        
    -   Green - all planned time was tracked
        
-   **Time To Approve** notifies you about unapproved time entries against the project. Each color represents how many unapproved time entries need resolving:
    
    -   Red - 10 or more unapproved time entries
        
    -   Yellow - from 1 to 9 unapproved time entries
        
    -   Green - no unapproved time entries
        

Project Indicators portlet always gathers data from last week. For example, if you submit new expense lines on Tuesday, they won't be taken into consideration on Wednesday of the same week, but instead can be approved by the start of the next week.

Note:

You can also access the Project Indicators from the subtab on the project record.

## Project Tasks and Task Hierarchies {#bridgehead_N1179996}

Create a project task record to track every activity you need to finish for each project. Project tasks are the individual steps you need to complete to reach your goal. For example, a project might have a Consultation task and an Installation task. The Installation task could have its own set of subtasks that define work required to complete the installation.

[Creating a Project Task Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1194983.html) and setting up hierarchies helps you organize, plan, and work on the project. Project tasks outline what needs to be done, who's doing it, and the order to do the work.

For each project task, enter start dates using the Fixed Start or As Soon As Possible constraint. NetSuite automatically calculates the end date for each project task based on the estimated work, the work calendar, and each resource's availability. A scheduling algorithm uses task duration combined with the predecessor relationships (Finish-to-Start, Start-to-Start, Start-to-Finish, or Finish-to-Finish) and constraints of other project tasks to calculate the project schedule.

Parent tasks organize the hierarchy of work tasks that are subordinate to other tasks required to complete a project. For example, to define an installation task that is composed of 3 individual tasks, you can set up task records as follows:

1.  Create a task record for the installation. This task becomes the parent task after you identify it as the parent of other tasks.
    
    Note:
    
    You don't have to assign resources or estimate work for a parent task. Its estimated work is the total of its child tasks, plus any estimated work you add to the parent task. If you don't enter an assignee or estimated work, the parent task is first saved as a milestone and turns into a parent task when you add subtasks.
    
2.  Enter a work task for each of the three individual tasks. Identify each as a subordinate, or child, of the installation parent task.
    

## Milestones {#bridgehead_3735731090}

Project milestones mark key points in your project, like finishing a group of tasks, or serve as a project health check to determine if you're on schedule.

Project milestones can't have estimated hours, assignees, or a Finish No Later Than (FNLT) constraint. When viewing a project Gantt chart or schedule, milestone tasks look different from regular project tasks.

## Project Templates {#bridgehead_3898923829}

Project templates let you create project records in NetSuite for projects you do repeatedly. You can include as much or as little detail as you like in your templates. Templates offer your project managers a standardized starting point when planning projects. For more information, see [Project Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3897375321.html).

## Resource Assignment {#bridgehead_N1180061}

When you mark employees and vendors as project resources, you can assign them to project tasks. Assign resources to projects to designate who should do the work for each task.

You can also select a project resource as the project manager on your project records. In the Primary Information section of the default entry form, there's a Project Manager field that clearly identifies who's in charge.

You must first mark a project resource as a project manager on their employee record before you update the project record. You can designate any project resource as a project manager by checking the Project Manager box on the Human Resource subtab of the employee's record.

[Assigning Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html) can be done in one or two steps depending on whether you are:

-   [Assigning Resources Restricted to the Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html#bridgehead_N1189256)
    
-   [Assigning Resources not Restricted to the Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html#bridgehead_N1189443)
    

When you assign resources to tasks, you can select service items to define the services to be provided during the task. For time and materials projects, these service items are included in transactions such as estimates and sales orders, and as work is done, they are billed on the invoice.

If you enter a labor rate for each resource, you can calculate resource profitability on projects. Project costs are sourced from the resource assignment rows. The work cost designated for the task comes from each resource record. The price comes from the service item and respects customer price levels as well as employee billing classes. The projected cost and revenue for all tasks combine to produce the total expected cost and revenue for the entire project.

You can also choose to restrict time entry to only resources assigned to the project. Read [Restricting Time Entry on Project Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1192197.html).

You can use the NetSuite Project Task Manager to manage project resources and tasks. For more information, see [Project Task Manager](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1214895.html).

If you use Resource Allocations, you must first allocate resources to your project before they can be assigned to tasks. For more information, see [Resource Allocations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3746701142.html).

## Project Billing {#bridgehead_N1180158}

[Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html) for orders is based on [Project Billing Schedule Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html#bridgehead_N1205076). The billing schedule type specified on the project determines the type of project:

-   **Fixed Bid, Interval** projects bill customers for a currency amount that is determined and agreed to before the project begins. The amount billed does not change over time as the project progresses. Materials and expenses can be added to invoices for these projects.
    
-   **Fixed Bid, Milestone** projects bill customers for projects in increments based on preset milestone goals. When a milestone is reached, the services associated with the milestone are eligible to be billed to the customer.
    
-   **Time and Materials** projects are billed based on the materials and resources used to complete the project and the amount of time required to complete the project. The final amount billed may change over the course of time and isn't determined before project work begins.
    

When you first define a project, depending on the type of project, you can create a project-specific billing schedule or select an existing billing schedule.The billing schedule you choose transfers to the project's associated transactions (estimates, sales orders), creates a billing forecast, and determines billing dates for service items. When an order includes work that has been completed and is ready for billing, that order automatically shows in the bulk billing queue or displays the Next Bill button on the sales order form.

The project record also gives the project manager financial data about the expected margin, based on the project plan. Having an understanding of the expected profitability at the beginning of the project helps you decide if the margin is sufficient when considering the risk for the project. If a project requires a minimum gross profit percentage, you can monitor the percentage throughout the project to maintain that goal.

## Forecasting Project Billings {#bridgehead_N1180231}

When a project uses a Time and Materials or Fixed Bid schedule, that billing schedule is applied to the associated estimate or sales order. Then you can use billing schedules for [Forecasting Project Billings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205824.html).

Billing forecasts are generated based on the planned effort across the planned project billing interval to determine when you expect currency to be billed.

Service items across the project tasks are sourced to provide a summary of quantity, cost, and revenue for the project. Then, this information is used to calculate the gross margin for the project.

Projected billings associated with a project are included in financial forecast reports. The forecast adjusts automatically based on actual work performed and any changes made to the schedule.

You can examine billing forecast data using project billing schedules, sales order reports, the History subtab on sales order transactions and the [Estimated Profitability by Project Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1211881.html).

## Creating Estimates and Sales Orders from Projects {#bridgehead_N1180277}

After you set up a project, [Generating an Estimate from a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187267.html) pulls the information from the project record to create an estimate. You can generate multiple estimates over time to reflect changes and refinements based on customer feedback.

Check or clear the Available in Customer Center box on estimates to determine whether they show to customers in the Customer Center.

When the project detail is finalized, the next step is [Creating Sales Orders from Projects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204698.html). When you create a sales order directly from the project, the pricing and billing information carries over from the final estimate, which originates from the linked project record.

## Creating Projects from Service Items {#bridgehead_N1182101}

Alternately, your process can use [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html). In this process, the service item is tagged to create a new project record automatically each time you sell it.

For example, set the item Deluxe Widget Installation to automatically generate a project by checking the Create Project box on its record. Then, each time you sell a Deluxe Widget Installation, a project record is created that lists the tasks that installers must complete for each sale of this item.

Note:

Projects created from sales orders don't automatically leverage the functionality associated with billing types. You also can't refresh items on the transactions with changes made on the project record.

### Related Topics:

-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html)
-   [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Forecasting Project Billings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205824.html)
-   [Project Risk Forecast](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158926773024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
