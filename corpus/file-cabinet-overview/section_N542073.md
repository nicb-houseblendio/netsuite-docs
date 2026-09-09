---
id: "section_N542073"
type: "section"
title: "Restricting Access to File Cabinet Folders"
branch: "file-cabinet-overview"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > File Cabinet Overview > File Cabinet Folders > Restricting Access to File Cabinet Folders"
parent: "section_4811464978"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542073.html"
anchors: ["subsect_163723956300"]
sha256: "99a7c7cc85c8ab776a3c38030db4c3330d5f31ff9b0221d63d27767d2e4d6a2f"
---

Within your organization, you can restrict access to files by setting permissions on File Cabinet folders. You can't restrict individual files, but you can restrict access to the enclosing folder. You can set permissions based on various criteria, such as location and department.

When a folder is marked as private, only the person who created that folder and the account administrator have access to it. Administrators can view the contents of any folder, including private folders and folders that have been restricted. If you create a folder, you become the owner of that folder. The owner of a folder always has access to the folder regardless of restrictions.

## Restricting Access to Subfolders {#subsect_163723956300}

Note the following when you restrict access to a folder with subfolders:

-   If a subfolder is created under a parent folder **after** the parent folder was restricted to a group, the subfolder automatically inherits the parent folder's restriction. You can change the subfolder's restriction.
    
-   If a parent folder's restriction is changed **after** a subfolder was created, the subfolder doesn't automatically inherit the new restriction. You can manually apply the restriction to the subfolder.
    

#### To change the restricted access setting in a folder:

1.  Log in to NetSuite with a role that has access to the folder.
    
2.  Go to _Documents > Files > File Cabinet_.
    
3.  Click **Edit** on the folder to which you want to restrict access.
    
4.  To restrict access in the following categories, select from the dropdown lists. Note that the following list names may be different depending on record naming customization in your NetSuite account:
    
    -   Restrict by Class
        
    -   Restrict by Department
        
    -   Restrict by Location
        
    -   Restrict by Group. If you choose a dynamic group, for performance reasons, the folder is restricted to a snapshot of the dynamic group members. The snapshot is updated twice a day. For more information, see [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html).
        
    -   Restrict by Subsidiary. Note that employees assigned to the parent subsidiary can access all child subsidiary folders. To change this behavior you can restrict the folder by group.
        
        For more information, see File Access Restriction by Subsidiary in File Cabinet (SuiteAnswers ID: 35400).
        
5.  Click **Save**.
    

All files in the folder are available based on the restricted access settings you selected.

### Related Support Articles

-   [Role Able to Access Restricted Files via 'Attach File' Column or via File URL](https://suiteanswers.custhelp.com/app/answers/detail/a_id/34568)

### Related Topics

-   [File Cabinet Folders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4811464978.html)
-   [Creating a Shortcut to a File Cabinet Folder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163723979344.html)
-   [Creating File Cabinet Folders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N541665.html)
-   [Deleting Folders from the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3947389300.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
