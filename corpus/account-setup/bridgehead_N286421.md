---
id: "bridgehead_N286421"
type: "bridgehead"
title: "Restricting Role Access to Subsidiaries (OneWorld Only)"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Customizing or Creating NetSuite Roles > Restricting Role Access to Subsidiaries (OneWorld Only)"
parent: "section_N285937"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N286421.html"
anchors: []
sha256: "af3e3c914f038def333b5f2902ae3b363b490b323409eaa57e0dfdd16d215d8f"
---

If you have NetSuite OneWorld, you can use subsidiary restrictions to restrict what users with this role can access.

When you restrict role access to subsidiaries, consider the following:

-   By default, the subsidiary restrictions is set to **User Subsidiary**.
    
-   Only a role with access to all subsidiaries assigned for a department can edit that department.
    

#### To restrict role access to specific subsidiaries:

1.  Go to _Setup > Users/Roles > User Management > Manage Roles_
    
2.  Click **Edit** next to the role whose access you want to restrict.
    
3.  Go to Subsidiary Restrictions, and choose one of the following options:
    
    -   **All** - Grants the role access to all subsidiaries, including inactive subsidiaries.
        
    -   **Active** - Grants the role access to the active subsidiaries only.
        
    -   **User Subsidiary** - Restricts the role's access to the user's subsidiary only. When users log in with this role, they can only access their own subsidiary. A user's subsidiary is set on the employee record. For more information, see [Assigning a Subsidiary to an Employee](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N276604.html).
        
    -   **Selected** - Grants the role access to one or more subsidiaries.
        
4.  If you choose **Selected**, in the auto-generated list of active and inactive subsidiaries, select the subsidiaries that you want the role to have access to. To select multiple subsidiaries, hold down the **Ctrl** key and click the selected subsidiaries.
    
5.  To allow users logged in with this role to see, but not edit, records for subsidiaries to which the role does not have access, check the **Allow Cross-Subsidiary Record Viewing** box. You cannot use this setting to view employee payroll or commissions data.
    
    Note:
    
    If the Book Record Restriction option is enabled for a user, this restriction overrides permissions granted by the Allow Cross-Subsidiary Record Viewing option.
    

The user with this edited role must log out of NetSuite and log in again to see the changes in the restrictions.

### Related Topics

-   [Customizing or Creating NetSuite Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N285937.html)
-   [Customizing and Creating Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N286284.html)
-   [Assigning Core Administration Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1552315155.html)
-   [Administrator - No HR/Employee Access SuiteApp](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1542138381.html)
-   [Restricting Role Access to Accounting Books](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_162486701937.html)
-   [Setting Employee Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637690919.html)
-   [Setting Department, Class, and Location Restrictions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_4637695352.html)
-   [Setting a Role as Issue Role for Issue Management](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288585.html)
-   [Setting a Role as Web Services Only Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288629.html)
-   [Setting a Role as Single Sign-On Only Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288661.html)
-   [Restricting a Role by Device ID](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1517945850.html)
-   [Restricting a Role by IP Address](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288693.html)
-   [Setting Two-Factor Authentication Requirements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_1517945906.html)
-   [Setting Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288727.html)
-   [Setting Default and Restricted Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288877.html)
-   [Setting Search Defaults for a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N288948.html)
-   [Setting Role-Based Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292753.html)
-   [Translating Custom Role Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N292998.html)
-   [Selecting a Dashboard for a Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N289178.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
