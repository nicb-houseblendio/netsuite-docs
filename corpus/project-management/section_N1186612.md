---
id: "section_N1186612"
type: "section"
title: "Setting a Service Item to Create a Project"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Setting a Service Item to Create a Project"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html"
anchors: []
sha256: "7eb20d9b8162ab5741f5c69a1ebdfa68bcb95aea38b5d0b2ce34782fb40e801b"
---

With Project Management, you can set up a service item to a create project each time you sell the item. This option is available for Service For Sale and Service for Resale items only. You designate a service item to create a project and identify the tasks for the project. Then, after selling the items, bulk create projects from sales transactions.

First, set up the item records for your service items.

#### Setting a service item to create a project:

1.  Go to _Lists > Accounting > Items_. Click **Edit** next to the service item.
    
2.  On the item record, click the **Related Records** subtab.
    
3.  Click the **Projects** subtab.
    
4.  Check the **Create Project** box.
    
5.  If you want to use a defined project template for projects created from this service item, select a template in the **Project Template** field.
    
6.  If you don't want to use a defined project template, you must define the tasks required to complete the project. For each task, complete the following steps:
    
    1.  In the **Task Template Name** field, enter the task name. This is the task name that appears on project records created for this item.
        
    2.  In the **Start Date Offset** field, specify the start date of the tasks relative to the project start date. For example, if the task starts two days after the project start date, enter **2**.
        
    3.  In the **Effort** (hours) field, specify the total number of hours typically required to complete this task. This number of hours is set as the initial time budget for this task on project records created for this item.
        
        Note:
        
        When you set up a task for a service for sale item, the task duration doesn't take weekends into account. For example, an 80 hour duration sets the end date 10 days after the start date.
        
    4.  Click **Add**.
        
7.  Click **Save**.
    

When you sell the item, create a project record from the Bulk Projects queue. The project includes the tasks from the template on the item record. To create project records from sales items, go to _Transactions > Customers > Create Projects_. For more information, read [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html).

To view the list of projects, go to Lists > Relationships > Projects. Click Edit next to a project in the list to open the record and assign tasks to personnel.

### Related Topics:

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
