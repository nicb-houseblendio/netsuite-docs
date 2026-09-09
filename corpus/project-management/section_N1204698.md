---
id: "section_N1204698"
type: "section"
title: "Creating Sales Orders from Projects"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Tracking and Managing Projects > Creating Sales Orders from Projects"
parent: "section_N1201734"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204698.html"
anchors: []
sha256: "4057cc33beb611359aaa495fe8896af04a594b3b58d0e7d09ef28897beb682d3"
---

You can create a sales order from an existing project. NetSuite creates line items on the sales order for the service items associated with the project tasks. The new sales order automatically fills in the customer, project, and items from the project schedule. You can also add extra items that aren't part of the project, like inventory, discounts, assemblies, descriptions, or subtotals.

To be able to create a sales order from a project:

-   You must select a billing schedule for the project.
    
-   Don't select the Consolidate Projects on Sales Transactions preference.
    

#### To create sales orders from a project:

1.  Open a project in **Edit** or **View** mode.
    
2.  In the **New** dropdown, click **Sales Order**. NetSuite creates a new sales order with the customer, project, and items from the project.
    
3.  Click **Save**.
    

On the sales order, the line item shows the following project information:

-   Project Item: Indicates that the line item came from the project associated with the sales order.
    
-   Billable Estimate: Displays the estimated amount of billable time for the item. This amount is included in the total amount of the sales order and represents time not yet recorded in Time Tracking for the task or tasks associated with the item. It only appears if you don't enable the Consolidate Projects on Sales Transactions feature.
    

Generally, you create a sales order a single time from a project at the point you have customer approval for the project. If the project schedule changes before invoicing the customer, then click Refresh Items from Project to update the sales order items to match the project information.

Note:

You can create sales orders at different points in the order-to-cash process. Depending on your needs, you might want to create them from opportunities or estimates instead of directly from projects.

You can add project names to sales order reports by customizing the report to include Bookings > Project > Job Name. If you use the Consolidate Projects on Sales Transactions preference, you can customize your reports to include Bookings > Entity (Line) > Name to display the project name. For more information about customizing reports, see [Report Customization](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N736328.html).

### Related Topics

-   [Viewing Project Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1201840.html)
-   [Working with the Project Schedule](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202036.html)
-   [Tracking Project Baselines and Variance](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202265.html)
-   [Setting a Project Baseline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1202427.html)
-   [Refreshing Project Items on Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204541.html)
-   [Using the Project Consolidation Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186943.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
