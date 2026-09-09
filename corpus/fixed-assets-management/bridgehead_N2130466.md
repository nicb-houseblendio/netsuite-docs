---
id: "bridgehead_N2130466"
type: "bridgehead"
title: "Record Permissions for Fixed Assets Management"
branch: "fixed-assets-management"
category: "accounting"
breadcrumb: "Accounting > Fixed Assets Management > Installing the Fixed Assets Management SuiteApp > Setting Fixed Assets Management Permission Levels > Record Permissions for Fixed Assets Management"
parent: "section_N2130365"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2130466.html"
anchors: []
sha256: "bc71c06d01c69b8dbf4bd335c5161f8be1f6fbbedaf134c73e11ea42ea6f2d3f"
---

To set permissions for a role, go to the Permissions subtab in Setup > Users/Roles > Manage Roles.

Permissions are divided into four subtabs: Transactions, Reports, Lists, Setup, and Custom Record.

-   To add a permission, do one of the following:
    
    -   Click a line in the list, select a permission, and then click **Insert**.
        
    -   Click **Add Row** at the bottom of the list, select a permission, and then click **Add**.
        
-   To remove a permission, select it from the list, and then click **Remove**.
    
-   To set the level of access for a permission, click a line in the list, and then select the level of access from the Level column. For information about these access levels, see [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).
    
-   You can limit a role's access to custom records by selecting value in the Restrict column. Each custom record permission provides access to a custom record type.
    
    -   **Viewing and Editing** - Restricts the role to view or edit only the records (of this type) that they or their subordinates created.
        
    -   **Editing Only** - Restricts the role to edit only the records (of this type) that they or their subordinates created. They can view all records of this type.
        
    
    Leave this column blank to give the role view and edit access to all records of this type.
    

You can use a mass update to add, remove, or change the level of a permission for multiple roles at the same time. For more information, see [Mass Updating a Permission on Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N293188.html).

The following table lists the record permissions required to use the Fixed Assets Management features.

| Subtab | Permission | Level | Notes |
| --- | --- | --- | --- |
| Transactions | Make Journal Entry | Full | Processes such as Depreciation, Revaluation and Disposal run with client user permissions and need to create Journals |
| Transactions | Bill | View |  |
| Transactions | Find Transaction | Full |  |
| Transactions | Invoice | Full |  |
| Custom Record | FAM Alternate Depreciation | Full |  |
| Custom Record | FAM Alternate Methods | Full |  |
| Custom Record | FAM Asset | Full |  |
| Custom Record | FAM Asset Proposal | Full |  |
| Custom Record | FAM Asset Reset Data | Create |  |
| Custom Record | FAM Asset Transfer Accounts | Full |  |
| Custom Record | FAM Asset Type | Full |  |
| Custom Record | FAM Asset Usage | Full |  |
| Custom Record | FAM Asset Values | Full |  |
| Custom Record | FAM Default Alt Depreciation | Full |  |
| Custom Record | FAM Depreciation History | Full |  |
| Custom Record | FAM Depreciation Method | Full |  |
| Custom Record | FAM Last Proposal Dates | Full |  |
| Custom Record | FAM Lifetimes | Full |  |
| Custom Record | FAM Process | Full |  |
| Custom Record | FAM Proposal Alt Depreciation | Full |  |
| Custom Record | FAM Repair & Maint Category | Full |  |
| Custom Record | FAM Repair & Maint Sub A | Full |  |
| Custom Record | FAM Repair & Maint Sub B | Full |  |
| Custom Record | FAM System Setup | Full |  |
| Custom Record | FAM Transaction Field Map | Full |  |
| Custom Record | BG Process Instance | Full |  |
| Custom Record | BG Summary Record | Full |  |
| Lists | Accounts | View |  |
| Lists | Classes | View |  |
| Lists | Currency | View |  |
| Lists | Customers | View |  |
| Lists | Departments | View |  |
| Lists | Documents and Files | View | You must have read access to the FAM resource folder (src/resource) so that Suitelets load without issue. If you still encounter issues even with the Documents and Files permission, check that your role complies with the restrictions (SCDL or group restrictions) applied on the FAM resource folder. |
| Lists | Items | View |  |
| Lists | Locations | View |  |
| Lists | Perform Search | View |  |
| Lists | Projects | View |  |
| Lists | Subsidiaries | View |  |
| Lists | Tax Items | Create |  |
| Setup | Accounting Book | View |  |
| Setup | Manage Accounting Periods | View |  |
| Setup | Setup Company | View |  |

### Related Topics

-   [Installing the Fixed Assets Management SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2126830.html)
-   [Making the Fixed Assets Tab Available to Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2129964.html)
-   [Setting Up the Fixed Assets Management System](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N2135031.html)
-   [Form Permissions for Fixed Assets Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2132392.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
