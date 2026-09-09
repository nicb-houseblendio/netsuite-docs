---
id: "section_N1205308"
type: "section"
title: "Billing and Project Consolidation"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Billing and Project Consolidation"
parent: "section_N1204906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205308.html"
anchors: ["bridgehead_N1205340", "bridgehead_N1205359", "bridgehead_N1205394", "procedure_N1205411", "bridgehead_N1205459"]
sha256: "1636b29c9aaaa46f96a0d2337187e282279f28c5ad36aa07f1db3a7cfe772f5a"
---

Consider the following points when using billing schedules with the Consolidate Projects on Sales Transactions preference. For more details on the consolidation preference, read [Using the Project Consolidation Preference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1186943.html).

## Billing Schedule Types and Consolidation {#bridgehead_N1205340}

You can edit billing schedules on the project sales order. With the Consolidate Projects on Sales Transactions preference disabled, the standard sales order form includes a billing schedule field. When you select the customer and project on the sales order form, the billing schedule associated with the project autofills the billing schedule field.

Important:

Because you can change the billing schedule associated with a project when creating a sales order, it's possible to assign a fixed bid billing schedule to a time and materials project, or a time and materials billing schedule to a fixed bid project. Verify that the schedule type is the same on the project and its sales order before billing.

## Project and Sales Order Schedule Synchronization {#bridgehead_N1205359}

On a sales order, if the billing schedule is set at the header level, there's only one schedule for the entire order. If there are multiple projects on the sales order, then each of the projects could have a different billing schedule specified on the project record.

In this case, the header-level billing schedule takes precedence over the project-level billing schedules and is used for all projects. This result can be confusing because the information about the individual projects may not be the same as the billing schedule on the sales order.

To avoid this confusion, if you enable Consolidated Projects on Sales Transactions preference, use a sales order form with line-level billing schedules. That way, when you add project items to the sales order, each item brings its project's billing schedule, so the billing schedule on the sales order and the project match.

For more information, see [To customize a sales order form for per-line billing schedules:](#procedure_N1205411)

It's also important to determine billing schedules for estimates and sales orders at the same level. For example, if an estimate uses a header-level billing schedule, the sales order should also.

## Fixed Bid, Milestone Project Billing with Consolidation {#bridgehead_N1205394}

If you have the Consolidate Projects on Sales Transactions preference enabled, you must customize the standard sales order form to show billing schedules on item lines to bill Fixed Bid, Milestone projects.

For example, if you select a project with a Fixed Bid, Milestone billing schedule on the Items subtab and click Refresh, NetSuite adds the service items to the sales order, but the header-level Billing Schedule field stays blank. To bill this type of project, follow the steps below to customize the sales order.

#### To customize a sales order form for per-line billing schedules: {#procedure_N1205411}

1.  Open the standard sales order you need to customize.
    
2.  Click **Customize**.
    
3.  Click the **Screen Fields** subtab.
    
4.  On the **Columns** subtab, check the **Billing Schedule** box.
    
5.  Click **Save**.
    
    Then, when you use the customized form to create a sales order, the billing schedule for each line item defaults to the billing schedule identified on the project, if any.
    

## Fixed Bid, Milestone Billing without Consolidation {#bridgehead_N1205459}

If you disable the Consolidate Projects on Sales Transactions preference, always verify that the schedule selected on the project and sales order match.

For example, if you set a Fixed Bid, Milestone schedule on the project but select a standard schedule on the sales order, you might expect milestones to be billed. But they won't be, because the sales order schedule takes over.

If you select a project-based billing schedule (Time and Materials, Fixed Bid, Interval, or Fixed Bid, Milestone) on the sales order, all line items for the order will be invoiced based on the project billing schedule whether they are project items or not.

For example, if you use a Fixed Bid, Milestone schedule from a project on the sales order, and then add non-inventory items, those items will be billed using the same milestone percentages as the project's service items.

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Project Billing Rates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205608.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
