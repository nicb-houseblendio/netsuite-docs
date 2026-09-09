---
id: "section_N515295"
type: "section"
title: "Customizing Templates for System-Automated Email"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Working with Email Templates > Customizing Templates for System-Automated Email"
parent: "section_N514744"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515295.html"
anchors: ["procedure_N515395"]
sha256: "6a6992f01c20eb509aa57ab2734234d0d1763cb55adad0ef9a3ea1eb2e369b50"
---

Note:

The email templates in this topic don't support email marketing campaigns. For information about email templates for campaigns, see [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).

Users with the Set Up Company permission can modify the following system email templates for automated email notifications. See [To modify a system email template:](#procedure_N515395).The task paths in the table below show where each template is applied in NetSuite.

| **System Email Template** | **Where Do I Apply This Template?** |
| --- | --- |
| Automatic Case Closure Notification | If you are setting up a new case profile, go to Setup > Support > Case Profiles > New, then go to the Notifications tab. To edit an existing case profile, go to Setup > Support > Case Profiles, and click **Edit** next to the profile you want to modify, then go to the Notifications tab. |
| Case Assignment Support Notifications |
| Case Escalation Notifications |
| Case Update Support Notifications |
| New Case Customer Notifications |
| Messages to Customers |
| Messages to Employees |
| Customer Center Access Email | _Setup > Company > Enable Features > Web Presenc_ See [Giving Customers Access](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N322750.html) |
| Partner Center Access Email | _Lists > Relationships > Customers > Edit_ See [The Partner Center Role](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1167882.html) |
| User Access Email | _Lists > Employees > Employees_ See [Giving an Employee Access to NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N896195.html) |
| Subscription Opt-In Invitation Email | _Setup > Marketing > Marketing Preferences_ See [Sending Subscription Messages](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996083.html) |
| Subscription Opt-In Confirmation Email |
| Web Site Order Received Email | _Commerce > Websites > Website List_ > Email tab > Order Emails subtab See [Order Emails](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2573247.html#bridgehead_N2573372) |
| Web Site Order Canceled Email |
| Web Site Order Approved Email |
| Web Site Order Fulfilled Email |
| Web Site Gift Certificate Email | _Commerce > Websites > Website List_ > Email tab > Digital Delivery Emails subtab See [Digital Delivery Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2573247.html#bridgehead_N2573580) |
| Web Site Gift Certificate Confirmation Email |
| Web Site Download Available Email |
| Web Site License Code Email |
| Web Site Checkout Errors Email | _Commerce > Websites > Website List_ > Email tab > Other Emails subtab See [Other Emails](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/bridgehead_N2573247.html#bridgehead_N2573796) |
| Web Site Password Recovery Email |
| Web Site Registration Confirmation Email |

System email can use scriptable templates that refer to specific information in your NetSuite data. When NetSuite generates an email message that uses a template, it replaces the field IDs with information sourced from the recipient's record. For more information about scriptable templates, see [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html).

#### To modify a system email template: {#procedure_N515395}

1.  Go to _Setup > Company > Company Management > System Email Templates_.
    
2.  Click **Edit** next to the type of email you want to change.
    
3.  If you need to modify a non-default system email template, click **Edit** next to that template.
    
4.  If you need to modify a default system email template, you can follow one of these methods:
    
    -   In the System Email Templates page, click **Customize** next to that template.
        
    -   In the System Email Templates page, click the name of the template you want to edit. When you are in the default System Email Template record, click **Customize**.
        
5.  Optional. Enter a description of this template.
    
6.  If you use the **Multi-Language** feature, multiple language subtabs appear on the **Templates** subtab. Click the subtab for the language of the template you want to edit.
    
7.  Edit the subject text, as required.
    
8.  In the **Create Template From** field, choose whether to modify template text and tags in the text editor, or to substitute an uploaded file.
    
    -   To use a file, choose the **File** option button. Then, click **Add New** to upload a file to the file cabinet. You can also click **Open** to open an existing file in the cabinet file.
        
    -   To modify the existing template in the text editor, choose the **Text Editor** button. Then, edit text and tags in the field below.
        
        Use the following fields to display tags for inclusion on the template:
        
        -   Select a record type in the **Field Type** list. This selection determines options in **Select Field** list.
            
        -   Select a field in the **Select Field** list. This selection determines the tag that displays in the **Tag** field.
            
        -   You can replace the tag displayed in the **Tag** field with information from each recipient's record. Place the tag between angle brackets in your template.
            
9.  If you do not want the customized template available to all users, click the **Restrict Access** subtab.
    
    -   To be the only user for this template, check the **Private** box.
        
    -   To restrict the use of this template to a group of employees, select the group in the **Restrict To Group** field. (You can create a new group record at Lists > Groups > New.)
        
10.  Click the **Categories** subtab to assign this template to other template categories.
     
     -   Select the required category from the **Template Category** list.
         
     -   Click **Attach** to associate the template with the selected category.
         
11.  Click **Save**.
     

You can optionally set the default email template for the following email template types:

-   Customer Center Access
    
-   Partner Center Access
    
-   User Access
    

Select the default template to use on the Templates subtab in _Setup > Company > Email > Email Preferences_. For more information about email preferences, see [Setting Email Preferences](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4375043929.html).

### Related Topics

-   [Working with Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514744.html)
-   [Creating New Email Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N515055.html)
-   [Scriptable Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3775087812.html)
-   [Sending Email from NetSuite](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N512264.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
