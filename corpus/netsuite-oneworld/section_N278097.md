---
id: "section_N278097"
type: "section"
title: "Control Employee Access to Subsidiaries"
branch: "netsuite-oneworld"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite OneWorld > Subsidiary Setup > Control Employee Access to Subsidiaries"
parent: "section_N272210"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278097.html"
anchors: []
sha256: "5ac3e50a06baeb0f9c6127663906f6857c3152597f9847b9fbab1e7e4757f50b"
---

By default, an employee has access to data for the subsidiary assigned on the employee record. For more information, see [Assigning a Subsidiary to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276604.html). However, you can grant an employee access to data for additional subsidiaries. Go to _Setup > Users/Roles > User Management > Manage Roles_. For the employee's assigned role, use the multi-select Subsidiaries list to customize the role. Press and hold the Ctrl key to select multiple subsidiaries.

The Role page also includes the Allow Cross-Subsidiary Record Viewing option. Check this box to permit users logged in with that role to see data from subsidiaries other than those selected in the Subsidiaries list.

Note:

Users with the Book Record Restriction option enabled override permissions granted by the Allow Cross-Subsidiary Record Viewing option.

Important:

The records and transactions that employees can view and edit for subsidiaries are limited by the complete set of permissions defined for their assigned roles. For example, by default, employees of a specific subsidiary are able to view and edit data only for the that subsidiary. If you customize a role to include multiple subsidiaries (Subsidiaries list), employees assigned this role can view and edit data for these subsidiaries. If you also checked the Allow Cross-Subsidiary Record Viewing box for the customized role, employees assigned this role can view data for all subsidiaries.

Note:

Employees with access to all active subsidiaries but not to one or more inactive subsidiaries are considered to have access to all subsidiaries.

The following choices are dependent on the subsidiaries selected for the user's assigned role, or on the subsidiary assigned to the employee record:

-   Available subsidiaries in the Subsidiary field when the user creates new entity and item records
    
    See [Associate Subsidiaries with Entities and Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276477.html) and [Associate Subsidiaries With Items](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N276948.html).
    
-   Available entities when the user creates new transactions
    
    Generally, users can create transactions only for entities associated with subsidiaries to which they have access. Time and expense entry forms are exceptions to this general rule. These forms they permit creation of transactions for customers or projects associated with other subsidiaries, if they are not billable.
    
-   Available subsidiaries in Subsidiary Context list when the user runs reports
    
-   Available classes, departments, and locations in footer filters on reports
    

A user can restrict the records displayed in NetSuite to those for a single subsidiary. Go to the Restrict View subtab at _Home > Set Preferences_. See [Restrict Your Subsidiary View](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N278473.html).

Important:

To generate automated intercompany adjustments for expenses, supported by the Intercompany Time and Expense feature, a user must have access to all subsidiaries. For information about this capability, see [Enabling Intercompany Time and Expenses](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1476983.html).

### Related Topics

-   [Creating Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272471.html)
-   [Editing Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273122.html)
-   [Deleting Subsidiary Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3760056730.html)
-   [Adding or Removing Nexuses from a Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273510.html)
-   [Locking Transactions by Subsidiary](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N273734.html)
-   [Using Subsidiary-Specific Transaction Auto-Numbering](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N275081.html)
-   [Subsidiary Setup](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N272210.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
