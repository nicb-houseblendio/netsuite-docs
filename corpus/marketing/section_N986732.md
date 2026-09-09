---
id: "section_N986732"
type: "section"
title: "Scheduling Campaign Events"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Managing Campaigns > Creating a Campaign Record > Scheduling Campaign Events"
parent: "section_N986170"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N986732.html"
anchors: ["procedure_N986863"]
sha256: "75e3b2d5e0a26ce9c0723bde7b39405c0108e408744950bf1fd1af5f1dd29d9f"
---

Campaign events represent individual aspects of a campaign.

For example, a campaign could include three events:

-   a series of print ads
    
-   an email message sent to existing customers
    
-   a banner ad on partner websites
    

You can create events for any channel your company uses in its marketing. The following channels are included by default: Direct Mail, Email, Phone, Print Ad, and Misc.

To create new campaign channels, go to _Setup > Marketing > Campaign Management > Channels_.

Only customers who haven't unsubscribed to your marketing campaigns can receive marketing email. Every email message you send includes an "Unsubscribe" link. Your customers can click this link to automatically unsubscribe from your email marketing campaigns.

With email campaign events, NetSuite automatically deletes duplicate messages to ensure each email address receives only one copy of your campaign mailing.

For more information about email marketing templates, see [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html).

Note:

Some of the fields listed below don't appear for all campaign channels.

#### To schedule a campaign event: {#procedure_N986863}

1.  On the campaign record, click the **Events** subtab.
    
2.  Click the subtab that corresponds with the type of event you want to schedule.
    
    Use the **Other Events** subtab to track any event that is not an email or direct mail event. For information about Lead Nurturing events, see [Lead Nurturing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003092.html).
    
3.  In the **Target Group** column, select the group that receives this campaign event.
    
    You can create new groups at _Commerce > Marketing > Personalization > Groups > New_.
    
4.  To test this campaign event, select the test cell you want to send it to.
    
    For more information, see [Marketing Test Cells](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1003925.html).
    
5.  If this event is an email or direct mail campaign event, select the template for the email or direct mail in the **Template** column.
    
    If you use the **CRM Template Categories** feature, you can select a category in the **Template Category** column to filter the list of templates.
    
    Set up marketing templates at _Documents > Templates > Marketing Templates > New_. Set up letter templates at _Documents > Templates > Letter Templates > New_.
    
6.  Enter a title for this campaign event.
    
    In the **Subscription** column, the subscription category for the selected template is chosen, by default. Only recipients that have this subscription receive this campaign event. For more information, see [Campaign Subscription Categories](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N996344.html).
    
    You can select a subscription different from the default for this template.
    
7.  In the **Channel** column, choose the method used to deliver this event.
    
    To create new campaign channels, go to _Setup > Marketing > Campaign Management > Channels_.
    
8.  Enter the cost incurred by this campaign event.
    
    When you enter a cost, you can track return on investment (ROI) for the campaign. The **Total Cost** field at the top of the page shows the sum of the base cost plus the cost of each campaign event.
    
9.  In the **Status** column, select the status of the campaign event.
    
    If you select **Execute** for an email campaign event, NetSuite send your email on the date and time you set.
    
10.  Select the date and time this campaign event will occur.
     
     Note:
     
     You can't change the time of day an email campaign executes on the day it's scheduled to execute.
     
11.  To associate a promotion with this campaign event, select the promotion.
     
     Promotions enable you to track discounts offered through a campaign.
     
     Important:
     
     You shouldn't associate a promotion with multiple campaigns or campaign events.
     
     You can create new promotions at _Lists > Marketing > Promotions_.
     
12.  Leave the field **Internal ID** empty.
     
     When you save the campaign, NetSuite generates a number for this field. This internal ID appears in forms as **Event ID** or **Campaign Event**, so that you can track event responses.
     
     ![The Events subtab with an empty Internal ID field.](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/img/MarketingSalesForceAutomationPartners/Marketing/5461sched_camp_events.png)
13.  Click **Add**.
     
14.  Repeat these steps for other campaign events you want to schedule within this campaign.
     

### Related Topics

-   [Campaign Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N987776.html)
-   [Initiating Campaign Events](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N989408.html)
-   [Adding Paid Search Keyword Information to Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N987245.html)
-   [Campaign Notes and Files](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N987446.html)
-   [Email Marketing Templates](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N1001310.html)
-   [How Customers Opt In to Marketing Campaigns](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N995569.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
