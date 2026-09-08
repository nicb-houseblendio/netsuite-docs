---
id: "section_N262059"
type: "section"
title: "Restricting Access to Records by Class"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Departments and Classes Overview > Restricting Access to Records by Class"
parent: "section_N261602"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262059.html"
anchors: []
sha256: "61012dfb5c69178797a39321d6aa213e615917ca2ea2f16fb2ce5623ec438007"
---

If your account has the Classes feature enabled, you can limit access to transaction, employee, partner, and optionally item records based on their class values. You can also limit which classes users can assign to these records. You can set class restrictions by user role and apply them to everyone using that role.

Important:

Any account in the Chart of Accounts list without an assigned class isn't subject to the **own, subordinate, and unassigned** or **own and subordinates only** restrictions.

The following settings for the Class Restrictions field on the Role page define class-related restrictions for transaction and customer records:

-   **none - no default** - There is no restriction on what can be selected. This field doesn't affect record access and doesn't show a default selection.
    
-   **none - default to own** - There is no restriction on what can be selected. Record access is not determined by this field. Fields of this type select the user by default.
    
-   **own, subordinate, and unassigned** - Users can only access records with their class, child classes, or unassigned classes. For example, if your role has access to class A, you can see only records in class A, its children or unassigned records.
    
-   **own and subordinates only** - Users can only access records with their class and its child classes. For example, if your role has access to class A, you can see only records in class A and its children.
    

Check the **Allow Viewing** box to let users logged in with this role see, but not edit, records for classes they don't have access to.

Check the **Apply to Items** box to add these class restrictions to item records, in addition to transaction and customer records.

To set up a role with these restrictions, go to _Setup > Users/Roles > Manage Roles_ and click **Customize**, **Edit**, or **New**.

Important:

In NetSuite OneWorld, subsidiary restrictions automatically apply to classes. For example, if Class A is assigned to only Subsidiary X and a role is restricted to Subsidiary X, users with that role can access only Class A, even if the role doesn't have class restrictions.

Important:

If you're using the Advanced Employee Permissions feature, restrictions on the Role page apply only to Employees and Employee Administration permissions. Employee Public and Employee Confidential permissions ignore the restrictions on this page. For more information, see [Setting Employee Access for Advanced Employee Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494598267.html).

You can also apply role-based class restrictions to custom records. For more information, see [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).

### Related Topics

-   [Departments and Classes Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261602.html)
-   [Creating Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N261769.html)
-   [Modifying and Deleting Classes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176293394.html)
-   [Creating Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262248.html)
-   [Modifying and Deleting Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176372145.html)
-   [Restricting Access to Records by Department](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262535.html)
-   [Converting Classes to Departments](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262723.html)
-   [Converting Classes to Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N262871.html)
-   [Custom Segments Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4732448748.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
