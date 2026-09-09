---
id: "section_N1752091"
type: "section"
title: "Associating a Revenue Recognition Forecast Template with a Project"
branch: "revenue-and-expense-recognition"
category: "accounting"
breadcrumb: "Accounting > Revenue and Expense Recognition > Using Sales Order Revenue Forecasting > Forecasting Project Revenue > Associating a Revenue Recognition Forecast Template with a Project"
parent: "section_N1751957"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1752091.html"
anchors: ["procedure_N1752114", "procedure_N1752170"]
sha256: "835564c0ae9e64f39a5b372b0982e92d26fae2a4439e836e800f17cb9bdb6a38"
---

To create a sales order forecast for a project, you must link a revenue recognition forecast template with a project and set the Estimated End Date or Actual End Date on the job record. The Calculated End Date that appears on the Standard Job Form isn't used for revenue forecasts. To add fields for estimated or actual end dates, you customize the job form.

The Sales Order Revenue Forecasting and Project Management features must both be enabled.

#### To add an end date to a custom job form:

1.  Go to _Lists > Relationships > Jobs > New_.
    
2.  Go to **Customize** in the upper right of the page, and select **Customize Form**.
    
3.  Type a **Name** for the custom form, and click the **Fields** subtab.
    
4.  Check the box in the **Show** column for either **Projected End Date** or **End Date**.
    
5.  Clear the box for **Calculated End Date**, and click **Save**.
    
    This adds a **Custom Form** field to the Job page so you can select which form to use for a project. When you're using project planned time entries, you can select the Standard Job Form.
    

#### To associate a template with a project: {#procedure_N1752114}

1.  Go to _Lists > Relationships > Jobs_.
    
2.  Click **Edit** next to the project.
    
3.  On the project record, verify that the **Start Date** and **Estimated End Date** are entered.
    
4.  Click the **Financial** subtab.
    
5.  In the **Rev Rec Forecast Template** field, select the template to associate with this project.
    
    The template selected in this field is used to forecast revenue for the project.
    
    If the value selected in the **Billing Type** field is **Fixed Bid, Milestone**, some revenue recognition templates may not be suitable. Don't select a template that has either of these term sources: Billing Schedule, Transaction Date on Sales Order or Billing Schedule, Rev Rec Date on Sales Order.
    
6.  Click **Save**.
    

## To create a private forecast template: {#procedure_N1752170}

You can now create a private revenue recognition forecast template on a project that is specific to that project only.

-   When a project uses a **private** revenue recognition forecast template, you can modify the forecast template and affect the forecast for that specific project only.
    
-   When changes are made to **public** templates, all projects associated with the template are affected if you mass update the schedules.
    

On a project record, click the ![New icon, which looks like a plus sign](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Accounting/RevenueExpenseRecognition/AddNew.png) icon next to the Rev Rec Forecast Template field to create a new template in a new window. On the template, select one of the following:

-   Check the **Public** box to allow this forecast template to be used on any project. A public template appears on all projects.
    
-   Clear the **Private** box to limit use of this forecast template to this project. A private template appears only on the project from which it's created.
    

You can also opt to use an existing public template. For more information about creating revenue recognition templates, read [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html).

For a forecast schedule to be created for a project, all of the following conditions must be met:

-   A project must be associated with the sales order, either in the header or on individual lines.
    
-   Applicable sales order lines must be associated with variable revenue recognition templates.
    
-   The associated project must have a template specified in the Rev Rec Forecast Template field.
    
-   Both a start date and end date must be set on the project. These are the dates used for revenue forecasting, not the start and end dates entered on the sales order.
    

When these conditions are met, a revenue recognition schedule is created and appears only on sales order forecast reports. These schedules are non-posting and don't affect your general ledger.

### Related Topics

-   [Using Revenue Recognition](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1678106.html)
-   [Using Sales Order Revenue Forecasting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1750747.html)
-   [Forecasting Project Revenue](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1751957.html)
-   [Using Project Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1179876.html)
-   [Creating Revenue Recognition Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1679446.html)
-   [Working with Revenue Recognition Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1689004.html)
-   [Sales Order Revenue Forecast Summary Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1700969.html)
-   [Sales Order Revenue Forecast Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1701383.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
