---
id: "section_N1204906"
type: "section"
title: "Project Billing"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing"
parent: "part_3746040281"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html"
anchors: ["procedure_N1205034", "bridgehead_N1205076"]
sha256: "0bdd448300be3da672e7ef5cb7916edb7882c85858cd42b995aa6b21ab3ad537"
---

NetSuite gives you flexible options for project billing. You can bill projects when work is done, when milestones are hit, or on a set schedule. The billing type you select determines how you'll bill, and the billing schedule gives you details for when and how to bill the customer. For more on the three types of billing schedules For information about the three types of project billing schedules, read [Project Billing Schedule Types](#bridgehead_N1205076).

You must enable Project Management and Advanced Billing to bill projects.

You can create a billing schedule specific to the project or select an existing billing schedule. After a billing schedule is set on the project record, the billing schedule is associated with the sales order when you source items from the project. The rules that determine when the order is ready to bill depend on the billing schedule type.

Note:

You can use a standard billing schedule for a project if that works for you. When you create the project, select Fixed Bid, Interval as the billing type but don't select a billing schedule. Then, on the sales order, edit the project line and assign a standard billing schedule (not Fixed Bid, Interval, Fixed Bid, Milestone, or Time and Materials). The billing schedule on the sales order will override the one on the project.

When an order includes work that's already done and ready for billing, that order automatically shows in the bulk billing queue or shows the Next Bill button on the sales order form. Use the Bill Sales Order page as the primary place to invoice for project work associated with an order, including project billable time that is billed on a time and materials basis. Project time must be entered and approved to be billable.

![BillSalesOrds](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/BillSalesOrds.png)

The best practice is to create sales orders for your projects and then bill the sales orders individually or in bulk on the Bill Sales Order page. A sales order doesn't contain the Next Bill button when it's connected to an inactive project.

You shouldn't use the Invoice Billable Customers page to bill time for Time and Materials projects that have associated sales orders. That's because the invoice won't be linked to the originating order. Use the Invoice Billable Customers page to process time that isn't associated with any order.

When creating invoices, all approved, billable time entered against the project is automatically included on the invoice. The Billable Time subtab also displays approved billable time not related to a sales order, such as time entered against a case. Select any non-sales order time that you want to include on the invoice. Project totals don't include non-sales order items billed to the customer.

To bulk bill projects, go to _Transactions > Sales > Bill Sales Orders_. For details about the bulk billing process, read [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html).

For details about project billing using all billing schedule types, read [Project Billing Schedule Types](#bridgehead_N1205076).

You can view the billing schedule on the sales order by clicking the Schedule subtab under the History subtab.

## Invoice Schedule Recalculation {#procedure_N1205034}

Changes to projects, tasks, or time entries can affect sales order invoice schedules if the project has a billing schedule. These changes trigger a recalculation of both the project plan and the invoice schedule.

For example, you may have a weekly billing schedule associated with a sales order for a 2-week project. The invoice schedule lists two expected bill dates. If a project task is changed in a way that the project duration becomes 4 weeks, then the invoice schedule on the sales order also updates. The updated schedule will include four expected bill dates.

Note:

The following changes don't trigger project plan or invoice schedule recalculation:

Changes made to work calendars

Changes made to billing schedules

## Project Billing Schedule Types {#bridgehead_N1205076}

To set up billing for a project, select a billing type and billing schedule on the Financial subtab of the project record. The billing type and the billing frequency of the associated schedule determine how Advanced Billing executes project billing.

Billing types include:

-   [Projects and Time and Materials Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html) - Bill customers for project expenses, such as resource time and materials
    
-   [Fixed Bid, Interval Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206277.html#bridgehead_N1206298) - Bill customers for work completed at predefined intervals
    
-   [Fixed Bid, Milestone Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html#bridgehead_N1206607) - Bill customers based on percent of work completed, or preset milestones
    
    ![BillingTypeSelect](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/BillingTypeSelect.png)
-   [Charge-Based Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3752830510.html) - If you use Charge-Based Billing, you can set up charge rules for more flexible billing. Billing Rate Cards let you set rates for Charge-Based projects.
    

#### To enter financial information for a project record:

1.  Go to Lists > Relationships > Projects. Click **Edit** next to the project you want to enter financial information for.
    
2.  Click the **Financial** subtab on your new project record.
    
3.  Select a billing type for this project.
    
4.  Select a billing schedule for this project or select **New** to create a new schedule.
    
    For details about creating a billing schedule, read [Creating Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1252880.html) and [Creating Billing Schedules From an Estimate or Sales Order](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1253492.html).
    
5.  If you select a **Fixed Bid** type schedule, enter the following:
    
    1.  In the **Billing Item** field, select the service item that will appear on transactions billed to the customer.
        
    2.  In the **Project Price** field, enter the project price. This is the price billed to the customer on transactions. It's also used to calculate gross profit margin for the project.
        
6.  If you use the Multi-Currency feature, select a currency for this project.
    
    The **Exchange Rate** field shows the appropriate exchange rate.
    
7.  If you use the Revenue Recognition feature, in the **Rev Rec Forecast Template** field, select a revenue recognition template created for a project. It's used only to forecast the expected revenue to be recognized for the project according to the schedule.
    
8.  If you use Job Costing, in the **Project Expense Type** field, select an expense type for this project. Check the **Apply to all time entries** box to apply this project expense type to all time transactions overriding any project expense types from service items. For more information, see [Job Costing and Project Budgeting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3748436271.html).
    
9.  You can now click **Save** to save your project record.
    

### Related Topics

-   [Billing and Project Consolidation](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205308.html)
-   [Project Billing Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205608.html)
-   [Using Billing Rate Cards](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4689764278.html)
-   [Forecasting Project Billings](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205824.html)
-   [Working with Project Management in OneWorld](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1182865.html)
-   [Projects and Time and Materials Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html)
-   [Projects and Interval Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206277.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)
-   [Project Risk Forecast](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_158926773024.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
