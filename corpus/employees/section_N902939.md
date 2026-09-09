---
id: "section_N902939"
type: "section"
title: "Giving an Employee Access to Time Tracking"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Time Tracking > Managing Time Tracking > Giving an Employee Access to Time Tracking"
parent: "section_N901953"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902939.html"
anchors: ["subsect_1536789369", "subsect_1536787429", "subsect_158799465963"]
sha256: "a66a7d0e07de2f42f28ef8f607713c526a4b38ca4d066e66bd838fa289e5f6bd"
---

Giving employees access to time tracking enables them to enter the hours they spend working for a particular customer or on a project.

There are three steps you must complete to give employees access to time tracking:

1.  An administrator must enable the **Time Tracking** features and set time tracking preferences.
    
2.  You must either set up access on employee records to the Employee Center or assign a custom role with the **Track Time** permission.
    
3.  You must provide access information to the employee.
    

After you've enabled time tracking, you can set preferences for how you want to use the feature.

Next, if you haven't already, create an employee record for employees that you want to give access to time tracking.

For more information about creating employee records, see the following:

-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
    
-   [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html)
    
-   [Assigning Roles to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N897798.html)
    

## Give Access to the Employee Center {#subsect_1536789369}

As of 2018.2, you should use the following procedure and let users set up a NetSuite password for themselves. However, if you prefer to assign user passwords yourself, see [Assign a Password Manually](#subsect_1536787429) instead.

#### To give an employee access to the Employee Center:

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the employee to whom you want to give access.
    
3.  Under Email|Phone|Address, ensure the employee's email address is entered.
    
4.  Click the **Access** subtab.
    
5.  Check the **Give Access** box.
    
6.  If this is a new employee, check the **Send New Access Notification Email** box to inform the user how to access your NetSuite account. The standard user access notification includes the email address to use for logging in to NetSuite, and also contains a URL so that the user can set up a NetSuite password.
    
7.  On the **Roles** tab, select **Employee Center** from the list.
    
8.  Click **Add**.
    
9.  Click **Save**.
    

## Assign a Password Manually {#subsect_1536787429}

You should use the procedure in [Give Access to the Employee Center](#subsect_1536789369) that lets users set up a NetSuite password for themselves. However, if you prefer to assign a user's password yourself, use the following procedure.

#### To manually assign a password:

1.  Do one of the following:
    
    -   If the user is an employee, go to _Lists > Employees > Employees_.
        
    -   If the user is not an employee, go to List > Relationships, and then select **Customers**, **Partners**, or **Vendors**.
        
2.  Click **Edit** next to the user that you want to assign a role to.
    
3.  In the **Email** field, enter the user's email address.
    
    This is the email address used to log in to NetSuite.
    
4.  Click the **Access** tab.
    
5.  Check the **Give Access** box.
    
6.  On the **Roles** tab, select **Employee Center** from the list.
    
7.  Don't check the **Send New Access Notification Email** box.
    
8.  Check the **Manually Assign or Change Password** box.
    
9.  Enter a password for your user. As you type, the characters are validated against the password policy criteria, and the results displayed.
    
    Note:
    
    If you need more information, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
10.  Enter the password again for verification.
     
11.  Check the **Require Password Change on Next Login** box to require the user to change the password on the next login to NetSuite.
     
     On the next login, they see the Change Password page and can't access other NetSuite pages until a new password is created and saved.
     
     Requiring this action protects your account from unauthorized access using generic passwords and prepares your account for an audit.
     
     Important:
     
     The **Require Password Change on Next Login** box never displays as checked. When you check this box and save the record, an internal flag is set. When the password change occurs, the flag is cleared. If you later check the box again and save the record, the internal flag is reset to require another password change.
     
12.  When you're done with entering information, click **Save**.
     
13.  Next, tell your user the appropriate login page to go to, the email address to use for login, and the password you assigned. For security reasons, don't send the password by email.
     
     For details, see [Types of Login Pages for Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504012590.html).
     

After employees log in to NetSuite, they can enter time and view their time reports.

If you enabled the **Require Approvals on Time Records** preference, supervisors can also approve time reports entered by the employees they supervise. You can also create custom approval routing workflows to enable more customization of your approval process. With custom approval routing on time entries, employees can approve or reject the entries where they are set as the Next Approver from the Employee Center.

## Assigning Custom Roles with Access to Time Tracking {#subsect_158799465963}

#### To assign an employee a custom role with access to time tracking:

1.  Go to Setup > Users/Roles > Manage Roles.
    
2.  Click **Customize** next to the role you want to assign with time tracking permission.
    
3.  Enter a name for this custom role.
    
4.  Check the **Restrict Time and Expenses** box to permit employees to enter time for only themselves.
    
5.  On the **Transactions** subtab, select **Track Time** in the **Permission** column.
    
6.  In the **Level** column, select **Full**.
    
7.  Click **Add**.
    
8.  Click **Save**.
    
9.  On employee records, select this role on the **Access** tab to assign this role and give access to time tracking.
    

### Related Topics

-   [Managing Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901953.html)
-   [Understanding Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902265.html)
-   [Setting Up Time Tracking Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N902575.html)
-   [Restricting Employee Time Tracking Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898879.html)
-   [Entering a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904108.html)
-   [Deleting or Editing Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4502096285.html)
-   [Weekly Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N904728.html)
-   [Weekly Timesheets](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4671374137.html)
-   [Using the Timer to Track Time](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905386.html)
-   [Calculating Total Time Worked](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N905783.html)
-   [Entering Time for a Payroll Item](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906077.html)
-   [Custom Fields in Time Tracking Pages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N906942.html)
-   [Approving or Rejecting a Time Transaction](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N907404.html)
-   [Custom Workflow-based Approvals for Time Tracking](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1554190531.html)
-   [Updating Time Entries](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156408321759.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
