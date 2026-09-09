---
id: "section_N1183012"
type: "section"
title: "Creating a Project Record"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Creating a Project Record"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html"
anchors: []
sha256: "1723a50c85d89a680b78721b2baefdf923465df1b9e573db1f320699a786ba03"
---

With Project Management, you can create project records to track your projects and tasks. Project records can capture basic information about your project, such as customer, start date, and status. You can add more detailed information about your project to capture financial, resource, and budget information.

Important:

You should break up long, multi-year projects into smaller parts to improve performance when working with project records.

#### To create a project record:

1.  Go to Lists > Relationships > Projects > New.
    
    You can also click **New Project** in the New menu at the top of most pages to create a new project for the current Customer.
    
2.  Under Primary Information:
    
    1.  In the **Custom Form** field, select the form you want to use to enter this record. This field only appears when you have at least one custom form. You can customize this form by clicking Customize at the top of the page.
        
    2.  The **Project ID** field displays either the ID that has been entered in the Project Name field or an auto-generated ID.
        
        -   In the **Auto** box next to Project ID, clear the box to manually enter a name for this record in the Project Name field.
            
        -   If you leave this box checked, NetSuite assigns a name or number for this record based on your settings at _Setup > Company > Auto-Generated Numbers_.
            
    3.  In the **Project Name** field, enter the project name.
        
        This name fills in the **Project ID** field unless you use auto-numbering. Enter a unique project name. If you use Auto-Generated Numbering, it is important that you enter the project name here because the Project ID doesn't include the project name.
        
    4.  If this project is associated with a customer, select them in the **Customer** field.
        
        Note:
        
        After a customer has been selected, it can't be changed on the project record when there are transactions, actual time, actual charge, child project, contact (if Company field holds a project) or personalized Rate Card associated with the project. Mentioned actions remove the Change a customer button. If you create a new project from the Actions menu at the top of an existing project, the new project record is automatically linked to the current project's customer. To change a project's customer, click the Change Customer button in View mode. You can only select a new customer that supports the same currency and subsidiary as the original customer.
        
        Note:
        
        Projects that aren't associated with a customer can't be used on transactions.
        
    5.  In the **Project Manager** field, select a project resource to be the project manager for this project. Only employees with both the Project Resource and Project Manager fields checked on the Human Resources subtab of their employee records appear in the Project Manager field selection.
        
        Project managers can approve and update time entries submitted for their assigned projects.
        
    6.  In the **Status** field, select the status that indicates the progress of the project.
        
        You can create new statuses at Setup > Accounting > Accounting Lists > New > Project Status.
        
    7.  If you use NetSuite OneWorld, select the subsidiary for this project in the **Subsidiary** field.
        
        For more information, see [Working with Project Management in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182865.html).
        
        Note:
        
        After a transaction posts for the project, you can't change the customer or subsidiary on the project record.
        
    8.  If you would like to apply a project template to this new project record, select the template in the **Project Template** field. For more information about project templates, see [Project Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3897375321.html).
        
3.  Under Project Dates, if you also use the Planned Work feature, in the **Scheduling Method** field, select **Forward** or **Backward**.
    
    -   If you know when your project needs to start, select **Forward** and enter the estimated date work will start on the project. You can change this date at any time during the project. NetSuite schedules all project tasks without predecessors to start on this date.
        
    -   If you know when your project needs to be finished, select **Backward** and enter the estimated date work must be completed. You can change this date at any time during the project. NetSuite schedules all project tasks without successors to end on this date.
        
    
    For more information about scheduling methods and planned work, see [Project Scheduling Methods](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182526.html#subsect_156296935424) and [Planned Work](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530301667.html). The rest of the Project Dates fields fill in after you save the project and add tasks.
    
4.  Click the **Financial** subtab to enter financial information about this project. For more information, see [Project Billing Schedule Types](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html#bridgehead_N1205076).
    
5.  If you use the Project Budgeting feature, click the **Budget** subtab and enter budget information for this project record. For more information, see [Creating Project Budgets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751156905.html).
    
    Note:
    
    Projects with more than 20 budget categories may run slower. It's best to add only the most common categories when setting up project budgets. For more information about selecting categories for project budgets, see [Setting Up Project Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751156538.html).
    
6.  Click the **Relationships** subtab to enter contacts for this project.
    
7.  Click the **Communication** subtab to enter phone calls, CRM tasks, events, attach files, and create user notes for this record. For more information, see [Communication](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740077129.html#bridgehead_4585951058).
    
8.  Click the **Preferences** subtab to select preferences to apply to this project. For more information, see [Setting Up Project Record Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4585905289.html).
    
9.  When you have finished, click **Save**.
    

After you save a project record, you can enter more details on the Resources and Schedule subtabs when you view or edit the project record. For more information, see [Assigning Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1189140.html) and [Working with Project Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740077129.html).

When you use Charge-Based Billing and Project Revenue Recognition, you can customize which actions are triggered by the status of your projects. These triggers are also available for custom statuses.

-   **Create Actual Charges During Midnight Run** - This box is available when you use Charge-Based Billing. Check it if you want actual charges created during the midnight run for projects with this status. For the In Progress project status, this box is checked by default.
    
-   **Create Forecast Charges During Midnight Run** - This box is available when you use Charge-Based Billing. Check it if you want forecast charges created during the midnight run for projects with this status. For the In Progress project status, this box is checked by default.
    
-   **Completely Billed** - This box is available when you use Project Revenue Recognition. Check the box to show the **Completely Billed** button at the top of a project record set to this status. Click this button to begin the project revenue reconciliation process. For the Closed project status, this box is checked by default.
    

For more information, see [Charge-Based Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752830510.html) and [Project Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4642885587.html).

### Related Topics:

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Working with Project Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3740077129.html)
-   [Creating Projects from Sales Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html)
-   [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Planned Work](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1530301667.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
