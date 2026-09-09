---
id: "section_N990539"
type: "section"
title: "Tracking Campaign Responses"
branch: "marketing"
category: "marketing-sales-force-automation-and-partners"
breadcrumb: "Marketing, Sales Force Automation, and Partners > Marketing > Managing Campaigns > Campaign Metrics > Tracking Campaign Responses"
parent: "section_N990085"
source: "https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990539.html"
anchors: ["bridgehead_3829748539", "procedure_N990746", "procedure_1026020914", "bridgehead_4054372800"]
sha256: "eb24e95916854033043d47c1e33142682666e1488d81f22f2059ea614d60eadf"
---

Campaign response information helps you refine how you deliver your campaigns.

You can track the following responses from campaign recipients. You can view these responses in the Response Detail column of the campaign response record:

-   **Received** - The recipient received the campaign but hasn't responded or purchased. This status is only applicable to non-email campaigns.
    
-   **Responded** - The recipient did one of the following:
    
    -   Replied to the From address on the campaign email message
        
    -   Submitted an online customer form that included the campaign's lead source or promotion
        
-   **Purchased** - The recipient made a purchase because of the campaign.
    
-   **Sent** - NetSuite sent the campaign.
    

You can also track the following responses to email campaigns:

-   **Queued** - The email is in a queue to be sent but hasn't yet been sent.
    
-   **Opened** - The recipient opened the email message.
    
-   **Clicked Thru** - The recipient opened and clicked a link in the email message.
    
    Note:
    
    Recipient response data is only tracked for links to NetSuite pages, not third-party sites.
    
-   **Failed - delivery failure** - NetSuite sent the email, but it could not be delivered.
    
-   **Failed - invalid address** - Email delivery failed due to an invalid email address. This is also known as a hard bounce. For more information about managing hard bounces, see [Managing Bounced Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_3869562023.html).
    
-   **Failed - miscellaneous delivery failure** - Email delivery failed due to a miscellaneous delivery error.
    
-   **Failed - spam** - The email was marked as spam by the recipient or the recipient's content filter. This is considered a soft bounce.
    
-   **Failed - delivery failure** - Network issues prevented email delivery. This is considered a soft bounce.
    
-   **Failed - other** - The email was not delivered due to unknown reasons. This response can only be set by SOAP web services. This is considered a soft bounce.
    
-   **Subscribed** - The recipient subscribed to your campaigns through the Unsubscribe link in the email message.
    
-   **Unsubscribed** - The recipient unsubscribed to your campaigns through the Unsubscribe link in the email message.
    

You can find additional information in the Note field of the campaign response. You can include these descriptions in searches or reports. On reports, you can add the Comment field as a column or filter. To include these responses in searches, create a Campaign type saved search. In the Criteria subtab, use the Response Comments field in Campaign Response Fields. For more information, see [Saved Searches](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N675442.html).

Note:

Email campaign responses are tracked automatically if you check the Track Outgoing Email box on the marketing template record. When a recipient opens and clicks through the email, the response is recorded. If the recipient's email client is configured to not display images or HTML, the tracking pixel does not automatically update the status of the campaign event.

Statistics on sent and bounced emails can take longer to update based on the size of your recipient list. Updates are also delayed based on the rate at which the recipient's email servers accept your email. Statistics are updated every two hours on reports and on the Statistics subtab of campaign records.

The following campaign responses are only tracked on older email campaign events. These responses are also available to searches and reports:

-   Invalid Sender Address
    
-   Mail Protocol Issues
    
-   Mailbox Disabled
    
-   Mailbox is Full
    
-   Mailbox not Accepting Messages
    
-   Media Error
    
-   Messages Exceeds Size/Limit
    
-   Network/Server Issues
    
-   Security Issues
    
-   Too Many Recipients
    

## Entering Campaign Responses {#bridgehead_3829748539}

You can manually mark a recipient's response on the Campaigns subtab of the recipient's record. This is useful for campaigns that do not automatically track response the way email campaigns do.

#### To enter a new campaign response: {#procedure_N990746}

1.  Open the recipient's record.
    
2.  Click the **Marketing** subtab.
    
3.  Click the **Campaigns** subtab.
    
4.  Click **Add Response**.
    
5.  In the New Campaign Response popup window, select the campaign the recipient responded to.
    
6.  Select the campaign event the recipient responded to.
    
7.  Enter the date and time of the response.
    
8.  In the **New Response Detail** field, select the response type.
    
9.  Enter any notes related to the response.
    
10.  Click **Save**.
     

The response history for each campaign is tracked, including the date and time of those responses.

#### To update the status of an existing campaign response: {#procedure_1026020914}

1.  Open the recipient's record.
    
2.  Click the **Marketing** subtab.
    
3.  Click the **Campaigns** subtab.
    
4.  Click **Update Status** next to the campaign event you want to update.
    
5.  In the Campaign Response popup window, set the date and time for this response.
    
6.  In the **New Response Detail** field, select the new response.
    
7.  Enter a note about the campaign response.
    
8.  Click **Save New Response**.
    

To delete all responses to a campaign, click Update Status next to the campaign. Click Actions, and then click Delete.

Note:

The Response column shows the most recent response for each campaign sent to this recipient. There may be a delay in reporting the response statuses of Sent and Bounced.

You can view how recipients respond to your campaign events with the Campaign Response Summary and Detail reports. For more information, see [Marketing Reports](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N1010316.html).

In addition, you can view data on the Statistics subtab of campaign records. This subtab provides cost analysis such as total revenue, ROI, profit, as well as cost per lead and per purchaser. You can also see the number of leads and website visitors generated by the campaign.

## Email with Multiple Links {#bridgehead_4054372800}

In a marketing email message, a **Clicked Thru** campaign response is returned when an entity clicks any link in the email message. You can see which specific links entities clicked in the Campaign Clickthrough report. For more information, see [Campaign Clickthrough Detail Report](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_4054301176.html).

### Related Topics

-   [Bounced Email](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990874.html)
-   [Campaign Metrics](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/section_N990085.html)

[General Notices](https://docs.oracle.com/en/cloud/saas/netsuite/ns-online-help/chapter_N000004.html)
