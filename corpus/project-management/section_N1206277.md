---
id: "section_N1206277"
type: "section"
title: "Projects and Interval Billing"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Projects and Interval Billing"
parent: "section_N1204906"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206277.html"
anchors: ["bridgehead_N1206298", "bridgehead_N1206329", "bridgehead_N1206432"]
sha256: "1eabea7875de46664e663b0d5d5947a1bad7d88fe476d21ef8ff9c916cdb858c"
---

## Fixed Bid, Interval Billing Schedules {#bridgehead_N1206298}

Fixed Bid, Interval billing schedules allow you to invoice customers at predefined intervals. This schedule type bills in arrears only. You can specify an initial amount, recurrence frequency, payment terms, and the time entry type to bill for these schedules.

Note:

You must enable Project Management and Advanced Billing to use fixed bid, interval billing.

Billing with Fixed Bid, Interval schedules is similar to using a standard billing schedule with a regular frequency. However, NetSuite calculates the number of billing cycles based on the duration of the project and the billing recurrence frequency. The percent work complete as of the bill date for each project item determines the amount billed.

Check the Invoice Actual Time Only box when creating the schedule to only bill actual time worked during the interval. Clear the box if you want to invoice both actual and planned time. If you invoice actual time only, then you can't specify an initial amount.

Because these schedules don't contain any project or order specific information, they're public by default and can be shared.

## Creating a Fixed Bid, Interval Billing Schedule {#bridgehead_N1206329}

#### To create a Fixed Bid, Interval billing schedule

1.  From the **Financial** subtab of a project record, click the **Add New** icon next to the **Billing Schedule** field.
    
2.  Enter a name for the billing schedule.
    
3.  In the **Initial Amount** field, enter the amount to bill on the first invoice created from the sales order. You can enter the amount as a currency amount or a percentage.
    
4.  In the **Initial Payment Terms** field, select the terms to be used on the first invoice to be created from the sales order.
    
    To add new payment terms, go to _Setup > Accounting > Accounting Lists > New_. Select **Term**.
    
5.  In the **Recurrence Frequency** field, select how often to create bills.
    
6.  Check **Invoice Actual Time Only** if you want to bill time worked and recorded but not planned time in each interval. You can't specify an initial amount if you bill actual time only.
    
7.  The **In Arrears** box is checked by default because all billing for fixed bid, interval projects occurs at the end of the recurrence period.
    
8.  In the **Recurrence Payment Terms** field, select the payment terms to be used on all recurring invoices.
    
9.  If you don't want this schedule to be applied to new projects, then check the **Inactive** box.
    
10.  Click **Save**.
     

## Billing Customers Using Fixed Bid, Interval Billing {#bridgehead_N1206432}

Bill customers for fixed bid, interval projects using Advanced Billing. You can:

-   Bill from the billing queue
    
-   Bill manually
    

For information about how to use the billing process, see [Billing Customers Using Billing Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1254744.html).

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Projects and Time and Materials Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1205953.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
