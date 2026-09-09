---
id: "section_N913502"
type: "section"
title: "Giving Accounting Approval for Expense Reports"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Expense Reports and Purchase Requests > Expense Reporting > Giving Accounting Approval for Expense Reports"
parent: "section_N907845"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913502.html"
anchors: ["subsect_1528469712", "subsect_156987306301", "bridgehead_N913584", "bridgehead_N913659"]
sha256: "cbbd655b6d89ba1556dbec47e1e151f9b69f7a44af67cf382525db41a4d6a2a5"
---

Expense reports have no accounting impact until they're approved by someone with accounting authority. When reports are entered, their totals remain in an unapproved non-posting account.

By default, an expense report requires approval by the employee's immediate supervisor before being sent for accounting approval. If approval routing is enabled and set up, a more complex approval hierarchy is followed. See [Approval Routing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2394992.html).

When an expense report receives accounting approval, a bill is automatically created and its amount is reflected on your books. The expense report is posted in the earliest open period, which may not be the same as the period when the expense report was entered.

The following three conditions must be met for a role to be able to give accounting approval of an expense report:

-   Use one of the following centers:
    
    -   Executive Center
        
    -   E-Commerce Management Center
        
    -   Marketing Center
        
    -   Classic Center
        
    -   Support Center
        
    -   Shipping Center
        
    -   Sales Center
        
    -   Project Center
        
    -   Accounting Center
        
    -   Engineering Center
        
-   Expense Report permission set to Edit or Full
    
-   Restrict Time and Expense preference is set to False
    

You can customize an existing role or create a new role to give access to accounting approval permissions. For more information, see [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html).

If an expense report is rejected by accounting, the employee can edit it. The employee's immediate supervisor can then resubmit it before it's routed to accounting for approval.

Expense reports that require accounting approval can be accessed in two different places:

-   Unapproved Expense Reports Register - See [Approving Expense Reports from the Register](#bridgehead_N913584).
    
-   Expense Reports List - See [Approving Expense Reports from the Expense Reports List](#bridgehead_N913659).
    

## Setting Default Payable Accounts for non-OneWorld Account {#subsect_1528469712}

Companies with multiple payable accounts can set a company-wide default payable account for expense reports. Setting a default account enables more consistent expense reporting across your company.

#### To set a default payable account non-OneWorld account:

1.  Go to _Setup > Accounting > Accounting Preferences_.
    
2.  Click the **Time & Expenses** subtab.
    
3.  In the **Default Payable Account for Expense Reports** field, select a payable account.
    
    Note:
    
    The Default Payable Account for Expense Reports field is only available when you have more than one payable account.
    
4.  Click **Save**.
    

In OneWorld accounts, the default payable account preference is set by subsidiary.

## Setting Default Payable Accounts for OneWorld Account {#subsect_156987306301}

#### To set a default payable account (OneWorld account):

1.  Go to _Setup > Company > Subsidiaries_.
    
2.  Next to the subsidiary you want to update, click **Edit**.
    
3.  Click the **Preferences** subtab.
    
4.  In the **Default Payable Account for Expense Reports** field, select a payable account.
    
5.  Click **Save**.
    

Note:

You can see the general ledger impact of an expense report before you approve it. You can also view the expense report record. Click the Actions menu, then click GL Impact.

## Approving Expense Reports from the Register {#bridgehead_N913584}

#### To approve expense reports from the Unapproved Expense Reports Register:

1.  Go to _Transactions > Employees > Enter Expense Reports_.
    
2.  In the More menu, click the **Approve Expense Reports** link.
    
3.  Click the date next to the expense report you want to approve.
    
4.  If the report is complete, click **Approve** in the middle of the form.
    
    If you want to reject the report, click **Reject**. When the email form appears, you can send a message to your employee about the expense report. Complete the email message, and then click **Save**.
    
    If multiple payable accounts exist and a default account isn't selected, you can't automatically approve the expense report from the register. You must edit the expense report and manually select a payable account. You set up a default account at Setup > Accounting > Accounting Preferences > Time & Expenses.
    

## Approving Expense Reports from the Expense Reports List {#bridgehead_N913659}

#### To approve expense reports from the list:

1.  Go to _Transactions > Employees > Enter Expense Reports > List_.
    
2.  Click **Edit** next to an expense report with a status of **Pending Accounting Approval**.
    
3.  On the expense report, check the **Accounting Approval** box.
    
4.  If multiple accounts payable accounts are available and a default account hasn't been set, select a payable account in the **Account** field. (This field doesn't appear if there's only one accounts payable account.)
    
5.  Click **Save**.
    

Note:

If you customize the expense report list view to include a Currency column, note the following. The listed currency values correspond to base currencies for employees and may not match the currencies entered in the expense reports.

### Related Topics

-   [Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908140.html)
-   [Employee Access to Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N908637.html)
-   [Enter an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N911232.html)
-   [Approving an Expense Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2396195.html)
-   [Editing an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1550694498.html)
-   [Deleting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3746063133.html)
-   [Rejecting an Expense Report From the Expense Reports List](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3751910971.html)
-   [Corporate Card Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1531259544.html)
-   [Reviewing Expense Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N913094.html)
-   [Paying Expenses on Employee Paychecks with Payroll](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914230.html)
-   [Giving an Employee Access to Purchase Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N914882.html)
-   [Notifying a Supervisor or Approver About Required Approvals](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N910874.html)
-   [Expense Reporting](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907845.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
