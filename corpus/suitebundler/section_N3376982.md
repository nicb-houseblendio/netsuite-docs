---
id: "section_N3376982"
type: "section"
title: "Locking Objects in Customization Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > Locking Objects in Customization Bundles"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html"
anchors: ["bridgehead_N3377087", "bridgehead_N3377144"]
sha256: "80259ba2d1a6a95d6a0c53d58fcde300ef7fe373a85ccfcc93470643d8cfa290"
---

A bundle author can lock some of the objects in a customization bundle on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder. When an administrator installs a bundle containing locked objects, these locked objects cannot be edited. Sometimes editing objects in a bundle can break a solution or make future upgrades impossible without data loss. Locking prevents this and allows customization in a controlled and safe manner.

Object locking provides bundle authors and independent software vendors (ISVs) the ability to control which aspects of their solution can be extended and customized to avoid upgrade issues. In addition, locking can ensure compatibility when bundle updates are rolled out.

Before a NetSuite account administrator installs or updates a bundle, the administrator can view which components in the bundle are locked, on the Preview Bundle Install Page. When an installed bundle includes locked objects, these objects' NetSuite pages do not have buttons that allow changes to the object, such as Edit, Delete, and Change ID. Also, all list and view pages display a lock icon to provide complete visibility of locked objects in installed bundles.

You can lock bundle objects as part of bundle creation or editing. To lock a bundle object, check the Lock on Install box on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the Bundle Builder.

Warning:

You should not lock bundle objects to be included in a bundle developed in sandbox. Locking objects in the source sandbox account for the bundle can eventually lead to the objects being locked in that account. After the bundle is installed in production and the sandbox account is later refreshed, the production account settings for locked objects are copied to the sandbox account. This copy causes the objects to be locked in the source sandbox account, with their lock options disabled, preventing bundle developers from editing these objects.

The installation of a bundle that contains locked objects requires the same steps as installing a bundle with no locked objects. For a detailed description of the procedure used to install a bundle, see [Installing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3395142.html). Also, see [Review Locked Bundle Objects](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3396121.html#bridgehead_N3396378).

The [Objects Available in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3364871.html#bridgehead_N3364890) table includes a column indicating which object types are lockable.

Locking effects differ by object type. See [Effects of Locking Different Object Types](#bridgehead_N3377144).

Note:

If you bundle a component that is already locked in another installed bundle, the component stays locked in the new bundle as well.

## Precautions about Locking Bundled Objects {#bridgehead_N3377087}

Locking an object does not prevent target account users from seeing it, only from editing it. For details about how to hide bundle objects in target accounts, see [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html). For details about how to prevent target account users from seeing code in bundled server SuiteScripts, see [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html).

Warning:

Bundle locking functionality is not a tool for Intellectual Property management and should not be treated as such. The intention of this functionality is to discourage end users from making changes to locked bundle objects. Locking an object does not prevent a user from installing another third party bundle with an object of the same name that is unlocked, and that can be used to replace the locked object. However, the resulting replacement object is locked.

When you copy (rather than install) a bundle that includes locked objects, the objects are not locked in the account where the bundle is copied. However, their locked settings are maintained on the [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html) page of the copied bundle, and are enforced in target accounts where the copied bundle is installed. See [Copying a Bundle to Other Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3391248.html).

## Effects of Locking Different Object Types {#bridgehead_N3377144}

The following list summarizes the effects of locking bundle objects for target accounts:

-   **Custom Fields:** Target account administrators can control access to locked custom fields through form customization as before.
    
-   **Custom Lists:** Values cannot be added, edited, or deleted in locked custom lists in target accounts.
    
-   **Custom Records:**
    
    -   Data can be modified in locked custom records in target accounts. This means records can be added, edited, or deleted for these custom records.
        
    -   Edits to metadata are restricted for locked custom records in target accounts.
        
        -   For locked custom records that included data when installed in target accounts, no edits to metadata are allowed. Custom record fields cannot be added, edited, or deleted.
            
        -   For locked custom records that did not include data when installed in target accounts, some edits to metadata are allowed. Fields can be added to these locked custom records, and these fields can later be edited and deleted. However, custom record fields from the source account cannot be edited or deleted.
            
-   **File Cabinet**
    
    -   **Files:** In target accounts, the File Cabinet displays lock icons for locked files from installed bundles, as these files cannot be edited.
        
        ![SuiteBundles for specific bundle with lock icon on files.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/FileCabLockedFile.png)
        -   Locked files cannot be overwritten in target accounts through Add File, Advanced Add, Copy Files, or Move Files actions in the File Cabinet.
            
            For example, if a user attempts to add a file with the same name as the locked file in the same location in the target account's File Cabinet, the action is not completed and the user receives a warning that a file with the same name already exists.
            
        -   The File Cabinet Move Files and Delete Files actions are not available for these locked files. If you choose Move Files or Delete Files for a File Cabinet folder that includes any locked files, the Folder Contents page disables the box for these files and displays a lock icon for each one.
            
            ![File Cabinet with lock icon on files.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/FileCabFolderContents.png)
    -   **Folders:** In target accounts, the File Cabinet displays lock icons for files contained in locked folders from installed bundles. Files in locked bundle folders are treated in the same manner as locked bundle files, as described above.
        
-   **Custom Forms:** Target account administrators who install a bundle containing locked objects can create a new instance of the locked form and customize it to fit their needs. This is similar to standard NetSuite form behavior.
    
-   **Custom Roles:** Target account administrators who install a bundle containing locked objects, can create a copy of the locked role and further customize it to fit their needs. This is similar to standard NetSuite role handling.
    
-   **Saved Searches:** Users who have access to the saved search can create a new copy of the saved search and add or remove filters and results columns.
    
-   **SuiteScripts:** Locking script records does not lock the script deployments. Customers can change properties of the deployment to fit their business needs. Script parameters lock automatically. However, users can define values for them, if the parameter is defined as company or user preference.
    

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [File and Folder Management in Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [SuiteApp Creation and Distribution](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3364150.html)
-   [Creating a Bundle with the Bundle Builder](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3374254.html)
-   [Step 4 Set Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3373802.html)
-   [SuiteApp Installation and Update](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3394134.html)
-   [SuiteApp Development Process with SuiteBundler](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4444212213.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
