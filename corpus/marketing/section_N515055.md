---
id: "section_N515055"
type: "section"
title: "Creating New Email Templates"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Email Templates > Creating New Email Templates"
parent: "section_N514744"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515055.html"
anchors: ["procedure_N515082"]
sha256: "98a84a27317fb4cfe14ea8bb20617685f85e514c0c4b0af8ba779a551caa7938"
---

Note:

The email templates in this topic don't support email marketing campaigns. For information about email templates for campaigns, see [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).

You can create email templates outside of NetSuite in a basic word processing application, or directly on the Template subtab of email template records. If you create an email template outside of NetSuite, save your template as a plain text (.txt) or an HTML (.html or .htm) file.

Email templates can use FreeMarker code to personalize and customize the messages you send. For more information, see [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html).

When you select an email template in the Send Email popup on a record, the text from your template appears in the Message field. You can modify the template message before you send the email message.

If you don't prepare your template file beforehand, you can compose the message in the Template field of the email template record.

#### To create an email template record: {#procedure_N515082}

1.  Go to _Documents > Templates > Email Templates > New_.
    
2.  Enter a name for this template.
    
3.  From the **Record Type** list, select the required type of template.
    
    If you select a record type, NetSuite restricts the template's availability to send email from only those record types. Leave this field blank if you want the template to be available across all record types.
    
4.  In the **Description** field, enter a short summary of what the template is used for. The description appears on the template list page.
    
5.  On the **Template** subtab, in the **Subject** field, enter the subject of the email.
    
6.  Do one of the following:
    
    -   Select **File** if you created the email template beforehand. Then select the template file.
        
        Select **New** if you have not uploaded your template file to your file cabinet.
        
    -   Select **Text Editor** if you have not created your email template. Compose your template in the text field.
        
        To insert a field, select the type of record you want to insert a field from. Then select a field in the **Insert Field** list.
        
        As you type the message, misspelled words appear underlined in red. To correct a word, press and hold CRTL and then right-click the correct spelling.
        
7.  On the **Restrict Access** subtab, check the **Private** box if you do not want others to use this template.
    
8.  If you want members of a specific group to use this template, select that group in the **Restrict to Group** field.
    
9.  Click the **Marketing** subtab.
    
10.  Check the **Add Unsubscribe Link to Message Footer in Bulk Merges** box.
     
     This option adds a link to the **Campaign Subscription Center** to the footer of email messages sent with this template.
     
11.  Check the **Add Company Address to Message Footer in Bulk Messages** box.
     
     This option displays your company's address in the footer of email sent with this template.
     
12.  Select the campaign email domain to use for this email template.
     
     Campaign domains replace any reference to netsuite.com in the email message you send with templates. Campaign domains are required if you send more than 10,000 email messages each month through campaigns or email merge operations.
     
13.  Select the campaign subscription associated with this email template.
     
     You can create new campaign subscription categories at Setup > Marketing > Campaign Subscriptions > New.
     
14.  Click the **Categories** subtab.
     
15.  In the **Template Category** column, select the category you want to organize this template into.
     
     For more information see, [Creating Email Template Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4534668235.html).
     
16.  Click **Add**.
     
17.  Repeat these steps for each category you want to organize this template into. A template can be in multiple categories.
     
18.  Click **Save**.
     

Note:

You can use SuiteCloud Development Framework (SDF) to manage custom email templates as part of file-based customization projects. For information about SDF, see [SuiteCloud Development Framework](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_4702622163.html).

You can use the Copy to Account feature to copy an individual custom email template to another of your accounts. When you edit a custom email template, a clickable **Copy to Account** option is available in the upper right corner. For information about Copy to Account, see [Copy to Account](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_1544019532.html).

### Related Topics

-   [Adding File Attachments to Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html#bridgehead_4519058066)
-   [Attaching Files to Email Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1004674.html)
-   [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html)
-   [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html)
-   [Customizing Templates for System-Automated Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515295.html)
-   [Sending Email from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512264.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
