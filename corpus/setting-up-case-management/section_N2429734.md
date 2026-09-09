---
id: "section_N2429734"
type: "section"
title: "Uploading Files Through an Online Case Form"
branch: "setting-up-case-management"
category: "support-management"
breadcrumb: "Support Management > Setting Up Case Management > Online Case Forms > Uploading Files Through an Online Case Form"
parent: "section_N2428291"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429734.html"
anchors: ["procedure_N2429787"]
sha256: "4b2156b287c2afc1d21e84e0d69b4c6d4b4217c9913e7e3d29aabe41b9c5a472"
---

You can set up your online case forms to allow customers to upload files, like screenshots, to help your support reps resolve cases. Uploaded files can be up to 10 MB in size. For a list of supported file types, see [File Types Recognized in the File Cabinet](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N544425.html).

When a file is uploaded through an online case form, it's attached to the case record in the following places:

-   The Attachments column on the Communication subtab of the case record.
    
-   The Files subtab on the Communication subtab of the case record.
    
-   The Attachments subtab of the message record.
    
    You can view the message record by clicking View next to the message on the Messages subtab.
    

![Screenshot of the Incident Information page, Messages subtab on the Communications subtab where the user is uploading an attachement.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SupportManagement/CRM_feature_10614_reply_links.png)

Files uploaded through online case forms are saved in the File Cabinet, in the Attachments Received folder, which contains subfolders named after customers who filed the cases. If the file is too large or of an unsupported type, the case is saved but the file isn't uploaded. To upload multiple files, use the .zip format.

Important:

Files attached directly to cases can be accessed by external roles, even if they're not visible on the case record.

To share files with case assignees only, attach the files to case messages. For more information, see [Entering a Case](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162402065037.html).

#### To allow files to be uploaded through an online case form: {#procedure_N2429787}

1.  Open the online case form record.
    
2.  On the **Select Fields** subtab, in the **Field** column, select **File**.
    
    You can also optionally do the following:
    
    -   Enter a new label for the field.
        
    -   Choose which section of your form the field appears on.
        
    -   Change the field width.
        
3.  Click **Add**.
    
4.  Click **Save**.
    
    The **Choose File** field will be added to the case form as shown below:
    
    ![Screenshot of the online case form where the user is choosing a file to upload.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/SupportManagement/online_support_form_file_upload.png)

### Related Topics

-   [Creating an Online Case Form](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/article_162307025197.html)
-   [Linking to Online Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429074.html)
-   [Custom HTML Form Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2429943.html)
-   [Online Case Forms](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N2428291.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
