---
id: "section_N1207171"
type: "section"
title: "Creating a Milestone Billing Schedule"
branch: "project-management"
category: "projects"
breadcrumb: "Projects > Project Management > Project Billing > Projects and Milestone Billing > Creating a Milestone Billing Schedule"
parent: "section_N1206555"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207171.html"
anchors: []
sha256: "fa0b766b88c3a79a42c57f0bfbf449adb3fdd4fd028e53193cd4eb4625c5a13a"
---

If you use both the Project Management and Advanced Billing features, you can use milestone billing to bill customers in increments when project milestones are reached. For more information, see [Billing Customers Using Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207490.html).

To enable the features required to use milestone billing, see [Enabling Project Features](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4740572949.html).

To use milestone billing, you must create a milestone billing schedule from inside the project. The schedule identifies the amount to bill as milestones are completed. Each milestone billing project has its own Fixed Bid, Milestone billing schedule.

Note:

Milestone billing schedules can't be made public.

#### To create a milestone billing schedule:

1.  Go to Lists > Relationships > Projects. Click **Edit** next to the project you want to create a schedule for.
    
2.  Click the **Financial** subtab.
    
3.  On the **Financial** subtab, select **Fixed Bid, Milestone** in the **Billing Type** field.
    
    ![NewBillingSchedMilestone](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/NewBillingSchedMilestone.png)
4.  On the billing schedule form, enter a name for this billing schedule.
    
5.  NetSuite fills in the Initial Amount and updates it automatically as you add billing milestones. If the total percentage amount for all milestones is less than 100%, then the remaining percentage is the initial amount to be billed.
    
6.  In the **Initial Payment Terms** field, select the terms to be used on the first invoice to be created from the sales order.
    
    To add new payment terms, go to _Setup > Accounting > Accounting Lists > New_. Select **Term**.
    
7.  Add a line for each milestone to be billed by this schedule.
    
    1.  In the **Amount** field, enter the percentage of the total project amount to be billed when the milestone is reached.
        
    2.  Optionally select payment terms to apply to this milestone.
        
    3.  Optionally, in the **Task** field, select the task that must be completed for this milestone.
        
    4.  In the **Estimated Completion** date, enter the date when you expect to reach this milestone. This is used for forecasting calculations.
        
        If you entered an estimated completion date when you created the project task, that date shows here.
        
        ![BillingSchedule\_Task](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/BillingSchedule_TaskSelect.png)
    5.  If you don't identify a project task for a milestone, then check the **Completed** box only when this milestone is completed and ready to be billed.
        
        If you specify a project task for a milestone, then NetSuite will automatically mark the milestone complete when the task is finished.
        
        Important:
        
        Milestones can't be billed unless they're marked as complete. If you don't specify a project task for the milestone, then you must check the **Completed** box manually.
        
        ![BillingSched\_Completed](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/Projects/BillingSched_Completed.png)
    6.  Optionally add comments about this milestone.
        
    7.  Click **Add**.
        
8.  Repeat step 8 for each milestone you want to add to this schedule.
    
9.  Click **Save**.
    

Each milestone billing schedule you create is private, applies only to one project, and can be viewed only from the project record. Upon completion of each milestone task, that portion of the project becomes eligible for billing.

### Related Topics

-   [Project Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1204906.html)
-   [Projects and Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1206555.html)
-   [Billing Customers Using Milestone Billing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207490.html)
-   [Project Management Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1207852.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
