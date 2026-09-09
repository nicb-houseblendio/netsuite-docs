---
id: "section_N555081"
type: "section"
title: "Granting User Access to Transaction History"
branch: "auditing-and-data-management"
category: "account-administration"
breadcrumb: "Account Administration > Auditing and Data Management > Managing Transactions > Reviewing Transaction History > Granting User Access to Transaction History"
parent: "section_N554247"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555081.html"
anchors: ["procedure_N555123"]
sha256: "bb93f0836ad9312ebeeb31ed8cbede4d2a375807f944a74678350ae125ccf4ce"
---

Users need the Financial History permission to view transaction history. Some roles have this permission by default, such as accounting clerks and sales administrators. To review permissions for standard roles, see [Standard Roles Permissions Table](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N295396.html).

An administrator can give other users access to transaction histories by adding the Financial History permission to their roles. For example, support reps can be allowed to see the sales transactions that customers inquire about.

#### To create a custom role with transaction history access: {#procedure_N555123}

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_.
    
2.  Click **Customize** next to the name of the role you want to customize.
    
3.  In the **Name** field, enter the name for this new role.
    
    This role name will be available in employee records on the **Access** subtab.
    
4.  On the **Permissions** subtab, click the **Lists** subtab.
    
5.  In the **Permission** column, select **Financial History**.
    
6.  In the **Level** column, select **View**.
    
7.  Click **Add**.
    
8.  Click **Save**.
    

With the new customized role, employees can view the Transaction History subtab on customer records and click the links to view those transactions.

To assign employees this custom role, go to _Lists > Employees > Employees_, and click Edit beside the employee you want to assign the role. Click the Access subtab. Select the new role in the Role field, and click Add/Edit. Click Save.

Important:

If the Global Permissions feature is enabled, the Financial History permission also can be added on a per-employee basis. For information, see [Using the Global Permissions Feature](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326630.html).

### Related Topics

-   [Reviewing Transaction History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554247.html)
-   [Transaction System Information and Communication Subtabs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N554714.html)
-   [Viewing Transaction System Notes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N555355.html)
-   [Using the Transaction Audit Trail](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N556825.html)
-   [Tracking Financial Account Changes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557197.html)
-   [Line-Level Audit Trail for Transactions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557476.html)
-   [Transaction Line-Level History Window](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N557750.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
