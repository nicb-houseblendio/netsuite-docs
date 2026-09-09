---
id: "section_N354513"
type: "section"
title: "Sharing Imports"
branch: "csv-imports"
category: "account-administration"
breadcrumb: "Account Administration > CSV Imports > Importing CSV Files with the Import Assistant > Working with Saved CSV Imports > Sharing Imports"
parent: "section_N353796"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354513.html"
anchors: ["procedure_N354618", "procedure_N354638"]
sha256: "618f2888616df2a8865d6537b3955d25cd91c43fda673542afad5fa8bfe455c6"
---

You can share your saved import maps with other users. After you share an import, they'll see it on their Saved CSV Imports list and can use it to run jobs. This helps avoid duplicate work and keeps your imported data consistent.

-   In the Share Import dialog, you can:
    
    -   Check the **Public** box to make the import map available to all users.
        
    -   Check the **Allow Audience to Edit** box if you want others to make changes and save with the same name. If you don't enable this option, users can make changes but can only select **Save As** to save the import map with a different name.
        
    -   Change the owner by selecting another user from the dropdown list.
        
    -   If you don't want to share the import map with all users, create a more limited audience by making selections from the fields provided.
        
        -   Only roles and departments with users who have the Import CSV File permission show up in this dialog.
            
        -   If you choose both role and department, a user has to be in one of the selected roles **and** one of the selected departments to get access. Otherwise, they need to be in either group.
            

Note:

You can open the Share Import dialog from the Finished page of the Import Assistant or from the Saved CSV Imports page.

![Share Import page.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/AccountAdministration/CSVImports/ShareImport.png)

#### Opening the Share Import Dialog from the Import Assistant {#procedure_N354618}

1.  After you've saved an import job, on the Finished page, click **Share Import**.
    

#### Opening the Share Import Dialog from the Saved CSV Imports Page {#procedure_N354638}

1.  Go to _Setup > Import/Export > Saved CSV Imports_ to see all imports to which you can access.
    
2.  Review an import's setting in the **Access** column to see if it has been shared. Three settings are possible:
    
    -   Private: Only the import owner (by default, the creator) can access the import map.
        
    -   Public: All users with the Import CSV File permission can access the import map.
        
    -   Shared: Selected users can access the import map.
        
3.  Click a link in the **Access** column to open the **Share Import** dialog.
    

Note:

If you are an administrator, you can see all users' saved import maps on the Saved CSV Imports page, and you can set them to be shared with other users.

### Related Topics

-   [Working with Saved CSV Imports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N353796.html)
-   [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html)
-   [Translating Import Map Name and Description](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354788.html)
-   [Including Import Maps and CSV Files in SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N355009.html)
-   [Editing a Saved Import](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N354236.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
