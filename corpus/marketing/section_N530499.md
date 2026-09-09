---
id: "section_N530499"
type: "section"
title: "Using PDF Templates"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge > Using PDF Templates"
parent: "section_N523426"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530499.html"
anchors: ["bridgehead_N530583", "procedure_N530690", "bridgehead_N530804", "procedure_N530930"]
sha256: "eb0cc09345a5725f0ca0d761629a704f0c8d4c34663918e3e3737fd64dd30af1"
---

Note:

This topic is unrelated to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

PDF templates are PDF documents you create for use in mail merge operations. NetSuite uses PDF templates to generate personalized documents that you can send to those with whom you do business.

You create PDF templates outside of NetSuite, and then upload them to your file cabinet. NetSuite then merges your template with the data contained in each recipient's record. When the merge is complete, you can download a ZIP file that contains each of your personalized PDF documents.

PDF templates can include CRMSDK tags that refer to specific information in your NetSuite data. When NetSuite merges your data with your template, information that corresponds with the recipient's record replaces the CRMSDK tags. For a list of CRMSDK tags, see [Using CRMSDK Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html).

## Creating a PDF Template {#bridgehead_N530583}

PDF templates are especially useful when you create documents that should not be edited. For example, contracts, user licenses, and proposals.

To prepare a PDF template, first create a document in a format that you can convert to PDF. Then, use Adobe Acrobat to convert your document to PDF format.

#### To insert CRMSDK tags in your PDF template: {#procedure_N530690}

1.  Open the PDF template file in Adobe Acrobat.
    
2.  Click the **Form Tool** button.
    
3.  Place a tag in the document with the **Form** Tool.
    
4.  In the Field Properties popup window, enter the CRMSDK tag in the **Name** field.
    
    This tag should be all capital letters and have no angle brackets.
    
5.  Click **OK**.
    
6.  Repeat these steps for each tag you want to place in the document.
    
7.  Save your template file.
    

## Creating a PDF Template Record {#bridgehead_N530804}

After you upload your PDF template file to your file cabinet, you can create a PDF template record.

#### To create a PDF template record: {#procedure_N530930}

1.  Go to _Documents > Templates > PDF Templates > New_.
    
2.  Enter a name for this template.
    
    The Mail Merge page displays this name on the **Template** subtab.
    
3.  In the **Subject** field, enter the subject of the PDF file.
    
4.  In the **Description** field, enter information about this template.
    
5.  Do one of the following:
    
    -   In the **Template File** field, select the template file.
        
    -   Select **\-New-** if you have not uploaded your template file to your file cabinet.
        
6.  Optional. Check the **Private** box if you do not want others in your company to use this template.
    
7.  Optional. If you want this template to be used by members of a specific group, select this group in the **Restrict to Group** field.
    
    Private templates can't be restricted to a group.
    
8.  Click **Save**.
    

Merge your PDF documents with your NetSuite data. For more information, see [Merging PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530117.html).

### Related Topics

-   [Merging PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530117.html)
-   [Working with Mail Merge](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N523426.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
