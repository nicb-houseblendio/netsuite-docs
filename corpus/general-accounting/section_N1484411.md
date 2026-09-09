---
id: "section_N1484411"
type: "section"
title: "Creating Expense Allocation Journal Entries"
branch: "general-accounting"
category: "accounting"
breadcrumb: "Accounting > General Accounting > Journal Entries > Expense Allocation Overview > Creating Expense Allocation Journal Entries"
parent: "section_N1483457"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484411.html"
anchors: ["procedure_N1484430", "procedure_N1484513"]
sha256: "cd609873b19e9c753a418516497366a66c0340a077c282ed0ac6ad2d85bb7164"
---

Allocation schedules are used to generate journal entries that distribute expenses to the appropriate accounts, departments, classes, and locations.

Dynamic allocation schedules calculate the weight of a statistical account through statistical journal entries or as an absolute value at the time the allocation journal is created. This is useful in advanced costing such as Activity Based Costing and Usage Based Costing, and when you're running cost centers and profit centers. For more information, see [Working with Allocation Schedules Weighted by the Balance of a Statistical Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_3866895958.html)

Important:

Your user role must have Edit or Full level of the Create Allocation Schedules permission to use Expense Allocation.

Note:

Journal entries created by allocation schedules can't trigger User Event scripts.

#### To create an allocation journal entry from an allocation schedule: {#procedure_N1484430}

1.  Go to _Transactions > Financial > Create Allocation Schedules > List_.
    
2.  Click **View** next to an allocation that is due.
    
3.  On the allocation schedule, click **Create Journal Entry**.
    
    The Journal Entry record opens in View mode.
    
    -   If the **Require Approvals on Journal Entries** accounting preference hasn't been enabled, you can click **Edit**, then **Save**, to post the journal entry.
        
    -   If the **Require Approvals on Journal Entries** accounting preference has been enabled, and you have journal approval permission, you can click **Approve** to post the journal entry. If you don't have this permission, you can view the journal entry.
        
    -   If you've enabled the **Journal Entries** accounting preference, the **Approval Status** and **Next Approver** lists appear. Custom buttons that perform various commands may also appear enabled or unavailable, depending on your workflow configuration. For information about a custom journal entry approval workflow, see [Using SuiteFlow for Journal Entry Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4643662034.html).
        
    -   This preference is available at _Setup > Accounting > Preferences > Accounting Preferences_, on the General subtab, under General Ledger.
        

If you've enabled the Allocation Schedules Due reminder on your dashboard, you can click the reminder to view a list of allocations that are due.

#### To enable the Allocation Schedules Due reminder: {#procedure_N1484513}

1.  On the Home page, click **Personalize**. The **Personalize Dashboard** palette opens.
    
2.  On the **Standard Content** tab of the **Personalize Dashboard** palette, click or drag and drop **Reminders**.
    
3.  In the Reminders portlet, click the ellipsis icon and select the **Set Up** link.
    
4.  In the Select Reminders dialog, click or drag the **Allocation Schedules due** box.
    
5.  Click **Save**.
    

If you need to alter an individual allocation, click **Add Custom Allocation** on the **History** subtab of an Allocation Schedule record.

### Related Topics

-   [Expense Allocation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483457.html)
-   [Creating Expense Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1483674.html)
-   [Creating Intercompany Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1484654.html)
-   [Viewing the Details of Allocation Schedules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869578910.html)
-   [Expense Allocation Assignment to Projects and Entities](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1485952.html)
-   [Creating an Allocation Batch](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3867806074.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
