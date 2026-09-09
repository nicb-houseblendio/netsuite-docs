---
id: "section_N1185988"
type: "section"
title: "Creating Projects from Sales Transactions"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Using Project Management > Creating Projects from Sales Transactions"
parent: "chapter_N1179876"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1185988.html"
anchors: []
sha256: "78ed240c8a00fd554205bf5e5eefc4755268a4361fda642cda655c91e57ef86e"
---

When you use Project Management and sell service items that are tagged to create projects automatically, use the Create Projects from Sales Transactions page to bulk create these projects.

Important:

You need the Create Projects from Sales Transactions permission to create projects from sales transactions. Roles with this permission can create projects from sales transactions using templates without requiring the individual permissions for each project element. Add the Create Projects from Sales Transactions permission to any role you want to be able to create projects in bulk.

For more information about setting up items to create projects automatically, read [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html).

Note:

The Consolidate Projects on Sales Transactions preference affects how projects are created using this method. For details, read [Using the Project Consolidation Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186943.html).

#### To create projects from sales transactions:

1.  Go to _Transactions > Customers > Create Projects From Sales Orders_.
    
    Sales orders, opportunities, and estimates appear in this list if they include items that are tagged to create projects but aren't yet associated with a project and aren't in one of the following statuses:
    
    -   Canceled
        
    -   Closed
        
    -   Pending Approval
        
2.  Check the **Create Projects** box next to each transaction you want to create a project for.
    
3.  In the **Project Name** field, the name defaults from the Project ID on the project record. You can enter a different name.
    
4.  In the **Project Template** field, if a project template is selected on the service item, the default template is selected. You can select a different template.
    
5.  Select a parent project, if applicable. The **Parent Project** dropdown appears only if other projects exist for the customer.
    
6.  In the **Project Manager** field, you can select a manager for this project.
    
    Note:
    
    Only entities marked as project resources on the Human Resources subtab of employee and vendor records appear in the Project Manager dropdown. For more information, see [Identifying an Employee as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188347.html) and [Identifying a Vendor as a Project Resource](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1188644.html).
    
7.  Click **Submit**.
    

When you submit this form, new project records are created for the service items on these transactions.

These projects default to show the primary contact from the customer on the sales transaction. The start date of the project defaults to the start date of the sales transaction.

### Related Topics:

-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating a Project Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1183012.html)
-   [Setting a Service Item to Create a Project](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186612.html)
-   [Working with Resources in Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1187445.html)
-   [Identifying Parent Tasks](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1199176.html)
-   [Managing Time and Expenses for Project Resources](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1190979.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
