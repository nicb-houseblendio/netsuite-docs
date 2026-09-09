---
id: "section_N1205953"
type: "section"
title: "Projects and Time and Materials Billing"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Projects and Time and Materials Billing"
parent: "section_N1204906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html"
anchors: ["bridgehead_N1206023", "bridgehead_N1206139"]
sha256: "18856c0fab613a11f73a9b077853fed0c0c1ac419b6108d2cea2e0ba2d79e068"
---

Use the Time and Materials billing type to bill customers for time worked on a project and material costs. Estimates and sales orders that include project service items can be billed on a Time and Materials basis. This enables you to use the Bill Next button, Bill Sales Orders link, or the bulk Bill Sales Orders page to process billing, and to view time and materials revenue forecasts.

Another possibility is to use the Billable box. For information, see [Billing Costs to Customers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1248576.html).

Note:

You must enable Project Management and Advanced Billing to use time and materials billing.

For Time and Materials schedules, billing dates are driven by the frequency selected in the billing schedule. The number of billing dates depends on the duration of the associated project. The expected amount billed on each billing date is determined by the expected percent-complete of each project item as of the bill date.

The Items subtab on the Sales Order shows the estimated billable service items from the project. This corresponds to the entered and approved time for project task and represents the full amount of project time expected to be billed for the billing period. On the invoice, the Billables subtab displays the billable service items.

Time and materials schedule lines that won't be carried over to the invoice have the Billable Estimate field checked on the sales order. Order lines for Time and Materials project items, as indicated by the Billable Estimate flag, are automatically linked to corresponding billable time when invoiced. The Invoiced column on the sales order reflects these billable time entries.

If you use a Time and Materials schedule, you can't show an initial payment against the project because the order lines are removed when you convert the order to an invoice and there are no lines to create an initial bill against. You can, however, accept a customer deposit in this case.

There is no need to close out a sales order or the individual lines to avoid billing them inadvertently. NetSuite doesn't bill an item until time worked is entered against it and approved. Only then will billing include time for that item. If the only remaining open lines on a sales order are billable estimate lines, then the Next Bill button doesn't appear until the billable time has been entered and approved.

Sales order lines are considered billed after the customer has been invoiced for a quantity equal to or greater than the quantity specified on the order. To invoice fewer hours than the number originally specified on the order, the quantity on the order must be reduced.

Important:

On a sales order, lines associated with a Time and Materials schedule are considered to be estimated lines and those lines are removed when the order is converted to an invoice. In these cases, you must apply billable time to the invoice to generate the appropriate bill.

## Creating a Time and Materials Billing Schedule {#bridgehead_N1206023}

Use the Billing Schedule page to create a Time and Materials billing schedule. You can access this page from the Financial subtab of a project or go to _Lists > Accounting > Billing Schedules > New_.

The Time and Materials billing schedule defines the billing frequency and payment terms and always bills in arrears. You can define a time and materials billing schedule and then use it for as many projects as you want. You don't have to create a separate time and materials billing schedule each time you create a time and materials project. If you want to create private time and materials billing schedule that can only be used for one project, then you must create the billing schedule from the project record.

#### To create a Time and Materials billing schedule:

1.  From the **Financial** subtab of a project record, click the **Add New** icon next to the **Billing Schedule** field.
    
2.  Enter a name for the billing schedule.
    
3.  In the **Recurrence Frequency** field, select how often to create bills.
    
4.  The **In Arrears** box is checked by default because all billing for time and materials projects occurs at the end of the recurrence period.
    
5.  In the **Recurrence Payment Terms** field, select the payment terms to be used on all recurring invoices.
    
6.  Clear the **Public** box if you want this billing schedule to be available only for the project it was created from.
    
7.  If you don't want this schedule to be applied to new projects, then check the **Inactive** box.
    
8.  Click **Save**.
    

## Billing Customers Using Time and Materials Billing {#bridgehead_N1206139}

Bill customers for time and materials projects using Advanced Billing. You can:

-   Bill from the billing queue
    
-   Bill manually
    

For information about how to use the billing process, see [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html).

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Projects and Time and Materials Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html)
-   [Projects and Interval Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206277.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
