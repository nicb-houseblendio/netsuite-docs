---
id: "section_N523426"
type: "section"
title: "Working with Mail Merge"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge"
parent: "chapter_N992514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N523426.html"
anchors: ["bridgehead_N523577"]
sha256: "a1c48e44f701777c00d65697ff7ae66d11d62e24edccc5a1c2d80aaa11e848d8"
---

Note:

This topic is unrelated to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

In NetSuite, the mail merge feature lets you create personalized letters, bulk email messages, faxes, and mailing labels from your NetSuite data.

Click one of the links below for information about specific mail merge processes.

-   [Merging Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html)
    
-   [Merging Letters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525062.html)
    
-   [Merging Faxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N527062.html)
    
-   [Merging PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530117.html)
    

The Mail Merge feature is best used for communication that does not need to be reported on. If you need to view reports on recipient response or revenue generation, you should use the Marketing Automation feature. For more information, see [Marketing Automation Overview](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N973384.html).

## Setting Up Mail Merge {#bridgehead_N523577}

To use the mail merge feature, an administrator must go to _Setup > Company > Enable Features_, and click the CRM subtab. In the Marketing section, click the Terms of Service link under Mail Merge. Read the NetSuite Inc. Terms of Service for Campaign Marketing Services, and click I Agree. Check the Mail Merge box, and click Save. If this feature is not available in your account, please contact your account manager.

To perform a mail merge, ensure you have fulfilled the prerequisites for performing a merge such as a group record. Some mail merge processes require a template and a template record. You can create a template file outside of NetSuite or fill in the message field. Upload the template created outside of NetSuite to your NetSuite file cabinet. Next, create a template record in NetSuite to correspond with the template file you created. For more information, see [Using Letter Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525773.html).

For example, a sales rep might use mail merge to print personalized thank you letters to their customers after they close deals. The sales rep might include their first name in the greeting. In this case you would use a scriptable template that inserts personalized information for each recipient. For more information about scriptable templates, see [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html).

PDF and letter templates use CRMSDK tags. For more information, see [Using CRMSDK Tags](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515605.html).

After you upload your template and create a template record, you create a group that includes the recipients of your mail merge document. For more information, see [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html).

After you create a template and a target group, go to Documents > Mail Merge > Bulk Merge to process your mail merge.

The following table shows the different kinds of mail merge templates and the file format for each kind of template.

| **Template type** | **File format** | Used in |
| --- | --- | --- |
| **Fax** | plain text (.txt) or FreeMarker (.ftl) | fax merge operations |
| **E-mail** | plain text (.txt), HTML, or FreeMarker (.ftl) | email to contacts, email merge operations, online form auto-replies |
| **Letter** | Word file (.doc) | letter merge operations |
| **PDF** | PDF file (.pdf) | PDF merge operation |

### Related Topics

-   [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html)
-   [Viewing Bulk Merge History](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4230927265.html)
-   [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html)
-   [Merging Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html)
-   [Merging Letters](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N525062.html)
-   [Merging Faxes](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N527062.html)
-   [Merging PDFs](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N530117.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
