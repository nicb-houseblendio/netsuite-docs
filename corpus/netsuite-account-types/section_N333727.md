---
id: "section_N333727"
type: "section"
title: "Granting Access to Your Sandbox Account"
branch: "netsuite-account-types"
category: "account-administration"
breadcrumb: "Account Administration > NetSuite Account Types > NetSuite Sandbox > Granting Access to Your Sandbox Account"
parent: "chapter_N333400"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N333727.html"
anchors: ["subsect_162136701343", "subsect_162136719078", "procedure_4775192547", "subsect_162136745765", "procedure_1524250666"]
sha256: "30e638e381307e6642d4250fb5da5d94221f8ec120f56ee85a543757ebec8808"
---

On the Sandbox Accounts page, account administrators can select who can access the sandbox: only users with an administrator role, or all users.

## Preference for Access After Sandbox Refresh {#subsect_162136701343}

A preference is provided on the Sandbox Accounts page to indicate who should have access to a sandbox account after it is refreshed: either administrators only or all users. If the Administrators only option is selected, only the Administrator role is copied to the sandbox. That is, for a user with multiple roles, only the administrator role for that user is copied to the sandbox. For more information, see [Refreshing Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334348.html).

### Giving Sandbox Access to Individual Users {#subsect_162136719078}

After a refresh of a sandbox account is complete, access can be added or removed as necessary for individual users in that account.

#### To give sandbox access to individual users: {#procedure_4775192547}

1.  In the sandbox account, go to _Lists > Employees > Employees (Administrator)_ and click **Edit** next to the name of the employee.
    
    Important:
    
    Customer Center and Partner Center roles are never allowed access to sandbox accounts.
    
2.  On the **Access** subtab in the employee record, clear the **Give Access** checkbox.
    
    ![Give Access box on the Access subtab.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/NetSuiteAccountTypes/GiveAccess.png)
    
    Note:
    
    Make note of the roles assigned to the user for later.
    
3.  Click **Save**.
    
4.  **Edit** the same employee record.
    
5.  On the **Access** subtab, check the **Give Access** box again and enter any required information.
    
6.  Reassign the appropriate roles to the user.
    
7.  Click **Save**.
    
8.  Advise the user to log out of their account and then log back in to access the sandbox account.
    
    -   On the My Roles page, the role is labeled Sandbox in the Account Type column.
        
    -   In the Change Roles list, the sandbox role is indicated by an SB symbol.
        

To give sandbox access to all users of your production account, you must go to the Sandbox Accounts page in your production account, select the **All Users** option for **Access After Sandbox Refresh**, and click **Refresh Sandbox** to request a refresh of your sandbox account.

### Giving Sandbox Access to Multiple Users {#subsect_162136745765}

The Administrator can use the CSV Import Assistant to give sandbox access to multiple users at a time.

#### To give multiple users access to the sandbox account using CSV import: {#procedure_1524250666}

1.  From your sandbox account, create a search for **Employee** with the following results:
    
    -   Internal ID (of the Employee)
        
    -   Give Access
        
2.  Export the search results as a CSV file.
    
3.  Add the non-administrator employees that you want to have sandbox access to the CSV file.
    
4.  Update the employee record in sandbox using the CSV Import Assistant.
    
    1.  Go to _Setup > Import/Export > Import CSV Records_.
        
    2.  Set the Import Type to **Employees**.
        
    3.  Set the Record Type to **Employees**.
        
    4.  Select the CSV file you want to import, and click **Next**.
        
    5.  Set Data Handling to **Update**, and click **Next**.
        
    6.  Make sure you map the following fields (your field and the NetSuite field must match), and then click **Next**:
        
        -   Internal ID
            
        -   Give Access
            
    7.  Click **Save & Run**.
        
    
    Note:
    
    For more information, see [Importing CSV Files with the Import Assistant](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N343158.html).
    

Important:

During the upgrade period for a new release of NetSuite, please pay attention to your scheduled upgrade date. Do not request a sandbox refresh when the upgrade date is near. A refresh will fail if it does not complete before your scheduled upgrade begins. See [Scheduled Version Upgrade Dates and Refresh Requests](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162577313831.html).

### Related Topics

-   [Removing Sandbox Access from Individual Users](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_162136754097.html)
-   [NetSuite Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N333400.html)
-   [About Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4609939018.html)
-   [Features Available for Testing in a Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N335071.html)
-   [Logging in to Your Sandbox Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430989285.html)
-   [Working with Multiple Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4430991327.html)
-   [Refreshing Sandbox Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334348.html)
-   [Data That is Not Copied from Production to Sandbox](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1516026974.html)
-   [Credit Card Processing in Your Sandbox After a Refresh](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_1516027026.html)
-   [When a Sandbox Account Expires](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334950.html)
-   [Setting Preferences for Sandbox Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N334772.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
