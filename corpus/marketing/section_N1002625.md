---
id: "section_N1002625"
type: "section"
title: "Creating an Email Marketing Campaign"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Email Marketing Campaigns > Creating an Email Marketing Campaign"
parent: "chapter_N992514"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1002625.html"
anchors: ["procedure_N1002637", "bridgehead_4055191346"]
sha256: "4bf80f6e64210a576e8563321a9326efad4775b12ff9bbc1be4683e412503f14"
---

Email marketing campaigns are used to generate email messages you send as part of a marketing effort.

#### To create an email marketing campaign: {#procedure_N1002637}

1.  Go to _Campaigns > Marketing > Marketing Campaigns > New_.
    
2.  Under Primary Information:
    
    1.  If you use custom forms, you can select a custom campaign form.
        
    2.  Enter an ID for this campaign in one of the following ways:
        
        -   If you use auto-generated numbers for campaigns, NetSuite automatically generates an ID.
            
            For more information, see [Set Auto-Generated Numbers](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N252198.html).
            
        -   If you do not use auto-generated numbers for campaigns, enter an ID.
            
        
        You can use campaign IDs to identify campaigns, especially when campaigns share similar names. In addition, you can use campaign IDs when you pass lead source information into online customer forms.
        
    3.  Enter a title for this campaign.
        
        You can enter up to 99 characters in this field.
        
    4.  Select the category this campaign belongs in.
        
        You can create new campaign categories at _Setup > Marketing > Campaign Management > Categories > New_.
        
    5.  Select a campaign manager for this campaign.
        
        The campaign manager receives confirmation that email campaign events have been sent.
        
    6.  Enter or pick the start date and end date for this campaign.
        
    7.  In the **Base Cost** field, enter the cost of this campaign apart from the cost of any specific campaign events.
        
        The **Total Cost** field shows the sum of the cost of any campaign events and the base cost.
        
    8.  Enter the URL for the campaign landing page or online customer form associated with this campaign.
        
        You can enter the cost of specific events on the **Events** subtab.
        
    9.  In the **Expected Revenue** field, enter the amount of revenue you expect this campaign to generate.
        
3.  Under the **Events** subtab, click the **Email** subtab.
    
4.  In the **Target Group** column, select the group to receive the campaign email.
    
    You can create new groups at _Commerce > Marketing > Personalization > Groups > New_.
    
5.  To test this email campaign and send it to only a portion of this group, select the test cell you want to send it to.
    
    For more information, see [Marketing Test Cells](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003925.html).
    
6.  Select a template category in the **Template Category** column to filter the list of email templates to that category.
    
    This field is available only if you have use the CRM Template Categories feature.
    
7.  Select the template for the email in the **Email Template** column.
    
    You can set up email templates at _Documents > Templates > Marketing Templates > New_.
    
8.  Enter a title for this campaign event.
    
9.  The **Subscription** column displays the subscription category for the template in use. Only recipients that have this subscription receive this campaign event. For more information, see [Campaign Subscription Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996344.html).
    
10.  Enter the cost incurred by this campaign event.
     
11.  In the **Status** column, select the status of the campaign event.
     
     Note:
     
     **Execute** instructs NetSuite to your email on the date and time specified in the **Delivery Date** and **Delivery Time** fields.
     
12.  Select the date and time you want this campaign event to occur.
     
13.  To associate a promotion with this campaign event, select it in the **Promotion** column.
     
14.  Click **Add/Edit**.
     
15.  Repeat these steps for each event for this email campaign.
     
16.  Click **Save**.
     

NetSuite automatically deletes duplicate messages to ensure that each email address only receives one copy of the campaign email you send.

After you save a campaign record, you can view additional subtabs on that record. Go to _Campaigns > Marketing > Marketing Campaigns_. Click the name of the campaign you want to view. You can view statistics on what recipients did with email messages, add notes to the campaign record and attach file cabinet documents.

Your Campaign Calendar keeps track of your campaign events. To view your campaign calendar, go to _Campaigns > Marketing > Campaign Calendar_.

Only customers that haven't unsubscribed to your marketing campaigns can receive marketing email. Every email message you send includes an "Unsubscribe" link your customers can click to automatically unsubscribe to your email marketing campaigns.

## Handling of Spam When Notified by Mail Service Providers {#bridgehead_4055191346}

NetSuite supports **Complaint Feedback Loop** by which mail service providers notify NetSuite when a campaign email was marked as spam by a recipient. NetSuite automatically unsubscribes the recipient from their marketing subscription preferences and sets their global subscription status to **Confirmed Opt-Out**. The unsubscribed recipient no longer receives email campaigns, which keeps the complaint rate per domain low. A low complaint rate increases the likelihood of ISPs delivering your messages to the inbox of your customers. Customers can also opt-out by clicking the unsubscribe link provided in the email.

For more information about creating email marketing templates, read [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).

### Related Topics

-   [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html)
-   [Using Variable Envelope Return Paths](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N514666.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
