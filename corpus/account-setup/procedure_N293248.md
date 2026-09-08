---
id: "procedure_N293248"
type: "procedure"
title: "To Mass Update a Permission for Multiple Roles"
branch: "account-setup"
category: "account-administration"
breadcrumb: "Account Administration > Account Setup > NetSuite Users & Roles > NetSuite Roles Overview > Mass Updating a Permission on Custom Roles > To Mass Update a Permission for Multiple Roles"
parent: "section_N293188"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/procedure_N293248.html"
anchors: []
sha256: "30f648133b6a4ca967cb64aa5a17d3fed898bd523521fad46c83af7185a0b1e5"
---

1.  Go to List > Mass Update > Mass Updates, expand Roles & Permissions, and select Add/Edit Permission on Roles.
    
2.  In the **Title of Action** field, enter a name for this update.
    
3.  In the **Permission** field, select the permission that you want to change for selected roles.
    
    -   Click the icon at the right of this field to see a list.
        
    -   Note that all permissions are listed in alphabetical order; they are not divided into Transactions, Reports, Lists, Setup, and Custom Records, as they are on role records.
        
4.  In the **Level** field, choose the permission access level to be applied to selected roles.
    
    -   Choose **None** to remove the permission from selected roles.
        
    -   Note that the available access levels vary according to the permission selected. See [Access Levels for Permissions](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N326341.html).
        
5.  For custom record permissions only, you can select a value in the **Restrict** field, to limit the selected roles' access to custom records of the type indicated by the permission.
    
    -   Select **Viewing and Editing** to restrict users with selected roles to viewing or editing only the records of this type that they or their subordinates created.
        
    -   Select **Editing Only** to restrict users with selected roles to editing only the records of this type that they or their subordinates created but allow them to view all records of this type.
        
    -   Leave this column blank to allow users with selected roles to view and edit all records of this type.
        
    
    For information about custom record type permissions, see [Setting Permissions for a Custom Record Type](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2879388.html).
    
6.  To limit the roles where the selected permission should be modified, define a filter or filters on the **Criteria** subtab.
    
    -   If existing role fields do not provide needed filtering, you can create one or more custom field(s) of the Other Custom Field type, and add them to role records, to be used as filter criteria for this mass update. See [Adding Custom Role Fields to be Mass Update Filter Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N294802.html).
        
    -   If you do not define any filter criteria, the permission change is applied to all custom roles in the account, other than customized Customer Center, Employee Center, Partner Center, and Vendor Center roles.
        
7.  Define display options for mass update results on the **Results** subtab.
    
8.  Define the users who can run the update on the **Audience** subtab, if available.
    
9.  If you have the Administrator role and you want to run the mass update on a recurring basis, set up this recurrence on the **Schedule** subtab. See [Scheduling a Mass Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N668529.html).
    
10.  View audited changes and actions respective to the update on the **Audit Trail** subtab.
     
11.  Click **Preview** to see which records the mass update will change, and review the Mass Update Preview page.
     
     -   To modify the mass update, click **Return to Criteria**, and repeat the previous steps as necessary.
         
     -   If your list has less than 1000 entries, an **Apply** column is shown. If any record listed should not be updated, clear the box in the **Apply** column.
         
12.  Choose one of the following options: **Perform Update**, or **Save**.
     
     you click **Perform Update**, you cannot stop or cancel the mass update, so proceed with caution!
     

### Related Topics

-   [Mass Updating a Permission on Custom Roles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N293188.html)
-   [Adding Custom Role Fields to be Mass Update Filter Criteria](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N294802.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
