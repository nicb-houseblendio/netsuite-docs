---
id: "section_N262535"
type: "section"
title: "Restricting Access to Records by Department"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Departments and Classes Overview > Restricting Access to Records by Department"
parent: "section_N261602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262535.html"
anchors: []
sha256: "5e8d7a52e914e67e16ac86aca5988b04428c0d81ac4d9ad04a71759a999d95f3"
---

If your account has the Departments feature enabled, you can limit access to transaction, employee, partner, and optionally item records based on department values. You can also limit which departments users can assign to these records. You can set department restrictions by user role and apply them to everyone using that role.

Important:

Any account in the Chart of Accounts without an assigned department isn't affected by the **own, subordinate, and unassigned** or **own and subordinates only** restrictions.

The following settings for the Department Restrictions field on the Role page define department-related restrictions for transaction and customer records:

-   **none - no default** - There is no restriction on what can be selected. This field doesn't affect record access and doesn't show a default selection.
    
-   **none - default to own** - There is no restriction on what can be selected. This field doesn't affect record access. Fields of this type select the user's department by default.
    
-   **own, subordinate, and unassigned** - Users can only access records with their department, children departments and unassigned departments. For example, if your role has access to department A, you can see only accounts in department A, its children, or unassigned accounts.
    
-   **own and subordinates only** - Users can only access records with their department its children departments. For example, if your role has access to department A, you can see only accounts in department A and its children.
    

Check the **Allow Viewing** box to let users with this role see, but not edit, records for departments they don't have access to.

Check the **Apply to Items** box to add these department restrictions to item records, in addition to transaction and customer records.

To set up a role with these restrictions, go to _Setup > Users/Roles > Manage Roles_ and click **Customize**, **Edit**, **New**.

Important:

In NetSuite OneWorld, subsidiary restrictions automatically apply to departments. For example, if Department A is assigned to only Subsidiary X and a role is restricted to Subsidiary X, users with that role can access Department A, only even if the role doesn't have department restrictions.

Important:

If you're using the Advanced Employee Permissions feature, restrictions on the Role page only apply to the Employees and Employee Administration permissions. The Employee Public and Employee Confidential permissions ignore the restrictions on this page. For more information, see [Setting Employee Access for Advanced Employee Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494598267.html).

You can also apply role-based department restrictions to custom records. For more information, see [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).

### Related Topics

-   [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html)
-   [Creating Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261769.html)
-   [Modifying and Deleting Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176293394.html)
-   [Restricting Access to Records by Class](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262059.html)
-   [Creating Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262248.html)
-   [Modifying and Deleting Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176372145.html)
-   [Converting Classes to Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262723.html)
-   [Converting Classes to Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262871.html)
-   [Custom Segments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4732448748.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
