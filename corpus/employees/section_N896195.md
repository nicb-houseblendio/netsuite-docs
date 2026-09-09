---
id: "section_N896195"
type: "section"
title: "Giving an Employee Access to NetSuite"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Employee Information Management > Giving an Employee Access to NetSuite"
parent: "chapter_N894090"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html"
anchors: ["procedure_N896243", "subsect_1536867824"]
sha256: "74ad6c421b3a719c5b1fb9cf8808a83b3ac2d697ff3f70d7881a919b39accf16"
---

Important:

Don't give access to unknown email addresses, or unknown employees. It is also unsafe to use generic email addresses like test@test.com.

To give an employee access to your NetSuite account, you must ensure the employee record includes an email address. The email address serves as the user ID. Then, complete the necessary information on the Access subtab of the employee record. This setup includes the following:

-   Enabling the Give Access option
    
-   Assigning roles and permissions
    

Note:

If you use the Effective Dating feature, the **Give Access** box and the **Email** address field on the employee record are not effective-dated. If you grant access to an employee or change the employee's email address, as part of an effective-dated change, those two changes are immediate.

Note:

If you use the Advanced Employee Permissions feature, the Employee Access permission must be assigned to a role. This assignment lets the role give access and assign roles to employees. For more information, see [Employee Access Tab Permission Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1541786744.html).

To secure the user login process:

-   Two-factor authentication is the preferred alternative to restricting access by IP Address. For more information, see [Two-Factor Authentication (2FA)](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N327688.html).
    
-   If you use the IP Address Rules feature, you can set up IP address restrictions to limit where employees can log in to NetSuite. For information about setting IP address rules, see [Enabling and Creating IP Address Rules](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4726612641.html).
    

Note:

Only active users with access count against the Full User Count purchased for your account. Inactive users that have access don't count. For information about making users inactive, see [Inactivating Employee Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504014571.html).

Follow this procedure to let employees set up a NetSuite password themselves. If you prefer to assign passwords, see [Assign an Employee Password Manually](#subsect_1536867824).

#### To give an existing employee access to NetSuite: {#procedure_N896243}

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the name of the employee for whom you want to set up access.
    
3.  Under Email|Phone|Address, enter the employee's email address.
    
    The email address is required for login.
    
4.  Click the **Access** tab.
    
5.  Check the **Give Access** box.
    
6.  Check the **Send New Access Notification Email** box to inform the user how to access your NetSuite account. The standard user access notification includes the email address to use for logging in to NetSuite. It also contains a URL so that the user can set up a NetSuite password. The user must set up a NetSuite password within 24 hours or the URL will expire. If this occurs, edit the employee record, clear the **Give Access** box, click **Save**, and repeat steps 1-6.
    
    Important:
    
    The email contains the URL only if the user doesn't have access to NetSuite. For example, it is a new user, or it is a user whose access was removed.
    
7.  On the **Roles** subtab, assign one or more roles to this employee.
    
    Each role includes a set of associated permissions that determine the data assigned users can see and the tasks they can perform. For more information, see [Assigning Roles to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N897798.html).
    
8.  If you use the **Global Permissions** feature on the **Employees** subtab, note the following. A **Global Permissions** subtab is available on the employee record. Use this subtab to assign permissions. Go to _Setup > Company > Enable Features_ to enable this feature.
    
    These permissions apply for all of the employee's assigned roles. For more information, see [Using the Global Permissions Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326630.html).
    
9.  Click **Save**.
    

## Assign an Employee Password Manually {#subsect_1536867824}

Use the following procedure if you prefer to assign a user's password, rather than letting users assign their own password.

#### To give an employee access to NetSuite and assign a password:

1.  Go to _Lists > Employees > Employees_.
    
2.  Click **Edit** next to the name of the employee for whom you want to set up access.
    
3.  Under Email|Phone|Address, enter the employee's email address.
    
    The email address is required for login.
    
4.  Click the **Access** tab.
    
5.  Check the **Give Access** box.
    
6.  Do not check the **Send New Access Notification Email** box.
    
7.  Check the **Manually Assign or Change Password** box.
    
8.  Enter a password for the employee. As you type, the characters are validated against the password policy criteria, and the results displayed.
    
    Note:
    
    For employees who can view unencrypted credit card numbers, note the following. The password must be at least 12 characters or the minimum length required for your account, whichever is greater. This is required to comply with Payment Card Industry (PCI) Data Security Standard. For more information, see [NetSuite Password Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N250541.html).
    
9.  In the **Confirm Password** field, re-enter the password.
    
10.  Check the **Require Password Change on Next Login** box to require this employee to change their password on their next login to NetSuite.
     
     When the employee next logs in, the **Change Password** page appears. The user cannot access other NetSuite pages until a new password is created and saved.
     
     Requiring this action protects your account from unauthorized access using generic passwords and prepares your account for an audit.
     
     Important:
     
     The **Require Password Change on Next Login** box never appears as checked. When you check this box and save the record, an internal flag is set. When the password change occurs, the flag is cleared. If you later check the box again and resave the record, the internal flag is reset to require another password change.
     
11.  When you have finished entering information, click **Save**.
     
12.  Next, tell your user the appropriate login page to go to, the email address to use for login, and the password you assigned. For security reasons, don't send the password by email.
     
     For more information, see [Types of Login Pages for Your NetSuite Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1504012590.html).
     

### Related Topics

-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Adding Employees by Importing a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322503072.html)
-   [Editing Employee Records Using CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322804075.html)
-   [Assigning a Supervisor to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898466.html)
-   [Viewing and Editing an Employee Record with Effective Dating](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494510731.html)
-   [Rehiring a Terminated Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160763200766.html)
-   [Searching for Effective-Dated Changes to the Employee Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503337187.html)
-   [Viewing an Employee's Timeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156216462597.html)
-   [Employee Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899090.html)
-   [Creating an Employee Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899487.html)
-   [Working with Employee Social Security Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html)
-   [Printing Mailing Labels for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N916939.html)
-   [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
