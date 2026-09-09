---
id: "section_N527062"
type: "section"
title: "Merging Faxes"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge > Merging Faxes"
parent: "section_N523426"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N527062.html"
anchors: ["procedure_N529199"]
sha256: "53c0f7cc7d21f673a6c2a841c2da9dbbdb1085717055251d607a41ab4a076ca5"
---

Note:

This topic is unrelated to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

Fax merge lets you send personalized faxes in bulk to those with whom you do business.

Before you perform a fax merge you must have:

-   Created a group record for the recipients of your faxes.
    
-   Prepared a fax template. See [Using Fax Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html).
    
-   Created a fax template record. See [Creating a Fax Template](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html#bridgehead_N529703) and [Creating a Fax Template Record](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html#bridgehead_N529835).
    

NetSuite merges and sends your faxes. NetSuite automatically deletes duplicate messages to ensure that each fax number receives only one copy.

You must have an account with eFax to perform a fax merge in NetSuite. For more information about this service, see [Fax Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_163594359424.html).

#### To perform a fax merge: {#procedure_N529199}

1.  Go to _Documents > Mail Merge > Bulk Merge_.
    
2.  On the Select Output page, click **Fax**.
    
3.  On the **Recipients** subtab, in the **Group Type** field, select the type of group to receive the fax.
    
4.  In the **Group** field, select the group to receive the fax.
    
    Note:
    
    For groups with more than 100 members, NetSuite schedules and sends the fax merge operations within an hour of submission. For groups with fewer than 100 members, NetSuite sends the fax merge operations at submission. You can't send fax merge operations to groups with more than 4000 members.
    
    You can create new groups at _Commerce > Marketing > Personalization > Groups > New_.
    
    A list of recipients appears on the **Recipients** subtab.
    
5.  Click the **Message** subtab.
    
6.  In the **Template** field, select the fax template you want to use to generate the faxed documents.
    
    Select **New** to create a new fax template record.
    
7.  Check the **Update** box to save changes you make to the message in the template file.
    
    The subject entered on the fax template record appears in the **Subject** field, by default. You can edit this subject for the merge.
    
    The message text from the template appears in the **Message** field.
    
8.  You can edit this message for this merge.
    
    If you checked the **Update** box, NetSuite saves the changes you make to the template file in your file cabinet.
    
9.  To attach files to your faxes, click the **Attachments** subtab.
    
10.  To compress attachments in a ZIP file, check the **Zip Attachments** box.
     
11.  Select a file to attach to the fax in the **Attach File** column.
     
     Attached files print as additional pages with your fax.
     
     Attachments can't exceed 5MB in size. You may incur additional charges from your fax service when you send attachments.
     
12.  Click **Add**.
     
13.  Repeat these steps for each file you want to attach.
     
14.  Click **Merge & Send**.
     

NetSuite records all messages sent in mail merge operations at _Documents > Mail Merge > Merge History_.

### Related Topics

-   [Using Fax Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N529539.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
