---
id: "section_N524089"
type: "section"
title: "Merging Email"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Mail Merge > Merging Email"
parent: "section_N523426"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N524089.html"
anchors: []
sha256: "ab3605b592b0cef6efae9ba1f7a03eeafe4f421ce674bc4a3611db84090da9d3"
---

Note:

All bulk email communications sent through NetSuite must meet the requirements defined in the Mass Email Messaging Terms of Service. You will see a link to the Terms of Service when you set up a bulk email merge in NetSuite.

The Email Merge feature in NetSuite lets you send personalized email messages in bulk. When you use this feature, the following actions take place:

-   NetSuite generates and sends your merged email message.
    
-   NetSuite automatically deletes duplicate messages to ensure that each email address only receives one copy of the email message.
    
-   Your login email address appears in the **From** field.
    
-   NetSuite records all messages sent by an email merge operation in Documents > Mail Merge > Merge History.
    

Note:

This topic does not relate to marketing campaigns. For information about campaigns, see [Email Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N992514.html).

Complete the following tasks before you perform an email merge:

-   Understand the terms of service for Mass Email Messaging and email best practices.
    
    You will see a link to the Terms of Service when you set up a bulk email merge in NetSuite.
    
    See [Email Best Practices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N993117.html) for information about email best practices.
    
-   Create a group that can be selected as the recipient group for bulk email messages. See [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html).
    
-   Create an email template record. See [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).
    

#### To perform an email merge:

1.  Go to Documents > Mail Merge > Bulk Merge.
    
2.  On the Select Output page, click **Email**.
    
3.  Click **Terms of Service** to read the terms of service for bulk email communications sent through NetSuite.
    
4.  Go to the **Recipients** tab to select your email recipients.
    
5.  Select the type of group you want to email from the **Group Type** list. See [Working with Groups](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N492945.html) for more information.
    
6.  Select the group you are emailing from the **Group** list.
    
    Note:
    
    For groups of over 100 members, NetSuite schedules and sends the email merge operations within an hour after you submit the merge request. For groups of fewer than 100 members, NetSuite sends the email merge operations after you submit the merge request.
    
    Note:
    
    You must set up a campaign domain to perform either of the following actions:
    
    -   Send over 100,000 email messages in a 30-day period
        
    -   Send over 10,000 email messages in any single campaign event (email blast)
        
    
    See [Campaign Email Domains](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996559.html) for more information.
    
    A list of recipients appears in the **Recipients** area. NetSuite lists only those recipients who have not opted out of your marketing campaigns.
    
7.  Check **Opt-Out Override** to ignore opt-outs to send critical updates or non-marketing emails. Enter the justification for the opt-out override in the **Opt-Out Override Reason** textbox.
    
    Note:
    
    Your justification must be compliant with General Data Protection Regulations (GDPR) and spam policies/regulations.
    
8.  Go to the **Message** tab to create your email message.
    
9.  From the **Template** list, select the email template you want to use to generate your email.
    
    Select **\-New-** to create a new email template.
    
10.  Check the **Update** box if you want changes you make to the selected template to be saved to the template file in your file cabinet.
     
11.  The subject text from the email template record appears in the **Subject** field by default. Edit this field as required.
     
12.  The message text from the email template record appears in the **Message** textbox by default. Edit this textbox as required.
     
13.  Go to the **Attachments** tab to send attachments with your email.
     
14.  Check **Zip Attachments** box if you want attachments to be compressed in a ZIP file.
     
15.  To attach a Microsoft Word document to the email message, select the letter template you want to use from the **Attach Document Template** list.
     
     Select **\-New-** to create a new letter template.
     
16.  Check the **Include Statement** box if you want to send a customer statement as an attachment with your email. Complete the following actions:
     
     -   In the **Statement Date** field, enter the date you want to appear on the attached statement.
         
     -   In the **Start Date** field, enter the date of the oldest transaction you want to appear on the attached statement. If you do not enter a start date, all transactions in the customer's history appear on the statement.
         
     -   Select one of the following types of statements to attach from the **Type** list:
         
         -   **Default From Customer** - uses the email preference from each customer's record.
             
         -   **Default** - uses HTML if you checked the **Email Using HTML** box at Home > Set Preferences > Transactions or, PDF if you didn't check the **Email Using HTML** box.
             
     -   Check the **Show Only Open Transactions** box if you only want to include open transactions on the statement. If you entered a start date, open transactions from that start date onward appear. If you didn't enter a start date, all open transactions appear.
         
     -   Check the **Consolidated Statement** box to apply payments, deposits, and credits to the top-level customers in a customer-subcustomer hierarchy. Clear this box to apply payments, deposits, and credits to any open invoice entered for any customer or subcustomer in a customer hierarchy.
         
         Note:
         
         This box is only available if you use the **Consolidated Payments** feature.
         
17.  Select a file to attach to the email in the **Attach File** column.
     
     Note:
     
     Attachments can't exceed 5 MB in size.
     
18.  Click **Add**.
     
19.  Repeat Steps 17 and 18 for each file you want to attach.
     
20.  Click **Merge & Send**.
     

### Related Topics

-   [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html)
-   [Working with Records, Transactions, and Lists](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N488023.html)
-   [Working with Mail Merge](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N523426.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
