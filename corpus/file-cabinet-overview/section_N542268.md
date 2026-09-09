---
id: "section_N542268"
type: "section"
title: "Uploading Files to the File Cabinet"
branch: "file-cabinet-overview"
category: "netsuite-basics"
breadcrumb: "NetSuite Basics > File Cabinet Overview > Working with Files > Uploading Files to the File Cabinet"
parent: "section_4811461596"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542268.html"
anchors: ["procedure_N542375"]
sha256: "703e4074083a0da45dea13898aabc64d29605eb4929064d334d5e82a25953e4d"
---

You can upload a file by clicking the Documents tab, and then selecting a folder. NetSuite accepts all file formats in the File Cabinet. The File Cabinet shows the file extension and lists the file type. You can also upload files by clicking the Communications subtab on transaction records and relationship records. When you attach files to records, you must select or create a folder where the document can be stored in the File Cabinet.

If Enhanced File Security is enabled, expense file attachments automatically submit to a dedicated employee expenses folder, predefined by the system.

You can make files available to everyone in the company, even if the file is in a private folder or not accessible to a specific group. To do this, check the Company-Wide Usage box on the file record. For more information, see [Preferences on File Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_0530052000.html).

All files uploaded to the File Cabinet are automatically scanned for viruses and malicious content. For more information, see [Antivirus Scanning on File Cabinet Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4822646785.html).

#### To upload files to a File Cabinet folder: {#procedure_N542375}

1.  Click the **Documents** tab.
    
2.  In the right pane, click the name of the folder where you want to store files.
    
    If the Enhanced File Security feature is enabled, expense file attachments are automatically uploaded to a system-defined employee expenses folder.
    
3.  To upload a file from your computer, click **Add File**.
    
4.  To add a file from the internet, or to add a .zip file, click **Advanced Add**.
    
    1.  To upload a .zip file, in the **Zip Archive to Add** field, click **Choose File**, and select the file you want to upload. Click **Open**.
        
    2.  In the **Character Encoding** field, choose the proper character encoding for the file.
        
    3.  To upload a file from the internet, in the **URL** field, enter URL path for the file location on the internet. Make sure the length of the URL isn't longer than 250 characters.
        
        Note:
        
        When a remote file that was added to the File Cabinet using a URL is modified, the File Content Hash field changes when you download this file or its parent folder from the File Cabinet. The value of the File Content Hash field also changes when NetSuite accesses the modified file through an internal process, such as a SuiteScript method call, or a SuiteFlow workflow step. This change is reflected in the system notes for that file. For more information, see [File Cabinet Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N541319.html).
        
    4.  Verify that the **Destination Folder** is where you want to upload the files.
        
    5.  To automatically extract files into the Destination folder as they're uploaded, check the **Unzip files** box.
        
    6.  (Optional) To make the files available on your website, check the **Make all Files Available Without Login** box. If you don't want to publish the files on your website, clear this box. Note that **Make All Files Available Without Login** takes precedence over **Make All Files Available for Company-Wide Usage**.
        
        Note:
        
        Enabling the Files Available Without Login capability prevents broken images and links in your website. This box is checked by default in the Images folder and the Web Site Hosting Files folder.
        
    7.  (Optional) To make the files available to all company users, check the **Make All Files Available for Company-Wide Usage** box.
        
        Note:
        
        When the box is checked, files are also available for viewing in the Customer, Vendor or Partner Centers.
        
    8.  To overwrite files that exist in the File Cabinet with the files in the .zip file, check the **Overwrite Files with Same Name** box. When the box is checked, files of the same name are automatically updated with the latest version you upload in this archive. When this box is cleared, files in the .zip archive that have the same path and name as existing files in File Cabinet aren't extracted to the File Cabinet. The same rules apply to individual files uploaded using a URL path.
        
        Only users with the Administrator role and users with the Edit level permission or higher can overwrite files in the File Cabinet.
        
        Important:
        
        This setting doesn't apply to locked files and folders that have been installed by a bundle. You can't edit or overwrite locked files and folders installed by a bundle.
        
    9.  To upload the.zip file, click **Add**.
        

To inactivate files being added using the Advanced Add form, check Make all Files Inactive. When you check this box, the file or files no longer appear on lists unless you check the Show Inactives box.

Note:

Users with the Billing Information permission can look up the amount of space the File Cabinet currently uses on the Billing Information page. Go to _Setup > Company > View Billing Information_. The Current Used Quantity column for File Cabinet Size (GB)\*\* component shows the current amount of space used.

Additional Information:

-   [Attaching Files to Records](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N490137.html)
    
-   [Attaching Files to Email Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514371.html)
    
-   [Best Practices for Preparing Files for Upload to the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_1539629264.html)
    
-   [Unsupported Symbols in File Names](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/subsect_163723987503.html)
    

Important:

Unless you've purchased additional storage space, each NetSuite account comes with 10 GB of total storage space.

For more information, see [How much storage space do I have in my NetSuite account?](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N3898540.html#question_N3900159)

### Related Topics

-   [Working with Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4811461596.html)
-   [Editing Files in the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N542738.html)
-   [Moving and Copying Files in the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N543817.html)
-   [Downloading Files from the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N544050.html)
-   [Deleting Files from the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N544279.html)
-   [File Types Recognized in the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N544425.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
