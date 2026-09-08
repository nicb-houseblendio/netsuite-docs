---
id: "section_N265799"
type: "section"
title: "Restricting Access to Records by Location"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > Classifications in NetSuite > Locations Overview > Restricting Access to Records by Location"
parent: "section_N263024"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265799.html"
anchors: []
sha256: "a823ba1f9fd7ca5478232b9f4de0c3a02a4c1f6f8d771a8f1e4895bca872486c"
---

If your account has the Locations feature enabled, you can restrict access to transaction, employee, partner, and optionally item records based on location values. You can also limit which locations users can assign to these records. You can set location restrictions by user role and then apply them to everyone using that role.

Important:

Any account in the Chart of Accounts without an assigned location isn't subject to the **own, subordinate, and unassigned** or **own and subordinates only** restrictions.

The following settings for the Location Restrictions field on the Role page define location-related restrictions for transaction and customer records:

-   **none - no default** - There is no restriction on what can be selected. This field doesn't affect record access and doesn't show a default selection.
    
-   **none - default to own** - There is no restriction on what can be selected. Record access is not determined by this field. Fields of this type select the user by default.
    
-   **own, subordinate, and unassigned** - Users can access only records with their location, child locations, and unassigned location field. For example, if your role has access to location A, you can see only records with location A, its children or unassigned accounts.
    
-   **own and subordinates only** - Users can access only records with their location and children locations. For example, if your role has access to location A, you can see only records with location A and its children.
    

Check the **Allow Viewing** box to let users logged in with this role see, but not edit, records for locations they don't have access to.

Check the **Apply to Items** box to add these location restrictions to item records, in addition to transaction and customer records.

To set up a role with these restrictions, go to _Setup > Users/Roles > Manage Roles_. Click **Customize** or **Edit**, or click the New button.

Important:

In NetSuite OneWorld, subsidiary restrictions automatically apply to locations. For example, if Location A is assigned to only Subsidiary X and a role is restricted to Subsidiary X, users with that role can access Location A only, even if that role doesn't have location restrictions.

Important:

If you're using the Advanced Employee Permissions feature, restrictions on the Role page apply only to the Employees and Employee Administration permissions. The Employee Public and Employee Confidential permissions ignore the restrictions on this page. For more information, see [Setting Employee Access for Advanced Employee Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1494598267.html).

You can also apply role-based location restrictions to custom records. For more information, see [Applying Role-Based Restrictions to Custom Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2880594.html).

### Related Topics

-   [Locations Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263024.html)
-   [Creating Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N263263.html)
-   [Modifying and Deleting Locations](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4176380463.html)
-   [Making a Location Inactive](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265253.html)
-   [Associating a Transaction with a Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265426.html)
-   [Searching for a Transaction by Location](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N265573.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
