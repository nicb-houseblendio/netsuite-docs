---
id: "section_N3381747"
type: "section"
title: "File and Folder Management in Bundles"
branch: "suitebundler"
category: "suitecloud-platform"
breadcrumb: "SuiteCloud Platform > SuiteBundler > SuiteApp Creation and Distribution > Bundle Builder Reference > File and Folder Management in Bundles"
parent: "section_4422668647"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381747.html"
anchors: ["bridgehead_4287995733"]
sha256: "64e5e6be28a345085ec8b0104294551861f5e832ab09aa851c4252f9621b4f4d"
---

You can use the Bundle Builder to include files and folders from the File Cabinet in a bundle. When a user installs the bundle, NetSuite installs the files and folders included in the bundle into the target account. You can use this feature to include any File Cabinet file in a bundle.

To include a file or folder in a bundle, you must first check the **Available for SuiteBundles** box on the file or folder record. The file or folder record then appears in the Bundle Builder.

The installation location in the target account depends on the source account type:

| Source Account Type | Installation Location |
| --- | --- |
| Sandbox | NetSuite installs the files and folders with the same path information as the source account. The installation location is the same for bundles installed from a sandbox account to another sandbox account, or for bundles installed from a sandbox account into a production account. The Preview Install page for SuiteBundler displays the folder and file paths for the files included in the bundle. Use this information to determine the changes that the bundle makes to the files and folders in the target account. Note: This feature does not apply for bundles created in Version 2014 Release 2 or earlier and installed in Version 2015 Release 1 or later, or for bundles installed from a production account into another production account. |
| Production | If it does not already exist, NetSuite creates a folder called **SuiteBundles** in the target account and installs all files and folders into a subfolder that contains the bundle ID in the title. For example, if you include a file named `foo.js` in a bundle with an ID of 100, NetSuite installs the file into the following File Cabinet directory in the target account: `/SuiteBundles/Bundle 100/foo.js` A user can access this file or folder with a descriptive URL that references the file and folder location. See [Accessing Installed Files and Folders with Descriptive URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4288167433.html). |

The following screenshot shows an example of using the Bundle Builder to include folders in a bundle:

![Select Objects selecting a list of folders.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SuiteCloudCustomizationScriptingWebServices/SuiteBundler/FolderBundleObjects.png)

## Rules and Guidelines for Bundling Files and Folders {#bridgehead_4287995733}

Important:

Follow these rules and guidelines for bundling files and folders.

-   If the file or folder included in a bundle already exists in the target account, NetSuite updates the file or folder and the associated properties from the source account.
    
-   To update a file or folder in a bundle after you create the bundle, edit the bundle and update the file or folder. When a user installs or updates the bundle, the file or folder is installed or updated with the changes. See [Editing a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3392791.html).
    
    Note:
    
    When a remote file that was added to the File Cabinet using a URL is modified, the File Content Hash field changes when you download this file or its parent folder from the File Cabinet. The value of the File Content Hash field also changes when NetSuite accesses the modified file through an internal process, such as a SuiteScript method call, or a SuiteFlow workflow step. This change is reflected in the system notes for that file. For more information, see [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html).
    
-   If you are creating a bundle on a sandbox account for installation in a production account, and you include a file from a subfolder, but do not explicitly include the folder in the bundle, NetSuite automatically includes the complete folder path for the file. The included subfolders do not appear on the Set Preferences page in the Bundle Builder. However, you can use the Preview Bundle Install page to view the included files and folders when you install the bundle.
    
-   If you include a file or folder in a bundle and then clear the **Available for Suitebundles** box, NetSuite still includes the file or folder in the bundle. To remove the object, edit the bundle and remove the file or folder.
    
-   Use the **Hide in SuiteBundles** box to restrict access to server SuiteScript files.
    
-   NetSuite may automatically include files in a bundle due to dependency on other objects. For instance, including a script deployment record also includes the script file. However, if you lock the script deployment record, NetSuite does not automatically lock the script file. You must manually lock the script file for the script deployment.
    
-   Including large folders in a bundle can extend installation time, in some cases causing network connection problems that result in a failed installation. To ensure successful installation, try one of the following:
    
    -   Divide folder contents into smaller bundles.
        
    -   Instead of transferring folder contents to the target account through a bundle installation, you can export all folder contents from the File Cabinet of the source account to a ZIP file and then upload that ZIP file to the File Cabinet of the target account, where you have installed the bundle. For more information, see [Downloading Files from the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N544050.html) and [Uploading Files to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html).
        
        However, even if you exclude some files from bundle installation and import them to the target account through a ZIP file afterward, some objects in the bundle can still reference such previously excluded files and pull them into the target account during bundle installation, thus resulting into duplicate files being installed in the target account.
        
        There is also a difference in where the files are installed in the File Cabinet, depending on whether you choose to install the files through a bundle, or import the files through a ZIP file.
        
        For example, if you include a file named `foo.js` in a bundle with an ID of 100, NetSuite installs the file into the following File Cabinet directory in the target account:
        
        `/SuiteBundles/Bundle 100/foo.js`
        
        However, if you decide to exclude files from bundle installation and import them to the target account through a ZIP file instead, the files imported to the File Cabinet in the target account retain the same folder structure as in the source account.
        

### Related Topics

-   [Bundle Builder Reference](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4422668647.html)
-   [Hiding Bundle Components in Target Accounts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380618.html)
-   [Using Bundle Installation Scripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377481.html)
-   [Bundle Support during NetSuite Release Phasing](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382536.html)
-   [Documenting a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3380831.html)
-   [Defining Bundle Terms of Service](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3381364.html)
-   [Protecting Your Bundled Server SuiteScripts](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3377764.html)
-   [Adding Files and Folders to a Bundle](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4288166972.html)
-   [Installing a Bundle That Contains Files and Folders](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4288183771.html)
-   [Accessing Installed Files and Folders with Descriptive URLs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4288167433.html)
-   [Bundling NetSuite Financial Statements](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3382176.html)
-   [Bundle Object Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376108.html)
-   [Locking Objects in Customization Bundles](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N3376982.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
