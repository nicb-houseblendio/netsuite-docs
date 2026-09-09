---
id: "section_N901259"
type: "section"
title: "Working with Employee Social Security Numbers"
branch: "employees"
category: "employee-management"
breadcrumb: "Employee Management > Employees > Employee Information Management > Working with Employee Social Security Numbers"
parent: "chapter_N894090"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N901259.html"
anchors: ["subsect_159233362314"]
sha256: "172073f67b045aacbe02f8e1cda65cc189da1e17a5d1fb46232fe2cb7f58549a"
---

Warning:

In some cases, your scripts may expose social security numbers to any user with administrator access. To prevent unintended access to this information, ensure only authorized users have access to scripts that may expose this information.

Social security numbers are masked and encrypted by default when displayed on the screen or when records or transactions are printed. Only administrators or users with permission to access social security number data can view the numbers unmasked.

Users permission to access social security number data is based on the level of the Employee Social Security Numbers permission. This permission is associated with their assigned roles. This permission can be at one of the following two levels:

-   **Masked** - Social security numbers appear in masked form such as (\*\*\*\*\*\*\*\*\* or \*\*\*\*\*\*\*\*\*\*\*). If 11 characters are displayed, it indicates that hyphens were used when the social security number was entered.
    
-   **Full** - The complete social security numbers is displayed such as (123-11-1234).
    

Users assigned standard roles can access social security number data as follows:

| Role | Permission Level |
| --- | --- |
| Administrator | Full |
| Employee Center | Masked |
| Payroll Manager | Full |
| Payroll Setup | Full |
| System Administrator | Full |

Social security number data is masked or displayed based on role access level when a user does any of the following:

-   Views the employee list
    
-   Views or edits HTML or PDF formats of forms
    
-   Views reports
    
-   Customizes reports
    
-   Saves or views saved reports
    

## Social Security Numbers in Search {#subsect_159233362314}

To ensure the security of your employees' social security numbers, NetSuite encrypts social security numbers. Because the numbers are encrypted, you cannot run a search that includes social security numbers in the results using the summary type Group.

### Related Topics

-   [Adding an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N894212.html)
-   [Adding Employees by Importing a CSV File](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322503072.html)
-   [Editing Employee Records Using CSV Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162322804075.html)
-   [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html)
-   [Assigning a Supervisor to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N898466.html)
-   [Viewing and Editing an Employee Record with Effective Dating](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494510731.html)
-   [Rehiring a Terminated Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_160763200766.html)
-   [Searching for Effective-Dated Changes to the Employee Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1503337187.html)
-   [Viewing an Employee's Timeline](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_156216462597.html)
-   [Employee Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899090.html)
-   [Creating an Employee Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N899487.html)
-   [Printing Mailing Labels for Employees](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N916939.html)
-   [Employee Information Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N894090.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
